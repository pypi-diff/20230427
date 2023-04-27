# Comparing `tmp/mypylib-0.1.70.tar.gz` & `tmp/mypylib-0.1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.1.70.tar", last modified: Tue Apr 18 13:51:29 2023, max compression
+gzip compressed data, was "mypylib-0.1.71.tar", last modified: Thu Apr 27 13:12:10 2023, max compression
```

## Comparing `mypylib-0.1.70.tar` & `mypylib-0.1.71.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-18 13:51:29.294130 mypylib-0.1.70/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-04-18 13:51:29.293904 mypylib-0.1.70/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.70/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-18 13:51:29.291403 mypylib-0.1.70/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.70/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    47005 2023-04-18 13:49:04.000000 mypylib-0.1.70/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.70/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.70/mypylib/binance_copy_bot_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.70/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.70/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.70/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.70/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24230 2022-06-02 06:59:21.000000 mypylib-0.1.70/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.70/mypylib/mytest.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.70/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.70/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.70/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.70/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.70/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.70/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7662 2022-06-02 06:59:21.000000 mypylib-0.1.70/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-18 13:51:29.293153 mypylib-0.1.70/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.70/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.70/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2443 2023-01-29 12:44:04.000000 mypylib-0.1.70/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8467 2023-01-12 13:51:57.000000 mypylib-0.1.70/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.70/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-18 13:51:29.292679 mypylib-0.1.70/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-04-18 13:51:28.000000 mypylib-0.1.70/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      654 2023-04-18 13:51:29.000000 mypylib-0.1.70/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-04-18 13:51:28.000000 mypylib-0.1.70/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-04-18 13:51:29.000000 mypylib-0.1.70/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-04-18 13:51:29.294210 mypylib-0.1.70/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.70/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-27 13:12:10.191868 mypylib-0.1.71/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-04-27 13:12:10.191624 mypylib-0.1.71/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.71/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-27 13:12:10.188927 mypylib-0.1.71/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.71/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    47074 2023-04-27 13:11:20.000000 mypylib-0.1.71/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.71/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.71/mypylib/binance_copy_bot_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.71/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.71/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.71/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.71/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24230 2022-06-02 06:59:21.000000 mypylib-0.1.71/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.71/mypylib/mytest.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.71/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.71/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.71/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.71/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.71/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.71/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7662 2022-06-02 06:59:21.000000 mypylib-0.1.71/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-27 13:12:10.191007 mypylib-0.1.71/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.71/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.71/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.71/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8467 2023-01-12 13:51:57.000000 mypylib-0.1.71/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.71/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-27 13:12:10.190471 mypylib-0.1.71/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-04-27 13:12:09.000000 mypylib-0.1.71/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      654 2023-04-27 13:12:10.000000 mypylib-0.1.71/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-04-27 13:12:09.000000 mypylib-0.1.71/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-04-27 13:12:09.000000 mypylib-0.1.71/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-04-27 13:12:10.191966 mypylib-0.1.71/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.71/setup.py
```

### Comparing `mypylib-0.1.70/README.md` & `mypylib-0.1.71/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/MP_shioaji_ticks.py` & `mypylib-0.1.71/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/__init__.py` & `mypylib-0.1.71/mypylib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import requests
 
 ssl._create_default_https_context = ssl._create_unverified_context
 from termcolor import cprint
 from inspect import currentframe
 
-__version__ = '0.1.70'
+__version__ = '0.1.71'
 
 __info__ = {
     '2022/01/04: 0.1.18 加入 __info__。',
     '2022/01/04: 0.1.18 Carey修改 MVP的部分。',
     '2022/01/05: 0.1.19 add check_place_cover 預防漲停鎖住',
     '2022/01/06: 0.1.20 add get_stock_future_data(). 用來抓取每天股票期貨資料',
     '2022/01/06: 0.1.20 add get_stock_future_snapshot(). 用來抓每天股票、股票期貨漲停、跌停價格',
@@ -58,15 +58,16 @@
     '2023/01/29: 0.1.63 del xls in read_warrant_bible()',
     '2023/01/29: 0.1.64 add block for playsound class',
     '2023/02/12: 0.1.65 修改 sjtools parse timestamp的方法，以免crash',
     '2023/02/13: 0.1.66 Move toggle_btn_off and toggle_btn_on here ',
     '2023/02/23: 0.1.67 get_new_warrant_list() 元富修改網站，封鎖 read_html()',
     '2023/03/15: 0.1.68 修正一些宣告',
     '2023/04/11: 0.1.69 換成shioaji 1.0 API',
-    '2023/04/18: 0.1.70 Market() 增加 ask bid information'
+    '2023/04/18: 0.1.70 Market() 增加 ask bid information',
+    '2023/04/27: 0.1.71 tplaysound 減少buffer音量以免很吵',
 
 }
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
```

### Comparing `mypylib-0.1.70/mypylib/binance_copy_bot.py` & `mypylib-0.1.71/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/binance_copy_bot_test.py` & `mypylib-0.1.71/mypylib/binance_copy_bot_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/chdbif.py` & `mypylib-0.1.71/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/crypto.py` & `mypylib-0.1.71/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/finmind.py` & `mypylib-0.1.71/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/libexcel.py` & `mypylib-0.1.71/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/mvp.py` & `mypylib-0.1.71/mypylib/mvp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/mytest.py` & `mypylib-0.1.71/mypylib/mytest.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/option_test.py` & `mypylib-0.1.71/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/shioaji_history_ticks.py` & `mypylib-0.1.71/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/shioaji_kline.py` & `mypylib-0.1.71/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/shioaji_ticks.py` & `mypylib-0.1.71/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/sjtools.py` & `mypylib-0.1.71/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/tLineNotify.py` & `mypylib-0.1.71/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/ti.py` & `mypylib-0.1.71/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.1.71/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/tplaysound.py` & `mypylib-0.1.71/mypylib/tplaysound.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
     def __init__(self):
         threading.Thread.__init__(self)
 
         self.time_block = 2
 
         self.queue = queue.Queue()
+        self.queue.maxsize = 2
+
 
         self.file_sound_alert = f'{_MYPYLIB_ROOT}/../data/alert.wav'
 
         self.start()
 
         self.dict_filename_to_datetime = defaultdict(datetime.datetime.now)
 
@@ -38,15 +40,18 @@
         if filename is None:
             filename = self.file_sound_alert
 
         if self.block_or_not(filename):
             return
 
         command = ('play', filename)
-        self.queue.put(command)
+        try:
+            self.queue.put(command, False)
+        except queue.Full:
+            pass
         # print(f'send command {command}')
 
     def run(self):
         while True:
             try:
                 (cmd, arg) = self.queue.get(timeout=1)
             except queue.Empty:
```

### Comparing `mypylib-0.1.70/mypylib/tredis.py` & `mypylib-0.1.71/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib/warrant.py` & `mypylib-0.1.71/mypylib/warrant.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/mypylib.egg-info/SOURCES.txt` & `mypylib-0.1.71/mypylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.70/setup.py` & `mypylib-0.1.71/setup.py`

 * *Files identical despite different names*


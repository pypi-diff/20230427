# Comparing `tmp/RStockvn-2.1.6.tar.gz` & `tmp/RStockvn-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RStockvn-2.1.6.tar", last modified: Wed Mar  1 05:06:53 2023, max compression
+gzip compressed data, was "RStockvn-2.1.8.tar", last modified: Thu Apr 27 03:05:18 2023, max compression
```

## Comparing `RStockvn-2.1.6.tar` & `RStockvn-2.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 05:06:53.704657 RStockvn-2.1.6/
--rw-rw-rw-   0        0        0     1090 2023-01-29 04:27:43.000000 RStockvn-2.1.6/LICENSE
--rw-rw-rw-   0        0        0     9446 2023-03-01 05:06:53.704657 RStockvn-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     8586 2023-03-01 05:06:26.000000 RStockvn-2.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-03-01 05:06:53.657651 RStockvn-2.1.6/RStockvn/
--rw-rw-rw-   0        0        0      831 2023-03-01 05:01:13.000000 RStockvn-2.1.6/RStockvn/__init__.py
--rw-rw-rw-   0        0        0     2447 2023-03-01 05:00:32.000000 RStockvn-2.1.6/RStockvn/cafef_test.py
--rw-rw-rw-   0        0        0     6344 2023-03-01 05:00:59.000000 RStockvn-2.1.6/RStockvn/data_cafef.py
--rw-rw-rw-   0        0        0    19726 2023-03-01 02:37:56.000000 RStockvn-2.1.6/RStockvn/stockvn.py
--rw-rw-rw-   0        0        0   139694 2023-02-06 06:33:27.000000 RStockvn-2.1.6/RStockvn/user_agent.py
-drwxrwxrwx   0        0        0        0 2023-03-01 05:06:53.704657 RStockvn-2.1.6/RStockvn.egg-info/
--rw-rw-rw-   0        0        0     9446 2023-03-01 05:06:53.000000 RStockvn-2.1.6/RStockvn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-03-01 05:06:53.000000 RStockvn-2.1.6/RStockvn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 05:06:53.000000 RStockvn-2.1.6/RStockvn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-03-01 05:06:53.000000 RStockvn-2.1.6/RStockvn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-01 05:06:53.000000 RStockvn-2.1.6/RStockvn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-01 05:06:53.704657 RStockvn-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1215 2023-03-01 05:01:39.000000 RStockvn-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:05:18.641405 RStockvn-2.1.8/
+-rw-rw-rw-   0        0        0     1090 2023-01-29 04:27:43.000000 RStockvn-2.1.8/LICENSE
+-rw-rw-rw-   0        0        0     9446 2023-04-27 03:05:18.640404 RStockvn-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8586 2023-03-01 05:06:26.000000 RStockvn-2.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 03:05:18.589154 RStockvn-2.1.8/RStockvn/
+-rw-rw-rw-   0        0        0      833 2023-04-27 02:56:04.000000 RStockvn-2.1.8/RStockvn/__init__.py
+-rw-rw-rw-   0        0        0     2668 2023-04-27 03:01:50.000000 RStockvn-2.1.8/RStockvn/cafef_test.py
+-rw-rw-rw-   0        0        0     6344 2023-03-01 05:00:59.000000 RStockvn-2.1.8/RStockvn/data_cafef.py
+-rw-rw-rw-   0        0        0    19726 2023-03-01 05:09:24.000000 RStockvn-2.1.8/RStockvn/stockvn.py
+-rw-rw-rw-   0        0        0   139694 2023-02-06 06:33:27.000000 RStockvn-2.1.8/RStockvn/user_agent.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:05:18.638021 RStockvn-2.1.8/RStockvn.egg-info/
+-rw-rw-rw-   0        0        0     9446 2023-04-27 03:05:18.000000 RStockvn-2.1.8/RStockvn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-04-27 03:05:18.000000 RStockvn-2.1.8/RStockvn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 03:05:18.000000 RStockvn-2.1.8/RStockvn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-27 03:05:18.000000 RStockvn-2.1.8/RStockvn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 03:05:18.000000 RStockvn-2.1.8/RStockvn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 03:05:18.641405 RStockvn-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1215 2023-04-27 03:02:27.000000 RStockvn-2.1.8/setup.py
```

### Comparing `RStockvn-2.1.6/LICENSE` & `RStockvn-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `RStockvn-2.1.6/PKG-INFO` & `RStockvn-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RStockvn
-Version: 2.1.6
+Version: 2.1.8
 Summary: Report Finance of Companies in Vietnamese and macro data - Lấy báo cáo tài chính của các công ty ở Việt Nam và số liệu vĩ mô
 Home-page: https://github.com/NPhucBinh/RStockvn
 Author: NGUYEN PHUC BINH
 Author-email: nguyenphucbinh67@gmail.com
 Keywords: RStockvn,rpv,rstockvn,report stock vn,báo cáo tài chính việt nam,lấy báo cáo tài chính việt nam bằng python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RStockvn-2.1.6/README.md` & `RStockvn-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `RStockvn-2.1.6/RStockvn/__init__.py` & `RStockvn-2.1.8/RStockvn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 __author__ ="Nguyen Phuc Binh"
 __copyright__ = "Copyright 2023, Nguyen Phuc Binh"
 __license__ = "MIT"
 __email__ = "nguyenphucbinh67@gmail.com"
 __website__ = "https://github.com/NPhucBinh"
 
 from . import user_agent
-from . import data_cafef
-from . import cafef_test
+#from . import data_cafef
+#from . import cafef_test
 from .stockvn import (report_finance_cf,report_finance_cp68,get_data_history_cafef,getCPI_vietstock,solieu_GDP_vietstock
                       ,info_company,trade_internal,laisuat_vietstock,event_price_cp68,exchange_currency,
                       tygia_vietstock,historical_price_cp68,solieu_XNK_vietstock,solieu_tindung_vietstock,solieu_sanxuat_congnghiep
                       ,solieu_banle_vietstock,solieu_danso_vietstock,solieu_FDI_vietstock,baocaonhanh)
```

### Comparing `RStockvn-2.1.6/RStockvn/cafef_test.py` & `RStockvn-2.1.8/RStockvn/cafef_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2023 Nguyen Phuc Binh @ GitHub
 # See LICENSE for details.
-__version__ = "2.1.6"
+__version__ = "2.1.8"
 __author__ ="Nguyen Phuc Binh"
 __copyright__ = "Copyright 2023, Nguyen Phuc Binh"
 __license__ = "MIT"
 __email__ = "nguyenphucbinh67@gmail.com"
 __website__ = "https://github.com/NPhucBinh"
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
@@ -13,35 +13,38 @@
 import sys
 import time
 
 class browser_get_data():
     
     def __init__(self,mck,fromdate,todate):
         from selenium.webdriver.chrome.options import Options
+        from .user_agent import random_user
+        self.useragent=random_user()
         self.url='https://s.cafef.vn/Lich-su-giao-dich-VNINDEX-1.chn#data'
         self.opt=Options()
-        self.opt.add_argument('--headless')
+        #self.opt.add_argument('--headless')
         self.opt.add_argument('--dark-mode-settings')
         self.opt.add_argument("--incognito")
         self.opt.add_argument('--disable-gpu')
         self.opt.add_argument('--no-default-browser-check')
+        self.opt.add_argument("user-agent={}".format(self.useragent))
         self.br=webdriver.Chrome(options=self.opt)
         self.br.maximize_window()
         self.br.get(self.url)
         self.mcp=self.br.find_element(By.ID,'ContentPlaceHolder1_ctl03_txtKeyword')
         self.mcp.clear()
         self.mcp.send_keys(mck)
         self.br.find_element(By.ID,'ContentPlaceHolder1_ctl03_dpkTradeDate1_txtDatePicker').send_keys(str(fromdate))
         self.br.find_element(By.ID,'ContentPlaceHolder1_ctl03_dpkTradeDate2_txtDatePicker').send_keys(str(todate))
         self.br.find_element(By.ID,'ContentPlaceHolder1_ctl03_btSearch').click()
     
     def getdata(self):
         self.lis=[]
         while True:
-            time.sleep(0.1)
+            time.sleep(0.6)
             try:
                 self.br.find_element(By.LINK_TEXT,'>').click()
                 df=self.dataframe()
                 self.lis.append(df)
             except:
                 df=self.dataframe()
                 self.lis.append(df)
@@ -50,12 +53,14 @@
         data.drop(['Thay đổi (+/-%).1'],axis=1,inplace=True)
         data.rename(columns={'KL':'KLGD khớp lệnh','GT':'GTGD khớp lệnh','KL.1':'KLGD thỏa thuận','GT.1':'GTGD thỏa thuận'}, inplace=True)
         self.close()
         return data.reset_index(drop=True)
     
     def dataframe(self):
         import pandas as pd
-        df=pd.read_html(self.br.page_source,header=1,encoding='utf-8')
-        return df[0]
+        df=pd.read_html(self.br.page_source,encoding='utf-8',header=0)
+        data=pd.DataFrame(df[2])
+        data=data.drop(index=0)
+        return data
     
     def close(self):
         self.br.quit()
```

### Comparing `RStockvn-2.1.6/RStockvn/data_cafef.py` & `RStockvn-2.1.8/RStockvn/data_cafef.py`

 * *Files identical despite different names*

### Comparing `RStockvn-2.1.6/RStockvn/stockvn.py` & `RStockvn-2.1.8/RStockvn/stockvn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2023 Nguyen Phuc Binh @ GitHub
 # See LICENSE for details.
-__version__ = "2.1.5"
+__version__ = "2.1.6"
 __author__ ="Nguyen Phuc Binh"
 __copyright__ = "Copyright 2023, Nguyen Phuc Binh"
 __license__ = "MIT"
 __email__ = "nguyenphucbinh67@gmail.com"
 __website__ = "https://github.com/NPhucBinh"
 
 import pandas as pd
```

### Comparing `RStockvn-2.1.6/RStockvn/user_agent.py` & `RStockvn-2.1.8/RStockvn/user_agent.py`

 * *Files identical despite different names*

### Comparing `RStockvn-2.1.6/RStockvn.egg-info/PKG-INFO` & `RStockvn-2.1.8/RStockvn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RStockvn
-Version: 2.1.6
+Version: 2.1.8
 Summary: Report Finance of Companies in Vietnamese and macro data - Lấy báo cáo tài chính của các công ty ở Việt Nam và số liệu vĩ mô
 Home-page: https://github.com/NPhucBinh/RStockvn
 Author: NGUYEN PHUC BINH
 Author-email: nguyenphucbinh67@gmail.com
 Keywords: RStockvn,rpv,rstockvn,report stock vn,báo cáo tài chính việt nam,lấy báo cáo tài chính việt nam bằng python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RStockvn-2.1.6/setup.py` & `RStockvn-2.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = fh.read()
 
 DS = 'Report Finance of Companies in Vietnamese and macro data - Lấy báo cáo tài chính của các công ty ở Việt Nam và số liệu vĩ mô'
 
 #Setting
 setup(
     name='RStockvn',
-    version='2.1.6',
+    version='2.1.8',
     author='NGUYEN PHUC BINH',
     author_email='nguyenphucbinh67@gmail.com',
     description=DS,
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     url="https://github.com/NPhucBinh/RStockvn",
```


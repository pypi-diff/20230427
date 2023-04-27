# Comparing `tmp/jquants_api_client-1.1.1.tar.gz` & `tmp/jquants_api_client-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jquants_api_client-1.1.1.tar", max compression
+gzip compressed data, was "jquants_api_client-1.1.2.tar", max compression
```

## Comparing `jquants_api_client-1.1.1.tar` & `jquants_api_client-1.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-04-11 01:31:26.267331 jquants_api_client-1.1.1/LICENSE
--rw-r--r--   0        0        0     5631 2023-04-11 01:31:26.267331 jquants_api_client-1.1.1/README.md
--rw-r--r--   0        0        0       66 2023-04-11 01:31:26.271331 jquants_api_client-1.1.1/jquantsapi/__init__.py
--rw-r--r--   0        0        0    48163 2023-04-11 01:31:26.271331 jquants_api_client-1.1.1/jquantsapi/client.py
--rw-r--r--   0        0        0    15206 2023-04-11 01:31:26.271331 jquants_api_client-1.1.1/jquantsapi/constants.py
--rw-r--r--   0        0        0      517 2023-04-11 01:31:26.271331 jquants_api_client-1.1.1/jquantsapi/enums.py
--rw-r--r--   0        0        0     1676 2023-04-11 01:31:38.435493 jquants_api_client-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     7141 1970-01-01 00:00:00.000000 jquants_api_client-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 04:50:47.685389 jquants_api_client-1.1.2/LICENSE
+-rw-r--r--   0        0        0     5631 2023-04-27 04:50:47.685389 jquants_api_client-1.1.2/README.md
+-rw-r--r--   0        0        0       66 2023-04-27 04:50:47.685389 jquants_api_client-1.1.2/jquantsapi/__init__.py
+-rw-r--r--   0        0        0    54334 2023-04-27 04:50:47.685389 jquants_api_client-1.1.2/jquantsapi/client.py
+-rw-r--r--   0        0        0    15206 2023-04-27 04:50:47.685389 jquants_api_client-1.1.2/jquantsapi/constants.py
+-rw-r--r--   0        0        0      517 2023-04-27 04:50:47.685389 jquants_api_client-1.1.2/jquantsapi/enums.py
+-rw-r--r--   0        0        0     1676 2023-04-27 04:51:00.489623 jquants_api_client-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7141 1970-01-01 00:00:00.000000 jquants_api_client-1.1.2/PKG-INFO
```

### Comparing `jquants_api_client-1.1.1/LICENSE` & `jquants_api_client-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.1.1/README.md` & `jquants_api_client-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.1.1/jquantsapi/client.py` & `jquants_api_client-1.1.2/jquantsapi/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -311,15 +311,15 @@
     )
     def get_id_token(self, refresh_token: Optional[str] = None) -> str:
         """
         get J-Quants API id_token
 
         Params:
             refresh_token: J-Quants API refresh token
-        Retruns:
+        Returns:
             id_token: J-Quants API id token
         """
         if self._id_token_expire > pd.Timestamp.utcnow():
             return self._id_token
 
         if refresh_token is not None:
             _refresh_token = refresh_token
@@ -352,31 +352,36 @@
             raise e
         id_token = ret.json()["idToken"]
         self._id_token = id_token
         self._id_token_expire = pd.Timestamp.utcnow() + pd.Timedelta(23, unit="hour")
         return self._id_token
 
     # /listed
-    def _get_listed_info_raw(self, code: str = "", date_yyyymmdd: str = "") -> str:
+    def _get_listed_info_raw(
+        self, code: str = "", date_yyyymmdd: str = "", pagination_key: str = ""
+    ) -> str:
         """
         Get listed companies raw API returns
 
         Args:
             code: Issue code (Optional)
             date: YYYYMMDD or YYYY-MM-DD (Optional)
+            pagination_key: ページングキー
 
         Returns:
             str: listed companies raw json string
         """
         url = f"{self.JQUANTS_API_BASE}/listed/info"
         params = {}
         if code != "":
             params["code"] = code
         if date_yyyymmdd != "":
             params["date"] = date_yyyymmdd
+        if pagination_key != "":
+            params["pagination_key"] = pagination_key
         ret = self._get(url, params)
         ret.encoding = self.RAW_ENCODING
         return ret.text
 
     def get_listed_info(self, code: str = "", date_yyyymmdd: str = "") -> pd.DataFrame:
         """
         Get listed companies
@@ -386,15 +391,25 @@
             date: YYYYMMDD or YYYY-MM-DD (Optional)
 
         Returns:
             pd.DataFrame: listed companies (sorted by Code)
         """
         j = self._get_listed_info_raw(code=code, date_yyyymmdd=date_yyyymmdd)
         d = json.loads(j)
-        df = pd.DataFrame.from_dict(d["info"])
+        data = d["info"]
+        while "pagination_key" in d:
+            j = self._get_listed_info_raw(
+                code=code,
+                date_yyyymmdd=date_yyyymmdd,
+                pagination_key=d["pagination_key"],
+            )
+            d = json.loads(j)
+            data += d["info"]
+        df = pd.DataFrame.from_dict(data)
+
         cols = constants.LISTED_INFO_COLUMNS
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
         df["Date"] = pd.to_datetime(df["Date"], format="%Y-%m-%d")
         df.sort_values("Code", inplace=True)
         return df[cols]
 
@@ -477,23 +492,25 @@
     # /prices
     def _get_prices_daily_quotes_raw(
         self,
         code: str = "",
         from_yyyymmdd: str = "",
         to_yyyymmdd: str = "",
         date_yyyymmdd: str = "",
+        pagination_key: str = "",
     ) -> str:
         """
         get daily quotes raw API returns
 
         Args:
             code: 銘柄コード
             from_yyyymmdd: 取得開始日
             to_yyyymmdd: 取得終了日
             date_yyyymmdd: 取得日
+            pagination_key: ページングキー
 
         Returns:
             str: daily quotes
         """
         url = f"{self.JQUANTS_API_BASE}/prices/daily_quotes"
         params = {
             "code": code,
@@ -501,14 +518,16 @@
         if date_yyyymmdd != "":
             params["date"] = date_yyyymmdd
         else:
             if from_yyyymmdd != "":
                 params["from"] = from_yyyymmdd
             if to_yyyymmdd != "":
                 params["to"] = to_yyyymmdd
+        if pagination_key != "":
+            params["pagination_key"] = pagination_key
         ret = self._get(url, params)
         ret.encoding = self.RAW_ENCODING
         return ret.text
 
     def get_prices_daily_quotes(
         self,
         code: str = "",
@@ -531,15 +550,26 @@
         j = self._get_prices_daily_quotes_raw(
             code=code,
             from_yyyymmdd=from_yyyymmdd,
             to_yyyymmdd=to_yyyymmdd,
             date_yyyymmdd=date_yyyymmdd,
         )
         d = json.loads(j)
-        df = pd.DataFrame.from_dict(d["daily_quotes"])
+        data = d["daily_quotes"]
+        while "pagination_key" in d:
+            j = self._get_prices_daily_quotes_raw(
+                code=code,
+                from_yyyymmdd=from_yyyymmdd,
+                to_yyyymmdd=to_yyyymmdd,
+                date_yyyymmdd=date_yyyymmdd,
+                pagination_key=d["pagination_key"],
+            )
+            d = json.loads(j)
+            data += d["daily_quotes"]
+        df = pd.DataFrame.from_dict(data)
         premium_flag = "MorningClose" in df.columns
         if premium_flag:
             cols = constants.PRICES_DAILY_QUOTES_PREMIUM_COLUMNS
         else:
             cols = constants.PRICES_DAILY_QUOTES_COLUMNS
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
@@ -577,29 +607,34 @@
                 df = future.result()
                 buff.append(df)
         return pd.concat(buff).sort_values(["Code", "Date"])
 
     def _get_prices_prices_am_raw(
         self,
         code: str = "",
+        pagination_key: str = "",
     ) -> str:
         """
         get the morning session's high, low, opening, and closing prices for individual stocks raw API returns
 
         Args:
             code: issue code (e.g. 27800 or 2780)
                 If a 4-digit issue code is specified, only the data of common stock will be obtained
                 for the issue on which both common and preferred stocks are listed.
+            pagination_key: ページングキー
+
         Returns:
             str: the morning session's OHLC data
         """
         url = f"{self.JQUANTS_API_BASE}/prices/prices_am"
         params = {
             "code": code,
         }
+        if pagination_key != "":
+            params["pagination_key"] = pagination_key
         ret = self._get(url, params)
         ret.encoding = self.RAW_ENCODING
         return ret.text
 
     def get_prices_prices_am(
         self,
         code: str = "",
@@ -613,49 +648,62 @@
                 for the issue on which both common and preferred stocks are listed.
         Returns: pd.DataFrame: the morning session's OHLC data
         """
         j = self._get_prices_prices_am_raw(
             code=code,
         )
         d = json.loads(j)
-        if d.get("message"):
-            return d["message"]
-        df = pd.DataFrame.from_dict(d["prices_am"])
+        data = d["prices_am"]
+        while "pagination_key" in d:
+            if d.get("message"):
+                return d["message"]
+            j = self._get_prices_prices_am_raw(
+                code=code,
+                pagination_key=d["pagination_key"],
+            )
+            d = json.loads(j)
+            data += d["prices_am"]
+        df = pd.DataFrame.from_dict(data)
         cols = constants.PRICES_PRICES_AM_COLUMNS
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
         df["Date"] = pd.to_datetime(df["Date"], format="%Y-%m-%d")
         df.sort_values(["Code"], inplace=True)
         return df[cols]
 
     # /markets
     def _get_markets_trades_spec_raw(
         self,
         section: Union[str, enums.MARKET_API_SECTIONS] = "",
         from_yyyymmdd: str = "",
         to_yyyymmdd: str = "",
+        pagination_key: str = "",
     ) -> str:
         """
         Weekly Trading by Type of Investors raw API returns
 
         Args:
             section: section name (e.g. "TSEPrime" or MARKET_API_SECTIONS.TSEPrime)
             from_yyyymmdd: starting point of data period (e.g. 20210901 or 2021-09-01)
             to_yyyymmdd: end point of data period (e.g. 20210907 or 2021-09-07)
+            pagination_key: ページングキー
+
         Returns:
             str: Weekly Trading by Type of Investors
         """
         url = f"{self.JQUANTS_API_BASE}/markets/trades_spec"
         params = {}
         if section != "":
             params["section"] = section
         if from_yyyymmdd != "":
             params["from"] = from_yyyymmdd
         if to_yyyymmdd != "":
             params["to"] = to_yyyymmdd
+        if pagination_key != "":
+            params["pagination_key"] = pagination_key
         ret = self._get(url, params)
         ret.encoding = self.RAW_ENCODING
         return ret.text
 
     def get_markets_trades_spec(
         self,
         section: Union[str, enums.MARKET_API_SECTIONS] = "",
@@ -672,15 +720,25 @@
         Returns:
             pd.DataFrame: Weekly Trading by Type of Investors (Sorted by "PublishedDate" and "Section" columns)
         """
         j = self._get_markets_trades_spec_raw(
             section=section, from_yyyymmdd=from_yyyymmdd, to_yyyymmdd=to_yyyymmdd
         )
         d = json.loads(j)
-        df = pd.DataFrame.from_dict(d["trades_spec"])
+        data = d["trades_spec"]
+        while "pagination_key" in d:
+            j = self._get_markets_trades_spec_raw(
+                section=section,
+                from_yyyymmdd=from_yyyymmdd,
+                to_yyyymmdd=to_yyyymmdd,
+                pagination_key=d["pagination_key"],
+            )
+            d = json.loads(j)
+            data += d["trades_spec"]
+        df = pd.DataFrame.from_dict(data)
         cols = constants.MARKETS_TRADES_SPEC
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
         df["PublishedDate"] = pd.to_datetime(df["PublishedDate"], format="%Y-%m-%d")
         df["StartDate"] = pd.to_datetime(df["StartDate"], format="%Y-%m-%d")
         df["EndDate"] = pd.to_datetime(df["EndDate"], format="%Y-%m-%d")
         df.sort_values(["PublishedDate", "Section"], inplace=True)
@@ -688,39 +746,43 @@
 
     def _get_markets_weekly_margin_interest_raw(
         self,
         code: str = "",
         from_yyyymmdd: str = "",
         to_yyyymmdd: str = "",
         date_yyyymmdd: str = "",
+        pagination_key: str = "",
     ) -> str:
         """
         get weekly margin interest raw API returns
 
         Args:
             code: issue code (e.g. 27800 or 2780)
                 If a 4-digit issue code is specified, only the data of common stock will be obtained
                 for the issue on which both common and preferred stocks are listed.
             from_yyyymmdd: starting point of data period (e.g. 20210901 or 2021-09-01)
             to_yyyymmdd: end point of data period (e.g. 20210907 or 2021-09-07)
             date_yyyymmdd: date of data (e.g. 20210907 or 2021-09-07)
+            pagination_key: ページングキー
         Returns:
             str: weekly margin interest
         """
         url = f"{self.JQUANTS_API_BASE}/markets/weekly_margin_interest"
         params = {
             "code": code,
         }
         if date_yyyymmdd != "":
             params["date"] = date_yyyymmdd
         else:
             if from_yyyymmdd != "":
                 params["from"] = from_yyyymmdd
             if to_yyyymmdd != "":
                 params["to"] = to_yyyymmdd
+        if pagination_key != "":
+            params["pagination_key"] = pagination_key
         ret = self._get(url, params)
         ret.encoding = self.RAW_ENCODING
         return ret.text
 
     def get_markets_weekly_margin_interest(
         self,
         code: str = "",
@@ -744,15 +806,26 @@
         j = self._get_markets_weekly_margin_interest_raw(
             code=code,
             from_yyyymmdd=from_yyyymmdd,
             to_yyyymmdd=to_yyyymmdd,
             date_yyyymmdd=date_yyyymmdd,
         )
         d = json.loads(j)
-        df = pd.DataFrame.from_dict(d["weekly_margin_interest"])
+        data = d["weekly_margin_interest"]
+        while "pagination_key" in d:
+            j = self._get_markets_weekly_margin_interest_raw(
+                code=code,
+                from_yyyymmdd=from_yyyymmdd,
+                to_yyyymmdd=to_yyyymmdd,
+                date_yyyymmdd=date_yyyymmdd,
+                pagination_key=d["pagination_key"],
+            )
+            d = json.loads(j)
+            data += d["weekly_margin_interest"]
+        df = pd.DataFrame.from_dict(data)
         cols = constants.MARKETS_WEEKLY_MARGIN_INTEREST
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
         df["Date"] = pd.to_datetime(df["Date"], format="%Y-%m-%d")
         df.sort_values(["Date", "Code"], inplace=True)
         return df[cols]
 
@@ -790,37 +863,41 @@
 
     def _get_markets_short_selling_raw(
         self,
         sector_33_code: str = "",
         from_yyyymmdd: str = "",
         to_yyyymmdd: str = "",
         date_yyyymmdd: str = "",
+        pagination_key: str = "",
     ) -> str:
         """
         get daily short sale ratios and trading value by industry (sector) raw API returns
 
         Args:
             sector_33_code: 33-sector code (e.g. 0050 or 8050)
             from_yyyymmdd: starting point of data period (e.g. 20210901 or 2021-09-01)
             to_yyyymmdd: end point of data period (e.g. 20210907 or 2021-09-07)
             date_yyyymmdd: date of data (e.g. 20210907 or 2021-09-07)
+            pagination_key: ページングキー
         Returns:
             str: daily short sale ratios and trading value by industry
         """
         url = f"{self.JQUANTS_API_BASE}/markets/short_selling"
         params = {
             "sector33code": sector_33_code,
         }
         if date_yyyymmdd != "":
             params["date"] = date_yyyymmdd
         else:
             if from_yyyymmdd != "":
                 params["from"] = from_yyyymmdd
             if to_yyyymmdd != "":
                 params["to"] = to_yyyymmdd
+        if pagination_key != "":
+            params["pagination_key"] = date_yyyymmdd
         ret = self._get(url, params)
         ret.encoding = self.RAW_ENCODING
         return ret.text
 
     def get_markets_short_selling(
         self,
         sector_33_code: str = "",
@@ -842,16 +919,28 @@
         """
         j = self._get_markets_short_selling_raw(
             sector_33_code=sector_33_code,
             from_yyyymmdd=from_yyyymmdd,
             to_yyyymmdd=to_yyyymmdd,
             date_yyyymmdd=date_yyyymmdd,
         )
+
         d = json.loads(j)
-        df = pd.DataFrame.from_dict(d["short_selling"])
+        data = d["short_selling"]
+        while "pagination_key" in d:
+            j = self._get_markets_short_selling_raw(
+                sector_33_code=sector_33_code,
+                from_yyyymmdd=from_yyyymmdd,
+                to_yyyymmdd=to_yyyymmdd,
+                date_yyyymmdd=date_yyyymmdd,
+                pagination_key=d["pagination_key"],
+            )
+            d = json.loads(j)
+            data += d["short_selling"]
+        df = pd.DataFrame.from_dict(data)
         cols = constants.MARKET_SHORT_SELLING_COLUMNS
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
         df["Date"] = pd.to_datetime(df["Date"], format="%Y-%m-%d")
         df.sort_values(["Date", "Sector33Code"], inplace=True)
         return df[cols]
 
@@ -888,39 +977,43 @@
 
     def _get_markets_breakdown_raw(
         self,
         code: str = "",
         from_yyyymmdd: str = "",
         to_yyyymmdd: str = "",
         date_yyyymmdd: str = "",
+        pagination_key: str = "",
     ) -> str:
         """
         get detail breakdown trading data raw API returns
 
         Args:
             code: issue code (e.g. 27800 or 2780)
                 If a 4-digit issue code is specified, only the data of common stock will be obtained
                 for the issue on which both common and preferred stocks are listed.
             from_yyyymmdd: starting point of data period (e.g. 20210901 or 2021-09-01)
             to_yyyymmdd: end point of data period (e.g. 20210907 or 2021-09-07)
             date_yyyymmdd: date of data (e.g. 20210907 or 2021-09-07)
+            pagination_key: ページングキー
         Returns:
             str: detail breakdown trading data
         """
         url = f"{self.JQUANTS_API_BASE}/markets/breakdown"
         params = {
             "code": code,
         }
         if date_yyyymmdd != "":
             params["date"] = date_yyyymmdd
         else:
             if from_yyyymmdd != "":
                 params["from"] = from_yyyymmdd
             if to_yyyymmdd != "":
                 params["to"] = to_yyyymmdd
+        if pagination_key != "":
+            params["pagination_key"] = pagination_key
         ret = self._get(url, params)
         ret.encoding = self.RAW_ENCODING
         return ret.text
 
     def get_markets_breakdown(
         self,
         code: str = "",
@@ -944,15 +1037,26 @@
         j = self._get_markets_breakdown_raw(
             code=code,
             from_yyyymmdd=from_yyyymmdd,
             to_yyyymmdd=to_yyyymmdd,
             date_yyyymmdd=date_yyyymmdd,
         )
         d = json.loads(j)
-        df = pd.DataFrame.from_dict(d["breakdown"])
+        data = d["breakdown"]
+        while "pagination_key" in d:
+            j = self._get_markets_breakdown_raw(
+                code=code,
+                from_yyyymmdd=from_yyyymmdd,
+                to_yyyymmdd=to_yyyymmdd,
+                date_yyyymmdd=date_yyyymmdd,
+                pagination_key=d["pagination_key"],
+            )
+            d = json.loads(j)
+            data += d["breakdown"]
+        df = pd.DataFrame.from_dict(data)
         cols = constants.MARKETS_BREAKDOWN_COLUMNS
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
         df["Date"] = pd.to_datetime(df["Date"], format="%Y-%m-%d")
         df.sort_values(["Code"], inplace=True)
         return df[cols]
 
@@ -988,30 +1092,34 @@
         return pd.concat(buff).sort_values(["Code", "Date"])
 
     # /indices
     def _get_indices_topix_raw(
         self,
         from_yyyymmdd: str = "",
         to_yyyymmdd: str = "",
+        pagination_key: str = "",
     ) -> str:
         """
         TOPIX Daily OHLC raw API returns
 
         Args:
             from_yyyymmdd: starting point of data period (e.g. 20210901 or 2021-09-01)
             to_yyyymmdd: end point of data period (e.g. 20210907 or 2021-09-07)
+            pagination_key: ページングキー
         Returns:
             str: TOPIX Daily OHLC
         """
         url = f"{self.JQUANTS_API_BASE}/indices/topix"
         params = {}
         if from_yyyymmdd != "":
             params["from"] = from_yyyymmdd
         if to_yyyymmdd != "":
             params["to"] = to_yyyymmdd
+        if pagination_key != "":
+            params["pagination_key"] = pagination_key
         ret = self._get(url, params)
         ret.encoding = self.RAW_ENCODING
         return ret.text
 
     def get_indices_topix(
         self,
         from_yyyymmdd: str = "",
@@ -1026,39 +1134,53 @@
         Returns:
             pd.DataFrame: TOPIX Daily OHLC (Sorted by "Date" column)
         """
         j = self._get_indices_topix_raw(
             from_yyyymmdd=from_yyyymmdd, to_yyyymmdd=to_yyyymmdd
         )
         d = json.loads(j)
-        df = pd.DataFrame.from_dict(d["topix"])
+        data = d["topix"]
+        while "pagination_key" in d:
+            j = self._get_indices_topix_raw(
+                from_yyyymmdd=from_yyyymmdd,
+                to_yyyymmdd=to_yyyymmdd,
+                pagination_key=d["pagination_key"],
+            )
+            d = json.loads(j)
+            data += d["topix"]
+        df = pd.DataFrame.from_dict(data)
         cols = constants.INDICES_TOPIX_COLUMNS
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
         df["Date"] = pd.to_datetime(df["Date"], format="%Y-%m-%d")
         df.sort_values(["Date"], inplace=True)
         return df[cols]
 
     # /fins
-    def _get_fins_statements_raw(self, code: str = "", date_yyyymmdd: str = "") -> str:
+    def _get_fins_statements_raw(
+        self, code: str = "", date_yyyymmdd: str = "", pagination_key: str = ""
+    ) -> str:
         """
         get fins statements raw API return
 
         Args:
             code: 銘柄コード
             date_yyyymmdd: 日付(YYYYMMDD or YYYY-MM-DD)
+            pagination_key: ページングキー
 
         Returns:
             str: fins statements
         """
         url = f"{self.JQUANTS_API_BASE}/fins/statements"
         params = {
             "code": code,
             "date": date_yyyymmdd,
         }
+        if pagination_key != "":
+            params["pagination_key"] = pagination_key
         ret = self._get(url, params)
         ret.encoding = self.RAW_ENCODING
 
         return ret.text
 
     def get_fins_statements(
         self, code: str = "", date_yyyymmdd: str = ""
@@ -1071,15 +1193,24 @@
             date_yyyymmdd: 日付(YYYYMMDD or YYYY-MM-DD)
 
         Returns:
             pd.DataFrame: 財務情報 (DisclosedDate, DisclosedTime, 及びLocalCode列でソートされています)
         """
         j = self._get_fins_statements_raw(code=code, date_yyyymmdd=date_yyyymmdd)
         d = json.loads(j)
-        df = pd.DataFrame.from_dict(d["statements"])
+        data = d["statements"]
+        while "pagination_key" in d:
+            j = self._get_fins_statements_raw(
+                code=code,
+                date_yyyymmdd=date_yyyymmdd,
+                pagination_key=d["pagination_key"],
+            )
+            d = json.loads(j)
+            data += d["statements"]
+        df = pd.DataFrame.from_dict(data)
         cols = constants.FINS_STATEMENTS_COLUMNS
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
         df["DisclosedDate"] = pd.to_datetime(df["DisclosedDate"], format="%Y-%m-%d")
         df["CurrentPeriodStartDate"] = pd.to_datetime(
             df["CurrentPeriodStartDate"], format="%Y-%m-%d"
         )
@@ -1179,39 +1310,43 @@
 
     def _get_fins_dividend_raw(
         self,
         code: str = "",
         from_yyyymmdd: str = "",
         to_yyyymmdd: str = "",
         date_yyyymmdd: str = "",
+        pagination_key: str = "",
     ) -> str:
         """
         get  information on dividends (determined and forecast) per share of listed companies etc.. raw API returns
 
         Args:
             code: issue code (e.g. 27800 or 2780)
                 If a 4-digit issue code is specified, only the data of common stock will be obtained
                 for the issue on which both common and preferred stocks are listed.
             from_yyyymmdd: starting point of data period (e.g. 20210901 or 2021-09-01)
             to_yyyymmdd: end point of data period (e.g. 20210907 or 2021-09-07)
             date_yyyymmdd: date of data (e.g. 20210907 or 2021-09-07)
+            pagination_key: ページングキー
         Returns:
             str: information on dividends data
         """
         url = f"{self.JQUANTS_API_BASE}/fins/dividend"
         params = {
             "code": code,
         }
         if date_yyyymmdd != "":
             params["date"] = date_yyyymmdd
         else:
             if from_yyyymmdd != "":
                 params["from"] = from_yyyymmdd
             if to_yyyymmdd != "":
                 params["to"] = to_yyyymmdd
+        if pagination_key != "":
+            params["pagination_key"] = pagination_key
         ret = self._get(url, params)
         ret.encoding = self.RAW_ENCODING
         return ret.text
 
     def get_fins_dividend(
         self,
         code: str = "",
@@ -1235,15 +1370,26 @@
         j = self._get_fins_dividend_raw(
             code=code,
             from_yyyymmdd=from_yyyymmdd,
             to_yyyymmdd=to_yyyymmdd,
             date_yyyymmdd=date_yyyymmdd,
         )
         d = json.loads(j)
-        df = pd.DataFrame.from_dict(d["dividend"])
+        data = d["dividend"]
+        while "pagination_key" in d:
+            j = self._get_fins_dividend_raw(
+                code=code,
+                from_yyyymmdd=from_yyyymmdd,
+                to_yyyymmdd=to_yyyymmdd,
+                date_yyyymmdd=date_yyyymmdd,
+                pagination_key=d["pagination_key"],
+            )
+            d = json.loads(j)
+            data += d["dividend"]
+        df = pd.DataFrame.from_dict(data)
         cols = constants.FINS_DIVIDEND_COLUMNS
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
         df["AnnouncementDate"] = pd.to_datetime(
             df["AnnouncementDate"], format="%Y-%m-%d"
         )
         df.sort_values(["Code"], inplace=True)
@@ -1278,26 +1424,32 @@
             for future in as_completed(futures):
                 df = future.result()
                 buff.append(df)
         return pd.concat(buff).sort_values(
             ["AnnouncementDate", "AnnouncementTime", "Code"]
         )
 
-    def _get_fins_announcement_raw(self) -> str:
+    def _get_fins_announcement_raw(
+        self,
+        pagination_key: str = "",
+    ) -> str:
         """
         get fin announcement raw API returns
 
         Args:
-            N/A
+            pagination_key: ページングキー
 
         Returns:
             str: Schedule of financial announcement
         """
         url = f"{self.JQUANTS_API_BASE}/fins/announcement"
-        ret = self._get(url)
+        params = {}
+        if pagination_key != "":
+            params["pagination_key"] = pagination_key
+        ret = self._get(url, params)
         ret.encoding = self.RAW_ENCODING
         return ret.text
 
     def get_fins_announcement(self) -> pd.DataFrame:
         """
         get fin announcement
 
@@ -1305,39 +1457,48 @@
             N/A
 
         Returns:
             pd.DataFrame: Schedule of financial announcement
         """
         j = self._get_fins_announcement_raw()
         d = json.loads(j)
-        df = pd.DataFrame.from_dict(d["announcement"])
+        data = d["announcement"]
+        while "pagination_key" in d:
+            j = self._get_fins_announcement_raw(pagination_key=d["pagination_key"])
+            d = json.loads(j)
+            data += d["announcement"]
+        df = pd.DataFrame.from_dict(data)
         cols = constants.FINS_ANNOUNCEMENT_COLUMNS
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
         df["Date"] = pd.to_datetime(df["Date"], format="%Y-%m-%d")
         df.sort_values(["Date", "Code"], inplace=True)
         return df[cols]
 
     # /option
     def _get_option_index_option_raw(
         self,
         date_yyyymmdd,
+        pagination_key: str = "",
     ) -> str:
         """
         get information on the OHLC etc. of Nikkei 225 raw API returns
 
         Args:
             date_yyyymmdd: date of data (e.g. 20210907 or 2021-09-07)
+            pagination_key: ページングキー
         Returns:
             str: Nikkei 225 Options' OHLC etc.
         """
         url = f"{self.JQUANTS_API_BASE}/option/index_option"
         params = {
             "date": date_yyyymmdd,
         }
+        if pagination_key != "":
+            params["pagination_key"] = pagination_key
         ret = self._get(url, params)
         ret.encoding = self.RAW_ENCODING
         return ret.text
 
     def get_option_index_option(
         self,
         date_yyyymmdd,
@@ -1351,15 +1512,23 @@
             pd.DataFrame:
                 Nikkei 225 Options' OHLC etc. (Sorted by "Code")
         """
         j = self._get_option_index_option_raw(
             date_yyyymmdd=date_yyyymmdd,
         )
         d = json.loads(j)
-        df = pd.DataFrame.from_dict(d["index_option"])
+        data = d["index_option"]
+        while "pagination_key" in d:
+            j = self._get_option_index_option_raw(
+                date_yyyymmdd=date_yyyymmdd,
+                pagination_key=d["pagination_key"],
+            )
+            d = json.loads(j)
+            data += d["index_option"]
+        df = pd.DataFrame.from_dict(data)
         cols = constants.OPTION_INDEX_OPTION_COLUMNS
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
         df["Date"] = pd.to_datetime(df["Date"], format="%Y-%m-%d")
         df.sort_values(["Code"], inplace=True)
         return df[cols]
```

### Comparing `jquants_api_client-1.1.1/jquantsapi/constants.py` & `jquants_api_client-1.1.2/jquantsapi/constants.py`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.1.1/jquantsapi/enums.py` & `jquants_api_client-1.1.2/jquantsapi/enums.py`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.1.1/pyproject.toml` & `jquants_api_client-1.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jquants-api-client"
-version = "1.1.1" # use poetry-dynamic-versioning
+version = "1.1.2" # use poetry-dynamic-versioning
 authors = [
     "J-Quants Project Contributors <j-quants@jpx.co.jp>",
 ]
 description = "J-Quants API Client Library"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
```

### Comparing `jquants_api_client-1.1.1/PKG-INFO` & `jquants_api_client-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jquants-api-client
-Version: 1.1.1
+Version: 1.1.2
 Summary: J-Quants API Client Library
 Home-page: https://github.com/J-Quants/jquants-api-client-python
 License: Apache-2.0
 Keywords: jquants,api,client,J-Quants
 Author: J-Quants Project Contributors
 Author-email: j-quants@jpx.co.jp
 Requires-Python: >=3.7.1,<4.0.0
```


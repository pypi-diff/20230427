# Comparing `tmp/finlogic-0.3.8.tar.gz` & `tmp/finlogic-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.3.8.tar", last modified: Sun Apr 23 12:24:42 2023, max compression
+gzip compressed data, was "finlogic-0.3.9.tar", last modified: Mon Apr 24 16:26:03 2023, max compression
```

## Comparing `finlogic-0.3.8.tar` & `finlogic-0.3.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.3.8/LICENSE
--rw-r--r--   0        0        0    10060 2023-04-22 03:12:14.634867 finlogic-0.3.8/README.md
--rw-r--r--   0        0        0      423 2023-04-22 17:40:14.252933 finlogic-0.3.8/finlogic/__init__.py
--rw-r--r--   0        0        0    22078 2023-04-22 03:12:14.634867 finlogic-0.3.8/finlogic/company.py
--rw-r--r--   0        0        0     1024 2023-04-22 03:12:14.634867 finlogic-0.3.8/finlogic/config.py
--rw-r--r--   0        0        0     9283 2023-04-22 03:12:14.634867 finlogic-0.3.8/finlogic/cvm.py
--rw-r--r--   0        0        0     6806 2023-04-22 03:12:14.634867 finlogic-0.3.8/finlogic/database.py
--rw-r--r--   0        0        0      989 2023-04-23 12:24:42.046992 finlogic-0.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.3.8/tests/__init__.py
--rw-r--r--   0        0        0     2125 2023-04-14 09:12:15.664615 finlogic-0.3.8/tests/test_company.py
--rw-r--r--   0        0        0      598 2023-04-22 03:12:14.635867 finlogic-0.3.8/tests/test_database.py
--rw-r--r--   0        0        0    12080 1970-01-01 00:00:00.000000 finlogic-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.3.9/LICENSE
+-rw-r--r--   0        0        0    10060 2023-04-22 03:12:14.634867 finlogic-0.3.9/README.md
+-rw-r--r--   0        0        0      423 2023-04-24 16:25:02.799288 finlogic-0.3.9/finlogic/__init__.py
+-rw-r--r--   0        0        0    22892 2023-04-24 07:38:21.875678 finlogic-0.3.9/finlogic/company.py
+-rw-r--r--   0        0        0     1024 2023-04-22 03:12:14.634867 finlogic-0.3.9/finlogic/config.py
+-rw-r--r--   0        0        0     9283 2023-04-22 03:12:14.634867 finlogic-0.3.9/finlogic/cvm.py
+-rw-r--r--   0        0        0     6806 2023-04-22 03:12:14.634867 finlogic-0.3.9/finlogic/database.py
+-rw-r--r--   0        0        0      989 2023-04-24 16:26:03.864074 finlogic-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.3.9/tests/__init__.py
+-rw-r--r--   0        0        0     2125 2023-04-14 09:12:15.664615 finlogic-0.3.9/tests/test_company.py
+-rw-r--r--   0        0        0      598 2023-04-22 03:12:14.635867 finlogic-0.3.9/tests/test_database.py
+-rw-r--r--   0        0        0    12080 1970-01-01 00:00:00.000000 finlogic-0.3.9/PKG-INFO
```

### Comparing `finlogic-0.3.8/LICENSE` & `finlogic-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.3.8/README.md` & `finlogic-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `finlogic-0.3.8/finlogic/company.py` & `finlogic-0.3.9/finlogic/company.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,19 +37,23 @@
         identifier: int | str,
         acc_method: Literal["consolidated", "separate"] = "consolidated",
         acc_unit: int | float | str = 1,
         tax_rate: float = 0.34,
         language: str = "english",
     ):
         """Initializes a new instance of the Company class."""
+        self._initialized = False
         self.identifier = identifier
         self.acc_method = acc_method
         self.acc_unit = acc_unit
         self.tax_rate = tax_rate
         self.language = language
+        self._initialized = True
+        # Only set company dataframe after identifier, acc_method and acc_unit are set
+        self._set_co_df()
 
     @property
     def identifier(self) -> int | str:
         """Set a unique identifier to select the company in FinLogic Database.
 
         This method sets the company's CVM and fiscal ID based on a given
         identifier. The identifier can be either the CVM ID or the Fiscal ID
@@ -84,17 +88,18 @@
                 df["co_id"] == identifier, "co_fiscal_id"
             ].item()
         elif identifier in df["co_fiscal_id"].values:
             self._co_fiscal_id = identifier
             self._co_id = df.loc[df["co_fiscal_id"] == identifier, "co_id"].item()
         else:
             raise KeyError("Company 'identifier' not found in FinLogic Database")
-        # Only set company data after object identifier validation
-        self._set_co_df()
         self._identifier = identifier
+        # If object was already initialized, reset company dataframe
+        if self._initialized:
+            self._set_co_df()
 
     @property
     def acc_method(self) -> Literal["consolidated", "separate"]:
         """Gets or sets the accounting method for registering investments in
         subsidiaries.
 
         The "acc_method" must be "consolidated" or "separate". Consolidated
@@ -109,14 +114,17 @@
 
     @acc_method.setter
     def acc_method(self, value: Literal["consolidated", "separate"]):
         if value in {"consolidated", "separate"}:
             self._acc_method = value
         else:
             raise ValueError("acc_method expects 'consolidated' or 'separate'")
+        # If object was already initialized, reset company dataframe
+        if self._initialized:
+            self._set_co_df()
 
     @property
     def acc_unit(self) -> float:
         """Gets or sets the accounting unit for the financial statements.
 
         The "acc_unit" is a constant that will divide all company
         accounting values. The constant must be a number greater than
@@ -152,14 +160,18 @@
             case str():  # Add this case to catch invalid strings
                 raise ValueError("Invalid string for Accounting Unit")
             case v if v > 0:
                 self._acc_unit = v
             case _:
                 raise ValueError("Accounting Unit is invalid")
 
+        # If object was already initialized, reset company dataframe
+        if self._initialized:
+            self._set_co_df()
+
     @property
     def tax_rate(self) -> float:
         """Gets or sets company 'tax_rate' property.
 
         The "tax_rate" is used to calculate some of the company
         indicators, such as EBIT and net income. The default value
         is 0.34, which is the standard corporate tax rate in Brazil.
@@ -211,47 +223,65 @@
         if language.lower() in list_languages:
             self._language = language.capitalize()
         else:
             sup_lang = f"Supported languages: {', '.join(list_languages)}"
             raise KeyError(f"'{language}' not supported. {sup_lang}")
 
     def _set_co_df(self) -> pd.DataFrame:
-        self._co_df = (
-            c.finlogic_df.query("co_id == @self._co_id")
+        """Sets the company data frame.
+
+        This method creates a data frame with the company's financial
+        statements.
+        """
+        # Create custom data frame for company selection
+        expr = "co_id == @self._co_id and acc_method == @self._acc_method"
+        co_df = (
+            c.finlogic_df.query(expr)
             .astype(
                 {
                     "co_name": str,
                     "co_id": "UInt32",
                     "co_fiscal_id": str,
                     "report_type": str,
-                    "report_version": str,
+                    "report_version": "UInt8",
                     "period_reference": "datetime64[ns]",
                     "period_begin": "datetime64[ns]",
                     "period_end": "datetime64[ns]",
                     "period_order": str,
                     "acc_code": str,
                     "acc_name": str,
                     "acc_method": str,
                     "acc_fixed": bool,
                     "acc_value": float,
                     "equity_statement_column": str,
                 }
             )
             .sort_values(by="acc_code", ignore_index=True)
         )
-        self._name = self._co_df["co_name"].iloc[0]
-        self._first_annual = self._co_df.query('report_type == "annual"')[
-            "period_end"
-        ].min()
-        self._last_annual = self._co_df.query('report_type == "annual"')[
-            "period_end"
-        ].max()
-        self._last_quarterly = self._co_df.query('report_type == "quarterly"')[
-            "period_end"
-        ].max()
+
+        # Change acc_unit only for accounts different from 3.99
+        co_df["acc_value"] = np.where(
+            co_df["acc_code"].str.startswith("3.99"),
+            co_df["acc_value"],
+            co_df["acc_value"] / self._acc_unit,
+        )
+
+        self._name = co_df["co_name"].iloc[0]
+        expr = 'report_type == "annual"'
+        self._first_annual = co_df.query(expr)["period_end"].min()
+        self._last_annual = co_df.query(expr)["period_end"].max()
+        expr = 'report_type == "quarterly"'
+        self._last_quarterly = co_df.query(expr)["period_end"].max()
+
+        # Drop columns that are already company properties
+        co_df.drop(
+            columns=["co_name", "co_id", "co_fiscal_id", "acc_method"], inplace=True
+        )
+        # Set company data frame
+        self._co_df = co_df
 
     def info(self) -> dict:
         """Return a dictionay with company info."""
         company_info = {
             "Name": self._name,
             "CVM ID": self._co_id,
             "Fiscal ID (CNPJ)": self._co_fiscal_id,
@@ -261,14 +291,52 @@
             "Selected Accounting Unit": self._acc_unit,
             "First Annual Report": self._first_annual.strftime("%Y-%m-%d"),
             "Last Annual Report": self._last_annual.strftime("%Y-%m-%d"),
             "Last Quarterly Report": self._last_quarterly.strftime("%Y-%m-%d"),
         }
         return company_info
 
+    def _build_report(self, dfi: pd.DataFrame) -> pd.DataFrame:
+        # keep only last quarterly fs
+        if self._last_annual > self._last_quarterly:
+            df = dfi.query('report_type == "annual"').copy()
+            df.query(
+                "period_order == 'PREVIOUS' or \
+                 period_end == @self._last_annual",
+                inplace=True,
+            )
+        else:
+            df = dfi.query(
+                'report_type == "annual" or \
+                 period_end == @self._last_quarterly'
+            ).copy()
+            df.query(
+                "period_order == 'PREVIOUS' or \
+                 period_end == @self._last_quarterly or \
+                 period_end == @self._last_annual",
+                inplace=True,
+            )
+
+        # Create output dataframe with only the index
+        dfo = df.sort_values(by="period_end", ascending=True)[
+            ["acc_name", "acc_code", "acc_fixed"]
+        ].drop_duplicates(subset="acc_code", ignore_index=True, keep="last")
+
+        periods = list(df["period_end"].sort_values().unique())
+        for period in periods:
+            year_cols = ["acc_value", "acc_code"]
+            df_year = df.query("period_end == @period")[year_cols].copy()
+            period_str = period.strftime("%Y-%m-%d")
+            if period == self._last_quarterly:
+                period_str += " (ttm)"
+            df_year.rename(columns={"acc_value": period_str}, inplace=True)
+            dfo = pd.merge(dfo, df_year, how="left", on=["acc_code"])
+
+        return dfo.sort_values("acc_code", ignore_index=True)
+
     def report(
         self,
         report_type: str,
         acc_level: int | None = None,
         num_years: int = 0,
     ) -> pd.DataFrame:
         """Generate an accounting report for the company.
@@ -299,36 +367,28 @@
         Raises:
             ValueError: If some argument is invalid.
         """
         # Check input arguments.
         if acc_level not in {None, 2, 3, 4}:
             raise ValueError("acc_level expects None, 2, 3 or 4")
 
-        df = self._co_df.query("acc_method == @self._acc_method").copy()
+        df = self._co_df.copy()
 
         # Set language
         class MyDict(dict):
             """Custom dictionary class to return key if key is not found."""
 
             def __missing__(self, key):
                 return "(pt) " + key
 
         if self._language == "English":
             _pten_dict = dict(c.language_df.values)
             _pten_dict = MyDict(_pten_dict)
             df["acc_name"] = df["acc_name"].map(_pten_dict)
-        else:
-            pass
 
-        # Change acc_unit only for accounts different from 3.99
-        df["acc_value"] = np.where(
-            df["acc_code"].str.startswith("3.99"),
-            df["acc_value"],
-            df["acc_value"] / self._acc_unit,
-        )
         # Filter dataframe for selected acc_level
         if acc_level:
             acc_code_limit = acc_level * 3 - 2  # noqa
             df.query("acc_code.str.len() <= @acc_code_limit", inplace=True)
         """
         Filter dataframe for selected report_type (report type)
         df['acc_code'].str[0].unique() -> [1, 2, 3, 4, 5, 6, 7]
@@ -357,31 +417,31 @@
             "earnings_per_share": ["3.99"],
             "comprehensive_income": ["4"],
             "changes_in_equity": ["5"],
             "cash_flow": ["6"],
             "added_value": ["7"],
         }
         acc_codes = report_types[report_type]
-        expression = ""
+        expr = ""
         for count, acc_code in enumerate(acc_codes):
             if count > 0:
-                expression += " or "
-            expression += f'acc_code.str.startswith("{acc_code}")'
-        df.query(expression, inplace=True)
+                expr += " or "
+            expr += f'acc_code.str.startswith("{acc_code}")'
+        df.query(expr, inplace=True)
 
         # remove earnings per share from income statment
         if report_type == "income":
             df = df[~df["acc_code"].str.startswith("3.99")]
 
         if report_type in {"income", "cash_flow"}:
             df = self._calculate_ttm(df)
 
         df.reset_index(drop=True, inplace=True)
 
-        report_df = self._make_report(df)
+        report_df = self._build_report(df)
         report_df.set_index(keys="acc_code", drop=True, inplace=True)
         # Show only selected years
         if num_years > 0:
             cols = report_df.columns.to_list()
             cols = cols[0:2] + cols[-num_years:]
             report_df = report_df[cols]
         return report_df
@@ -529,45 +589,7 @@
         dfo.loc["net_margin"] = net_income / revenues
 
         dfo.index.name = "Company Financial Indicators"
         # Show only the selected number of years
         if num_years > 0:
             dfo = dfo[dfo.columns[-num_years:]]
         return dfo
-
-    def _make_report(self, dfi: pd.DataFrame) -> pd.DataFrame:
-        # keep only last quarterly fs
-        if self._last_annual > self._last_quarterly:
-            df = dfi.query('report_type == "annual"').copy()
-            df.query(
-                "period_order == 'PREVIOUS' or \
-                 period_end == @self._last_annual",
-                inplace=True,
-            )
-        else:
-            df = dfi.query(
-                'report_type == "annual" or \
-                 period_end == @self._last_quarterly'
-            ).copy()
-            df.query(
-                "period_order == 'PREVIOUS' or \
-                 period_end == @self._last_quarterly or \
-                 period_end == @self._last_annual",
-                inplace=True,
-            )
-
-        # Create output dataframe with only the index
-        dfo = df.sort_values(by="period_end", ascending=True)[
-            ["acc_name", "acc_code", "acc_fixed"]
-        ].drop_duplicates(subset="acc_code", ignore_index=True, keep="last")
-
-        periods = list(df["period_end"].sort_values().unique())
-        for period in periods:
-            year_cols = ["acc_value", "acc_code"]
-            df_year = df.query("period_end == @period")[year_cols].copy()
-            period_str = period.strftime("%Y-%m-%d")
-            if period == self._last_quarterly:
-                period_str += " (ttm)"
-            df_year.rename(columns={"acc_value": period_str}, inplace=True)
-            dfo = pd.merge(dfo, df_year, how="left", on=["acc_code"])
-
-        return dfo.sort_values("acc_code", ignore_index=True)
```

### Comparing `finlogic-0.3.8/finlogic/config.py` & `finlogic-0.3.9/finlogic/config.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.3.8/finlogic/cvm.py` & `finlogic-0.3.9/finlogic/cvm.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.3.8/finlogic/database.py` & `finlogic-0.3.9/finlogic/database.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.3.8/pyproject.toml` & `finlogic-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pandas>=1.4.0",
     "requests>=2.27.0",
     "zstandard>=0.17.0",
 ]
-version = "0.3.8"
+version = "0.3.9"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.0.0",
```

### Comparing `finlogic-0.3.8/tests/test_company.py` & `finlogic-0.3.9/tests/test_company.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.3.8/tests/test_database.py` & `finlogic-0.3.9/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.3.8/PKG-INFO` & `finlogic-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finlogic
-Version: 0.3.8
+Version: 0.3.9
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finlogic Version: 0.3.8 Summary: Finance toolkit
+Metadata-Version: 2.1 Name: finlogic Version: 0.3.9 Summary: Finance toolkit
 for listed Brazilian companies Keywords: pandas, cvm, finance, investment,
 accounting Author-Email: Carlos Carvalho
 cj@outlook.com> License: MIT License Copyright (c) 2022 Carlos Carvalho
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```


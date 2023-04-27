# Comparing `tmp/sports-betting-0.4.0.tar.gz` & `tmp/sports-betting-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports-betting-0.4.0.tar", last modified: Tue Apr 25 11:31:34 2023, max compression
+gzip compressed data, was "sports-betting-0.5.0.tar", last modified: Thu Apr 27 17:17:44 2023, max compression
```

## Comparing `sports-betting-0.4.0.tar` & `sports-betting-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1072 2023-04-12 10:43:30.277668 sports-betting-0.4.0/LICENSE
--rw-r--r--   0        0        0     9397 2023-04-24 09:43:10.763453 sports-betting-0.4.0/README.md
--rw-r--r--   0        0        0     5438 2023-04-24 21:31:06.056541 sports-betting-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1026 2023-04-24 09:43:10.783945 sports-betting-0.4.0/src/sportsbet/__init__.py
--rw-r--r--   0        0        0      131 2023-04-19 07:06:57.452684 sports-betting-0.4.0/src/sportsbet/__main__.py
--rw-r--r--   0        0        0      124 2023-04-24 09:43:10.712522 sports-betting-0.4.0/src/sportsbet/cli/__init__.py
--rw-r--r--   0        0        0      466 2023-04-24 09:43:10.713830 sports-betting-0.4.0/src/sportsbet/cli/_cli.py
--rw-r--r--   0        0        0     3905 2023-04-24 09:43:10.715546 sports-betting-0.4.0/src/sportsbet/cli/_datasets.py
--rw-r--r--   0        0        0     3328 2023-04-24 09:43:10.716418 sports-betting-0.4.0/src/sportsbet/cli/_evaluation.py
--rw-r--r--   0        0        0      874 2023-04-24 09:43:10.717061 sports-betting-0.4.0/src/sportsbet/cli/_options.py
--rw-r--r--   0        0        0     4912 2023-04-24 09:43:10.717626 sports-betting-0.4.0/src/sportsbet/cli/_utils.py
--rw-r--r--   0        0        0      320 2023-04-24 09:43:10.784738 sports-betting-0.4.0/src/sportsbet/datasets/__init__.py
--rw-r--r--   0        0        0    18296 2023-04-24 09:43:10.786065 sports-betting-0.4.0/src/sportsbet/datasets/_base.py
--rw-r--r--   0        0        0    15883 2023-04-24 09:43:10.787051 sports-betting-0.4.0/src/sportsbet/datasets/_dummy.py
--rw-r--r--   0        0        0        0 2023-04-11 16:17:21.696007 sports-betting-0.4.0/src/sportsbet/datasets/_soccer/__init__.py
--rw-r--r--   0        0        0    21957 2023-04-24 09:43:10.788101 sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_data.py
--rw-r--r--   0        0        0    28799 2023-04-24 09:43:10.735625 sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_fd.py
--rw-r--r--   0        0        0     5122 2023-04-03 15:00:25.776337 sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_fte.py
--rw-r--r--   0        0        0     2595 2023-03-27 20:39:08.417256 sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_utils.py
--rw-r--r--   0        0        0      326 2023-04-24 09:43:10.695223 sports-betting-0.4.0/src/sportsbet/evaluation/__init__.py
--rw-r--r--   0        0        0    11881 2023-04-24 09:43:10.696860 sports-betting-0.4.0/src/sportsbet/evaluation/_base.py
--rw-r--r--   0        0        0     6783 2023-04-24 09:43:10.697929 sports-betting-0.4.0/src/sportsbet/evaluation/_classifier.py
--rw-r--r--   0        0        0     7919 2023-04-24 09:43:10.699163 sports-betting-0.4.0/src/sportsbet/evaluation/_rules.py
--rw-r--r--   0        0        0        0 2023-04-12 10:43:30.443650 sports-betting-0.4.0/src/sportsbet/py.typed
--rw-r--r--   0        0        0      162 2023-04-12 10:43:30.222813 sports-betting-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0       20 2023-04-24 09:43:10.718388 sports-betting-0.4.0/tests/cli/__init__.py
--rw-r--r--   0        0        0      270 2023-04-24 09:43:10.719615 sports-betting-0.4.0/tests/cli/configs/bettor.py
--rw-r--r--   0        0        0      316 2023-04-24 09:43:10.720456 sports-betting-0.4.0/tests/cli/configs/dataloader.py
--rw-r--r--   0        0        0     2919 2023-04-24 09:43:10.721300 sports-betting-0.4.0/tests/cli/test_datasets.py
--rw-r--r--   0        0        0     2050 2023-04-24 09:43:10.721779 sports-betting-0.4.0/tests/cli/test_evaluation.py
--rw-r--r--   0        0        0      482 2023-04-24 09:43:10.722335 sports-betting-0.4.0/tests/cli/test_main.py
--rw-r--r--   0        0        0      310 2023-04-12 10:43:30.475416 sports-betting-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0       28 2023-03-24 22:39:56.568853 sports-betting-0.4.0/tests/datasets/__init__.py
--rw-r--r--   0        0        0    18705 2023-03-28 15:26:00.605472 sports-betting-0.4.0/tests/datasets/test_dummy.py
--rw-r--r--   0        0        0       30 2023-03-24 22:40:31.109809 sports-betting-0.4.0/tests/evaluation/__init__.py
--rw-r--r--   0        0        0     7350 2023-04-02 15:06:18.413287 sports-betting-0.4.0/tests/evaluation/test_classifier.py
--rw-r--r--   0        0        0     2897 2023-04-24 09:22:43.246577 sports-betting-0.4.0/tests/evaluation/test_rules.py
--rw-r--r--   0        0        0    10739 1970-01-01 00:00:00.000000 sports-betting-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-25 16:59:22.976380 sports-betting-0.5.0/LICENSE
+-rw-r--r--   0        0        0     9397 2023-04-25 17:00:49.972566 sports-betting-0.5.0/README.md
+-rw-r--r--   0        0        0     5464 2023-04-27 17:17:40.274284 sports-betting-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1026 2023-04-25 17:00:49.977235 sports-betting-0.5.0/src/sportsbet/__init__.py
+-rw-r--r--   0        0        0      131 2023-04-25 16:59:22.992255 sports-betting-0.5.0/src/sportsbet/__main__.py
+-rw-r--r--   0        0        0      124 2023-04-25 17:00:49.977635 sports-betting-0.5.0/src/sportsbet/cli/__init__.py
+-rw-r--r--   0        0        0      466 2023-04-25 17:00:49.977881 sports-betting-0.5.0/src/sportsbet/cli/_cli.py
+-rw-r--r--   0        0        0     3905 2023-04-25 17:00:49.978201 sports-betting-0.5.0/src/sportsbet/cli/_datasets.py
+-rw-r--r--   0        0        0     3328 2023-04-25 17:00:49.978506 sports-betting-0.5.0/src/sportsbet/cli/_evaluation.py
+-rw-r--r--   0        0        0      874 2023-04-25 17:00:49.978798 sports-betting-0.5.0/src/sportsbet/cli/_options.py
+-rw-r--r--   0        0        0     4912 2023-04-25 17:00:49.979119 sports-betting-0.5.0/src/sportsbet/cli/_utils.py
+-rw-r--r--   0        0        0      320 2023-04-25 19:18:34.131135 sports-betting-0.5.0/src/sportsbet/datasets/__init__.py
+-rw-r--r--   0        0        0    18296 2023-04-25 17:00:49.980378 sports-betting-0.5.0/src/sportsbet/datasets/_base.py
+-rw-r--r--   0        0        0    15883 2023-04-25 17:00:49.981171 sports-betting-0.5.0/src/sportsbet/datasets/_dummy.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:59:22.999739 sports-betting-0.5.0/src/sportsbet/datasets/_soccer/__init__.py
+-rw-r--r--   0        0        0    21957 2023-04-25 17:00:49.981862 sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_data.py
+-rw-r--r--   0        0        0    29307 2023-04-27 17:17:40.275507 sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_fd.py
+-rw-r--r--   0        0        0     5122 2023-04-26 13:27:31.161262 sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_fte.py
+-rw-r--r--   0        0        0     3802 2023-04-27 17:17:40.277950 sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_utils.py
+-rw-r--r--   0        0        0      326 2023-04-25 17:00:49.984179 sports-betting-0.5.0/src/sportsbet/evaluation/__init__.py
+-rw-r--r--   0        0        0    11881 2023-04-25 17:00:49.984882 sports-betting-0.5.0/src/sportsbet/evaluation/_base.py
+-rw-r--r--   0        0        0     6783 2023-04-25 17:00:49.985439 sports-betting-0.5.0/src/sportsbet/evaluation/_classifier.py
+-rw-r--r--   0        0        0     7919 2023-04-25 17:00:49.985811 sports-betting-0.5.0/src/sportsbet/evaluation/_rules.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:59:23.004536 sports-betting-0.5.0/src/sportsbet/py.typed
+-rw-r--r--   0        0        0      162 2023-04-25 16:59:23.004826 sports-betting-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0       20 2023-04-25 17:00:49.986811 sports-betting-0.5.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-25 17:00:49.987208 sports-betting-0.5.0/tests/cli/configs/bettor.py
+-rw-r--r--   0        0        0      316 2023-04-25 17:00:49.987619 sports-betting-0.5.0/tests/cli/configs/dataloader.py
+-rw-r--r--   0        0        0     2919 2023-04-25 17:00:49.988270 sports-betting-0.5.0/tests/cli/test_datasets.py
+-rw-r--r--   0        0        0     2050 2023-04-25 17:00:49.988782 sports-betting-0.5.0/tests/cli/test_evaluation.py
+-rw-r--r--   0        0        0      482 2023-04-25 17:00:49.989200 sports-betting-0.5.0/tests/cli/test_main.py
+-rw-r--r--   0        0        0      310 2023-04-25 16:59:23.005092 sports-betting-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0       28 2023-04-25 16:59:23.005357 sports-betting-0.5.0/tests/datasets/__init__.py
+-rw-r--r--   0        0        0    18705 2023-04-25 17:00:49.989963 sports-betting-0.5.0/tests/datasets/test_dummy.py
+-rw-r--r--   0        0        0       30 2023-04-25 16:59:23.006158 sports-betting-0.5.0/tests/evaluation/__init__.py
+-rw-r--r--   0        0        0     7350 2023-04-25 16:59:23.006482 sports-betting-0.5.0/tests/evaluation/test_classifier.py
+-rw-r--r--   0        0        0     2897 2023-04-25 17:00:49.990754 sports-betting-0.5.0/tests/evaluation/test_rules.py
+-rw-r--r--   0        0        0    10743 1970-01-01 00:00:00.000000 sports-betting-0.5.0/PKG-INFO
```

### Comparing `sports-betting-0.4.0/LICENSE` & `sports-betting-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/README.md` & `sports-betting-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/pyproject.toml` & `sports-betting-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -39,23 +39,24 @@
     "cloudpickle>=2.0.0",
     "beautifulsoup4>=4.0.0",
     "vectorbt>=0.24.5",
     "QuantStats>=0.0.47",
     "typing-extensions>=4.5.0",
     "click>=8.1.3",
     "rich>=13.3.3",
+    "aiohttp>=3.8.4",
 ]
-version = "0.4.0"
+version = "0.5.0"
 
 [project.urls]
 Homepage = "https://georgedouzas.github.io/sports-betting"
 Documentation = "https://georgedouzas.github.io/sports-betting"
 Changelog = "https://georgedouzas.github.io/sports-betting/changelog"
 Repository = "https://github.com/georgedouzas/sports-betting"
-Issues = "https://github/georgedouzas/sports-betting/issues"
+Issues = "https://github.com/georgedouzas/sports-betting/issues"
 Discussions = "https://github.com/georgedouzas/sports-betting/discussions"
 Gitter = "https://gitter.im/sports-betting/community"
 Funding = "https://github.com/sponsors/georgedouzas"
 
 [project.scripts]
 sportsbet = "sportsbet.cli:main"
```

### Comparing `sports-betting-0.4.0/src/sportsbet/__init__.py` & `sports-betting-0.5.0/src/sportsbet/__init__.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/src/sportsbet/cli/_datasets.py` & `sports-betting-0.5.0/src/sportsbet/cli/_datasets.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/src/sportsbet/cli/_evaluation.py` & `sports-betting-0.5.0/src/sportsbet/cli/_evaluation.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/src/sportsbet/cli/_options.py` & `sports-betting-0.5.0/src/sportsbet/cli/_options.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/src/sportsbet/cli/_utils.py` & `sports-betting-0.5.0/src/sportsbet/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/src/sportsbet/datasets/_base.py` & `sports-betting-0.5.0/src/sportsbet/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/src/sportsbet/datasets/_dummy.py` & `sports-betting-0.5.0/src/sportsbet/datasets/_dummy.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_data.py` & `sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_data.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_fd.py` & `sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_fd.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,24 @@
 # Author: Georgios Douzas <gdouzas@icloud.com>
 # License: MIT
 
 from __future__ import annotations
 
 from datetime import datetime
 from functools import lru_cache
-from urllib.request import urlopen
 
 import numpy as np
 import pandas as pd
 from bs4 import BeautifulSoup
-from rich.progress import track
 from sklearn.model_selection import ParameterGrid
 from typing_extensions import Self
 
 from ... import Param
 from .._base import _BaseDataLoader
-from ._utils import OUTPUTS, _read_csv
+from ._utils import OUTPUTS, _read_csv, _read_csvs, _read_urls_content
 
 URL = 'https://www.football-data.co.uk'
 BASE_URLS = [
     'englandm.php',
     'scotlandm.php',
     'germanym.php',
     'italym.php',
@@ -273,18 +271,24 @@
 def _convert_base_url_to_league(base_url: str) -> str:
     league = base_url.replace('.php', '')
     if base_url[0].islower():
         league = league[:-1].capitalize()
     return league
 
 
-def _extract_csv_urls(base_url: str) -> set[str]:
-    html = urlopen('/'.join([URL, base_url]))  # noqa: S310
-    bsObj = BeautifulSoup(html.read(), features='html.parser')
-    return {el.get('href') for el in bsObj.find_all('a') if el.get('href').endswith('csv')}
+def _extract_all_urls() -> list[tuple[str, str, tuple[str, ...], set[str]]]:
+    base_urls = ['/'.join([URL, base_url]) for base_url in BASE_URLS]
+    bsObjs = [BeautifulSoup(html, features='html.parser') for html in _read_urls_content(base_urls)]
+    all_urls = []
+    for base_url, bsObj in zip(BASE_URLS, bsObjs):
+        league = _convert_base_url_to_league(base_url)
+        divisions = LEAGUES_MAPPING[league][1:]
+        urls = {el.get('href') for el in bsObj.find_all('a') if el.get('href').endswith('csv')}
+        all_urls.append((base_url, league, divisions, urls))
+    return all_urls
 
 
 def _param_grid_to_csv_urls(param_grid: ParameterGrid) -> list[tuple[Param, str]]:
     urls = []
     for params in param_grid:
         in_main_leagues = f'{params["league"].lower()}m.php' in BASE_URLS
         encoded_league, *divisions = LEAGUES_MAPPING[params['league']]
@@ -483,47 +487,61 @@
         ('target__away_team__bookings_points', float),
     ]
     OUTPUTS = OUTPUTS
 
     @classmethod
     @lru_cache
     def _get_full_param_grid(cls: type[_FDSoccerDataLoader]) -> ParameterGrid:
-        full_param_grid = []
-        for base_url in track(BASE_URLS, description='Downloading parameters data', transient=True):
-            league = _convert_base_url_to_league(base_url)
-            divisions = LEAGUES_MAPPING[league][1:]
-            urls = _extract_csv_urls(base_url)
+        # Get all URLs
+        all_urls = _extract_all_urls()
+
+        urls_main, urls_extra = [], []
+        for base_url, league, divisions, urls in all_urls:
             for url in urls:
+                url_full = '/'.join([URL, url])
                 if base_url[0].islower():
-                    _, year, division = url.split('/')
-                    division = division.replace('.csv', '')[-1]
-                    param_grid = {
-                        'league': [league],
-                        'division': [int(division) + int('0' in divisions) if division != 'C' else 5],
-                        'year': [datetime.strptime(year[2:], '%y').astimezone().year],
-                    }
+                    urls_main.append((league, divisions, url_full))
                 else:
-                    years = _read_csv('/'.join([URL, url]))['Season']
-                    years = list(
-                        {
-                            season + 1 if type(season) is not str else int(season.split('/')[-1])
-                            for season in years.unique()
-                        },
-                    )
-                    param_grid = {'league': [league], 'division': [1], 'year': years}
-                full_param_grid.append(param_grid)
+                    urls_extra.append((league, divisions, url_full))
+
+        # Download CSVs for extra leagues
+        csvs_extra = _read_csvs([url for *_, url in urls_extra])
+
+        full_param_grid = []
+
+        # Extra leagues
+        for (league, *_), csv in zip(urls_extra, csvs_extra):
+            years = csv['Season']
+            years = list(
+                {season + 1 if type(season) is not str else int(season.split('/')[-1]) for season in years.unique()},
+            )
+            param_grid = {'league': [league], 'division': [1], 'year': years}
+            full_param_grid.append(param_grid)
+
+        # Main leagues
+        for league, divisions, url in urls_main:
+            *_, year, division = url.split('/')
+            division = division.replace('.csv', '')[-1]
+            param_grid = {
+                'league': [league],
+                'division': [int(division) + int('0' in divisions) if division != 'C' else 5],
+                'year': [datetime.strptime(year[2:], '%y').astimezone().year],
+            }
+            full_param_grid.append(param_grid)
+
         return ParameterGrid(full_param_grid)
 
     @lru_cache  # noqa: B019
     def _get_data(self: Self) -> pd.DataFrame:
         # Training data
         data_container = []
-        urls = _param_grid_to_csv_urls(self.param_grid_)
-        for params, url in track(urls, description='Downloading training data', transient=True):
-            data = _read_csv(url).replace('^#', np.nan, regex=True)
+        urls_params = _param_grid_to_csv_urls(self.param_grid_)
+        csvs = _read_csvs([url for _, url in urls_params])
+        for (params, url), csv in zip(urls_params, csvs):
+            data = csv.replace('^#', np.nan, regex=True)
             try:
                 data['Date'] = pd.to_datetime(data['Date'], format='%d/%m/%Y')
             except ValueError:
                 data['Date'] = pd.to_datetime(data['Date'], infer_datetime_format=True)
 
             if url.split('/')[-2] != 'new':
                 data = data.assign(
```

### Comparing `sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_fte.py` & `sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_fte.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/src/sportsbet/evaluation/_base.py` & `sports-betting-0.5.0/src/sportsbet/evaluation/_base.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/src/sportsbet/evaluation/_classifier.py` & `sports-betting-0.5.0/src/sportsbet/evaluation/_classifier.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/src/sportsbet/evaluation/_rules.py` & `sports-betting-0.5.0/src/sportsbet/evaluation/_rules.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/tests/cli/test_datasets.py` & `sports-betting-0.5.0/tests/cli/test_datasets.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/tests/cli/test_evaluation.py` & `sports-betting-0.5.0/tests/cli/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/tests/datasets/test_dummy.py` & `sports-betting-0.5.0/tests/datasets/test_dummy.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/tests/evaluation/test_classifier.py` & `sports-betting-0.5.0/tests/evaluation/test_classifier.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/tests/evaluation/test_rules.py` & `sports-betting-0.5.0/tests/evaluation/test_rules.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.4.0/PKG-INFO` & `sports-betting-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports-betting
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python sports betting toolbox.
 License: MIT
 Keywords: sports betting,sports analytics,machine learning
 Author-email: Georgios Douzas <gdouzas@icloud.com>
 Requires-Python: >=3.9, <3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 Classifier: Typing :: Typed
 Project-URL: Changelog, https://georgedouzas.github.io/sports-betting/changelog
 Project-URL: Discussions, https://github.com/georgedouzas/sports-betting/discussions
 Project-URL: Documentation, https://georgedouzas.github.io/sports-betting
 Project-URL: Funding, https://github.com/sponsors/georgedouzas
 Project-URL: Gitter, https://gitter.im/sports-betting/community
 Project-URL: Homepage, https://georgedouzas.github.io/sports-betting
-Project-URL: Issues, https://github/georgedouzas/sports-betting/issues
+Project-URL: Issues, https://github.com/georgedouzas/sports-betting/issues
 Project-URL: Repository, https://github.com/georgedouzas/sports-betting
 Description-Content-Type: text/markdown
 
 [scikit-learn]: <http://scikit-learn.org/stable/>
 [black badge]: <https://img.shields.io/badge/%20style-black-000000.svg>
 [black]: <https://github.com/psf/black>
 [docformatter badge]: <https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg>
```


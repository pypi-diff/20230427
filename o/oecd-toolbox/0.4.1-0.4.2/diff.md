# Comparing `tmp/oecd_toolbox-0.4.1.tar.gz` & `tmp/oecd_toolbox-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oecd_toolbox-0.4.1.tar", last modified: Wed Apr 26 09:41:32 2023, max compression
+gzip compressed data, was "oecd_toolbox-0.4.2.tar", last modified: Thu Apr 27 12:13:02 2023, max compression
```

## Comparing `oecd_toolbox-0.4.1.tar` & `oecd_toolbox-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 09:41:32.399867 oecd_toolbox-0.4.1/
--rw-rw-rw-   0        0        0     1131 2021-12-03 19:53:43.000000 oecd_toolbox-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     5795 2023-04-26 09:41:32.399867 oecd_toolbox-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     5176 2023-04-26 09:39:10.000000 oecd_toolbox-0.4.1/README.md
--rw-rw-rw-   0        0        0      108 2021-12-03 19:53:44.000000 oecd_toolbox-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0      868 2023-04-26 09:41:32.407350 oecd_toolbox-0.4.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 09:41:32.239796 oecd_toolbox-0.4.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 09:41:32.352439 oecd_toolbox-0.4.1/src/oecd_toolbox/
--rw-rw-rw-   0        0        0        0 2021-12-03 19:53:44.000000 oecd_toolbox-0.4.1/src/oecd_toolbox/__init__.py
--rw-rw-rw-   0        0        0     7046 2022-12-01 16:43:33.000000 oecd_toolbox-0.4.1/src/oecd_toolbox/converters.py
--rw-rw-rw-   0        0        0    13022 2023-04-26 09:39:10.000000 oecd_toolbox-0.4.1/src/oecd_toolbox/csv_writers.py
--rw-rw-rw-   0        0        0     5112 2022-02-04 15:48:18.000000 oecd_toolbox-0.4.1/src/oecd_toolbox/downloaders.py
-drwxrwxrwx   0        0        0        0 2023-04-26 09:41:32.393998 oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/
--rw-rw-rw-   0        0        0     5795 2023-04-26 09:41:32.000000 oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-04-26 09:41:32.000000 oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 09:41:32.000000 oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-04-26 09:41:32.000000 oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-26 09:41:32.000000 oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 12:13:02.920650 oecd_toolbox-0.4.2/
+-rw-rw-rw-   0        0        0     1131 2021-12-03 19:53:43.000000 oecd_toolbox-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     5795 2023-04-27 12:13:02.922370 oecd_toolbox-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5176 2023-04-26 09:39:10.000000 oecd_toolbox-0.4.2/README.md
+-rw-rw-rw-   0        0        0      108 2021-12-03 19:53:44.000000 oecd_toolbox-0.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0      868 2023-04-27 12:13:02.932002 oecd_toolbox-0.4.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 12:13:02.697808 oecd_toolbox-0.4.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 12:13:02.808055 oecd_toolbox-0.4.2/src/oecd_toolbox/
+-rw-rw-rw-   0        0        0        0 2021-12-03 19:53:44.000000 oecd_toolbox-0.4.2/src/oecd_toolbox/__init__.py
+-rw-rw-rw-   0        0        0     7046 2022-12-01 16:43:33.000000 oecd_toolbox-0.4.2/src/oecd_toolbox/converters.py
+-rw-rw-rw-   0        0        0    13022 2023-04-27 12:08:54.000000 oecd_toolbox-0.4.2/src/oecd_toolbox/csv_writers.py
+-rw-rw-rw-   0        0        0     5112 2022-02-04 15:48:18.000000 oecd_toolbox-0.4.2/src/oecd_toolbox/downloaders.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:13:02.910316 oecd_toolbox-0.4.2/src/oecd_toolbox.egg-info/
+-rw-rw-rw-   0        0        0     5795 2023-04-27 12:13:02.000000 oecd_toolbox-0.4.2/src/oecd_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-04-27 12:13:02.000000 oecd_toolbox-0.4.2/src/oecd_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 12:13:02.000000 oecd_toolbox-0.4.2/src/oecd_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-04-27 12:13:02.000000 oecd_toolbox-0.4.2/src/oecd_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-27 12:13:02.000000 oecd_toolbox-0.4.2/src/oecd_toolbox.egg-info/top_level.txt
```

### Comparing `oecd_toolbox-0.4.1/LICENSE` & `oecd_toolbox-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.4.1/PKG-INFO` & `oecd_toolbox-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oecd_toolbox
-Version: 0.4.1
+Version: 0.4.2
 Summary: OECD fetcher building templates and helpers
 Home-page: https://gitlab.algobank.oecd.org/oecd-data-fetchers1/OECD-TOOLBOX
 Author: Gyorgy Gyomai, Isaac Afambo, Alena Brin
 Author-email: gyorgy.gyomai@oecd.org
 Project-URL: Bug Tracker, https://gitlab.algobank.oecd.org/oecd-data-fetchers1/OECD-TOOLBOX/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `oecd_toolbox-0.4.1/README.md` & `oecd_toolbox-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.4.1/setup.cfg` & `oecd_toolbox-0.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 6563 645f 746f 6f6c 626f 780d   = oecd_toolbox.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e34 2e31  .version = 0.4.1
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e34 2e32  .version = 0.4.2
 00000030: 0d0a 6175 7468 6f72 203d 2047 796f 7267  ..author = Gyorg
 00000040: 7920 4779 6f6d 6169 2c20 4973 6161 6320  y Gyomai, Isaac 
 00000050: 4166 616d 626f 2c20 416c 656e 6120 4272  Afambo, Alena Br
 00000060: 696e 0d0a 6175 7468 6f72 5f65 6d61 696c  in..author_email
 00000070: 203d 2067 796f 7267 792e 6779 6f6d 6169   = gyorgy.gyomai
 00000080: 406f 6563 642e 6f72 670d 0a64 6573 6372  @oecd.org..descr
 00000090: 6970 7469 6f6e 203d 204f 4543 4420 6665  iption = OECD fe
```

### Comparing `oecd_toolbox-0.4.1/src/oecd_toolbox/converters.py` & `oecd_toolbox-0.4.2/src/oecd_toolbox/converters.py`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.4.1/src/oecd_toolbox/csv_writers.py` & `oecd_toolbox-0.4.2/src/oecd_toolbox/csv_writers.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
                         dim_dict['year'], dim_dict['freq'], dim_dict['period'] = get_DC_compatible_date(obs[0])
                         for c, v in enumerate(series['observations'][0][1:]):
                             dim_dict[v] = obs[c+1]
 
                         L.append(dim_dict)
                         
                 elif target_freq and f_aggregation and (target_freq in DC_eligible_frequencies):
-                    fieldnames.append('value')
+                    fieldnames.append('VALUE')
                     L.append({v:v for v in fieldnames}) 
                     df = pd.DataFrame(data=series["observations"][1:],columns=series["observations"][0]) 
                     # this only aggregates values, but omits observation attributes that might be in the original file                   
                     df_new_freq = df.groupby(pd.PeriodIndex(df['PERIOD'], freq=target_freq.to_dimension_code()))['VALUE'].apply(f_aggregation)
                     for ind in df_new_freq.index:
                         dim_dict=dict()
                         dim_dict['code'] = series['code']
```

### Comparing `oecd_toolbox-0.4.1/src/oecd_toolbox/downloaders.py` & `oecd_toolbox-0.4.2/src/oecd_toolbox/downloaders.py`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/PKG-INFO` & `oecd_toolbox-0.4.2/src/oecd_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oecd-toolbox
-Version: 0.4.1
+Version: 0.4.2
 Summary: OECD fetcher building templates and helpers
 Home-page: https://gitlab.algobank.oecd.org/oecd-data-fetchers1/OECD-TOOLBOX
 Author: Gyorgy Gyomai, Isaac Afambo, Alena Brin
 Author-email: gyorgy.gyomai@oecd.org
 Project-URL: Bug Tracker, https://gitlab.algobank.oecd.org/oecd-data-fetchers1/OECD-TOOLBOX/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/apexmf-0.3.2.tar.gz` & `tmp/apexmf-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\apexmf-0.3.2.tar", last modified: Thu Feb  2 22:35:41 2023, max compression
+gzip compressed data, was "apexmf-0.4.0.tar", last modified: Thu Apr 27 21:01:01 2023, max compression
```

## Comparing `apexmf-0.3.2.tar` & `apexmf-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-02-02 22:35:41.000000 apexmf-0.3.2/
--rw-rw-rw-   0        0        0     1549 2022-02-07 21:13:22.000000 apexmf-0.3.2/LICENSE
--rw-rw-rw-   0        0        0       26 2022-02-14 17:45:17.000000 apexmf-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2196 2023-02-02 22:35:41.000000 apexmf-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2022-09-05 15:21:30.000000 apexmf-0.3.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-02 22:35:41.000000 apexmf-0.3.2/apexmf/
--rw-rw-rw-   0        0        0      443 2022-03-22 18:08:34.000000 apexmf-0.3.2/apexmf/__init__.py
--rw-rw-rw-   0        0        0    31262 2023-02-02 22:25:16.000000 apexmf-0.3.2/apexmf/apexmf_pst_par.py
--rw-rw-rw-   0        0        0     3076 2020-01-02 16:14:19.000000 apexmf-0.3.2/apexmf/apexmf_pst_stats.py
--rw-rw-rw-   0        0        0    49972 2023-02-02 22:35:03.000000 apexmf-0.3.2/apexmf/apexmf_pst_utils.py
--rw-rw-rw-   0        0        0    24332 2023-01-30 05:40:30.000000 apexmf-0.3.2/apexmf/apexmf_pst_viz.py
--rw-rw-rw-   0        0        0    15836 2022-02-14 17:26:36.000000 apexmf-0.3.2/apexmf/apexmf_scenario_utils.py
--rw-rw-rw-   0        0        0    19710 2022-06-13 15:47:40.000000 apexmf-0.3.2/apexmf/apexmf_utils.py
--rw-rw-rw-   0        0        0     5787 2022-05-24 20:20:06.000000 apexmf-0.3.2/apexmf/forward_run.py
--rw-rw-rw-   0        0        0     1974 2021-06-02 17:31:06.000000 apexmf-0.3.2/apexmf/forward_run_gns.py
--rw-rw-rw-   0        0        0     1202 2020-11-01 18:16:33.000000 apexmf-0.3.2/apexmf/forward_run_tmp.py
-drwxrwxrwx   0        0        0        0 2023-02-02 22:35:41.000000 apexmf-0.3.2/apexmf/opt_files/
--rwxrwxrwx   0        0        0  9834496 2023-01-27 22:33:24.000000 apexmf-0.3.2/apexmf/opt_files/amrs_rel230127.exe
--rw-rw-rw-   0        0        0    34998 2022-04-18 21:33:32.000000 apexmf-0.3.2/apexmf/opt_files/apex.parm.xlsx
--rwxrwxrwx   0        0        0  2826752 2019-05-12 16:54:36.000000 apexmf-0.3.2/apexmf/opt_files/beopest64.exe
--rw-rw-rw-   0        0        0       37 2022-03-02 20:51:04.000000 apexmf-0.3.2/apexmf/opt_files/crop.parm
--rwxrwxrwx   0        0        0  2470400 2017-04-27 22:26:52.000000 apexmf-0.3.2/apexmf/opt_files/i64pest.exe
--rwxrwxrwx   0        0        0   844288 2019-11-21 19:44:00.000000 apexmf-0.3.2/apexmf/opt_files/i64pwtadj1.exe
-drwxrwxrwx   0        0        0        0 2023-02-02 22:35:41.000000 apexmf-0.3.2/apexmf/salt/
--rw-rw-rw-   0        0        0      252 2023-01-30 18:45:07.000000 apexmf-0.3.2/apexmf/salt/__init__.py
--rw-rw-rw-   0        0        0     4429 2023-02-02 17:42:45.000000 apexmf-0.3.2/apexmf/salt/salt_handler.py
--rw-rw-rw-   0        0        0     6209 2023-02-02 22:03:26.000000 apexmf-0.3.2/apexmf/salt_forward_run.py
--rw-rw-rw-   0        0        0     1159 2020-06-02 21:21:54.000000 apexmf-0.3.2/apexmf/swat_par_chg_run.py
--rw-rw-rw-   0        0        0     3291 2022-02-26 07:26:51.000000 apexmf-0.3.2/apexmf/utils.py
--rw-rw-rw-   0        0        0       22 2023-02-02 22:35:22.000000 apexmf-0.3.2/apexmf/version.py
-drwxrwxrwx   0        0        0        0 2023-02-02 22:35:41.000000 apexmf-0.3.2/apexmf.egg-info/
--rw-rw-rw-   0        0        0     2196 2023-02-02 22:35:40.000000 apexmf-0.3.2/apexmf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      767 2023-02-02 22:35:41.000000 apexmf-0.3.2/apexmf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-02 22:35:40.000000 apexmf-0.3.2/apexmf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-02-02 22:35:40.000000 apexmf-0.3.2/apexmf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-02 22:35:40.000000 apexmf-0.3.2/apexmf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-02 22:35:41.000000 apexmf-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1834 2023-02-02 22:35:30.000000 apexmf-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:01:01.610576 apexmf-0.4.0/
+-rw-rw-rw-   0        0        0     1549 2022-02-07 21:13:22.000000 apexmf-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0       26 2022-02-14 17:45:17.000000 apexmf-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2156 2023-04-27 21:01:01.605584 apexmf-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2022-09-05 15:21:30.000000 apexmf-0.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-27 21:01:01.315509 apexmf-0.4.0/apexmf/
+-rw-rw-rw-   0        0        0      443 2022-03-22 18:08:34.000000 apexmf-0.4.0/apexmf/__init__.py
+-rw-rw-rw-   0        0        0    31260 2023-02-28 23:24:02.000000 apexmf-0.4.0/apexmf/apexmf_pst_par.py
+-rw-rw-rw-   0        0        0     3076 2020-01-02 16:14:19.000000 apexmf-0.4.0/apexmf/apexmf_pst_stats.py
+-rw-rw-rw-   0        0        0    49972 2023-02-17 16:33:59.000000 apexmf-0.4.0/apexmf/apexmf_pst_utils.py
+-rw-rw-rw-   0        0        0    24332 2023-03-03 19:42:15.000000 apexmf-0.4.0/apexmf/apexmf_pst_viz.py
+-rw-rw-rw-   0        0        0    15836 2022-02-14 17:26:36.000000 apexmf-0.4.0/apexmf/apexmf_scenario_utils.py
+-rw-rw-rw-   0        0        0    19710 2022-06-13 15:47:40.000000 apexmf-0.4.0/apexmf/apexmf_utils.py
+-rw-rw-rw-   0        0        0     5787 2022-05-24 20:20:06.000000 apexmf-0.4.0/apexmf/forward_run.py
+-rw-rw-rw-   0        0        0     1974 2021-06-02 17:31:06.000000 apexmf-0.4.0/apexmf/forward_run_gns.py
+-rw-rw-rw-   0        0        0     1202 2020-11-01 18:16:33.000000 apexmf-0.4.0/apexmf/forward_run_tmp.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:01:01.551560 apexmf-0.4.0/apexmf/opt_files/
+-rwxrwxrwx   0        0        0  9834496 2023-01-27 22:33:24.000000 apexmf-0.4.0/apexmf/opt_files/amrs_rel230127.exe
+-rw-rw-rw-   0        0        0    34998 2022-04-18 21:33:32.000000 apexmf-0.4.0/apexmf/opt_files/apex.parm.xlsx
+-rwxrwxrwx   0        0        0  2826752 2019-05-12 16:54:36.000000 apexmf-0.4.0/apexmf/opt_files/beopest64.exe
+-rw-rw-rw-   0        0        0       37 2022-03-02 20:51:04.000000 apexmf-0.4.0/apexmf/opt_files/crop.parm
+-rwxrwxrwx   0        0        0  2470400 2017-04-27 22:26:52.000000 apexmf-0.4.0/apexmf/opt_files/i64pest.exe
+-rwxrwxrwx   0        0        0   844288 2019-11-21 19:44:00.000000 apexmf-0.4.0/apexmf/opt_files/i64pwtadj1.exe
+drwxrwxrwx   0        0        0        0 2023-04-27 21:01:01.593571 apexmf-0.4.0/apexmf/salt/
+-rw-rw-rw-   0        0        0      252 2023-01-30 18:45:07.000000 apexmf-0.4.0/apexmf/salt/__init__.py
+-rw-rw-rw-   0        0        0     7131 2023-03-23 03:07:27.000000 apexmf-0.4.0/apexmf/salt/analyzer.py
+-rw-rw-rw-   0        0        0     6680 2023-03-23 03:07:01.000000 apexmf-0.4.0/apexmf/salt/salt_handler.py
+-rw-rw-rw-   0        0        0     6209 2023-04-27 19:25:58.000000 apexmf-0.4.0/apexmf/salt_forward_run.py
+-rw-rw-rw-   0        0        0     1159 2020-06-02 21:21:54.000000 apexmf-0.4.0/apexmf/swat_par_chg_run.py
+-rw-rw-rw-   0        0        0     3339 2023-04-07 19:53:42.000000 apexmf-0.4.0/apexmf/utils.py
+-rw-rw-rw-   0        0        0       22 2023-04-27 21:00:25.000000 apexmf-0.4.0/apexmf/version.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:01:01.372516 apexmf-0.4.0/apexmf.egg-info/
+-rw-rw-rw-   0        0        0     2156 2023-04-27 21:01:00.000000 apexmf-0.4.0/apexmf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2023-04-27 21:01:01.000000 apexmf-0.4.0/apexmf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 21:01:00.000000 apexmf-0.4.0/apexmf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-27 21:01:00.000000 apexmf-0.4.0/apexmf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 21:01:00.000000 apexmf-0.4.0/apexmf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 21:01:01.614585 apexmf-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1828 2023-04-27 21:00:30.000000 apexmf-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apexmf-0.3.2/LICENSE` & `apexmf-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/PKG-INFO` & `apexmf-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: apexmf
-Version: 0.3.2
+Version: 0.4.0
 Summary: apexmf is a set of python modules for APEX-MODFLOW model evaluation and parameter estimation.
 Download-URL: https://pypi.org/project/apexmf
 Author: Seonggyu Park
 Author-email: <envpsg@gmail.com>
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/spark-brc/apexmf/issues
 Project-URL: Source Code, https://github.com/spark-brc/apexmf
 Project-URL: Documentation, https://github.com/spark-brc/apexmf
 Keywords: python,APEX-MODFLOW,PEST
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 apexmf
 ------
@@ -54,9 +52,7 @@
    >>> apexmf_pst_utils.init_setup(wd, APEX_wd)
 
    'apex.parm.xlsx' file copied ... passed
    'beopest64.exe' file copied ... passed
    'i64pest.exe' file copied ... passed
    'i64pwtadj1.exe' file copied ... passed
    'forward_run.py' file copied ... passed
-
-
```

### Comparing `apexmf-0.3.2/README.rst` & `apexmf-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/apexmf_pst_par.py` & `apexmf-0.4.0/apexmf/apexmf_pst_par.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             f.write(line1)
             f.write(line2)
             f.write(line3)
             df_riv.to_csv(
                         f, sep='\t',
                         header=False,
                         index=False,
-                        line_terminator='\n',
+                        lineterminator='\n',
                         encoding='utf-8'
                         )
         print(os.path.basename(riv_f) + " file is overwritten successfully!")
 
     elif len(riv_files) > 1:
         print(
                 "You have more than one River Package file!("+str(len(riv_files))+")"+"\n"
@@ -714,15 +714,15 @@
         data = f.readlines()
         data1 = [x.split() for x in data] # make each line a list
     with open('SALINITY/salt_input','w') as wf:
         for d in data[:nlines[0]+2]:
             wf.write(d)
         sub_con_df.to_csv(
                     wf, sep =' ', index=None, header=None, float_format='%.5e',
-                    line_terminator='\n', encoding='utf-8'
+                    lineterminator='\n', encoding='utf-8'
                     )
         wf.write('\n')
         for d in data[nlines[1]:]:
             wf.write(d)
     print('The "salt_input" file has been updated ...')
```

### Comparing `apexmf-0.3.2/apexmf/apexmf_pst_stats.py` & `apexmf-0.4.0/apexmf/apexmf_pst_stats.py`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/apexmf_pst_utils.py` & `apexmf-0.4.0/apexmf/apexmf_pst_utils.py`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/apexmf_pst_viz.py` & `apexmf-0.4.0/apexmf/apexmf_pst_viz.py`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/apexmf_scenario_utils.py` & `apexmf-0.4.0/apexmf/apexmf_scenario_utils.py`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/apexmf_utils.py` & `apexmf-0.4.0/apexmf/apexmf_utils.py`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/forward_run.py` & `apexmf-0.4.0/apexmf/forward_run.py`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/forward_run_gns.py` & `apexmf-0.4.0/apexmf/forward_run_gns.py`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/forward_run_tmp.py` & `apexmf-0.4.0/apexmf/forward_run_tmp.py`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/opt_files/amrs_rel230127.exe` & `apexmf-0.4.0/apexmf/opt_files/amrs_rel230127.exe`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/opt_files/apex.parm.xlsx` & `apexmf-0.4.0/apexmf/opt_files/apex.parm.xlsx`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/opt_files/beopest64.exe` & `apexmf-0.4.0/apexmf/opt_files/beopest64.exe`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/opt_files/i64pest.exe` & `apexmf-0.4.0/apexmf/opt_files/i64pest.exe`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/opt_files/i64pwtadj1.exe` & `apexmf-0.4.0/apexmf/opt_files/i64pwtadj1.exe`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/salt_forward_run.py` & `apexmf-0.4.0/apexmf/salt_forward_run.py`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/swat_par_chg_run.py` & `apexmf-0.4.0/apexmf/swat_par_chg_run.py`

 * *Files identical despite different names*

### Comparing `apexmf-0.3.2/apexmf/utils.py` & `apexmf-0.4.0/apexmf/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             *sims* series, and *μ* is the arithmetic mean.
 
         """
         nse_ = 1 - (
                 np.sum((obds - sims) ** 2, axis=0, dtype=np.float64)
                 / np.sum((obds - np.mean(obds)) ** 2, dtype=np.float64)
         )
-        return nse_
+        return round(nse_, 4)
 
     @staticmethod
     def rmse(sims, obds):
         """Root Mean Square Error (RMSE).
 
         :Calculation Details:
             .. math::
@@ -41,15 +41,15 @@
             periods, *e* is the *obds* series, *s* is (one of) the
             *sims* series.
 
         """
         rmse_ = np.sqrt(np.mean((obds - sims) ** 2,
                                 axis=0, dtype=np.float64))
 
-        return rmse_
+        return round(rmse_, 4)
 
     @staticmethod
     def pbias(sims, obds):
         """Percent Bias (PBias).
 
         :Calculation Details:
             .. math::
@@ -59,29 +59,29 @@
             periods, *e* is the *obds* series, and *s* is (one of)
             the *sims* series.
 
         """
         pbias_ = (100 * np.sum(obds - sims, axis=0, dtype=np.float64)
                 / np.sum(obds))
 
-        return pbias_
+        return round(pbias_, 4)
 
     @staticmethod
     def rsq(sims, obds):
         ## R-squared
         rsq_ = (
             (
                 (sum((obds - obds.mean())*(sims-sims.mean())))**2
             ) 
             /
             (
                 (sum((obds - obds.mean())**2)* (sum((sims-sims.mean())**2))
             ))
         )
-        return rsq_
+        return round(rsq_, 4)
 
 class DefineTime:
 
     def __init__(self) -> None:
         pass
 
     def get_start_end_time(self):
@@ -96,8 +96,8 @@
             stday = int(data[0][3])
             ptcode = int(data[0][4])
             edyr = styr + numyr -1
             stdate = datetime.datetime(styr, stmon, 1) + datetime.timedelta(stday - 1)
             eddate = datetime.datetime(edyr, 12, 31)
             stdate_ = stdate.strftime("%m/%d/%Y")
             eddate_ = eddate.strftime("%m/%d/%Y")
-            return stdate_, eddate_
+            return stdate_, eddate_, ptcode
```

### Comparing `apexmf-0.3.2/apexmf.egg-info/PKG-INFO` & `apexmf-0.4.0/apexmf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: apexmf
-Version: 0.3.2
+Version: 0.4.0
 Summary: apexmf is a set of python modules for APEX-MODFLOW model evaluation and parameter estimation.
 Download-URL: https://pypi.org/project/apexmf
 Author: Seonggyu Park
 Author-email: <envpsg@gmail.com>
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/spark-brc/apexmf/issues
 Project-URL: Source Code, https://github.com/spark-brc/apexmf
 Project-URL: Documentation, https://github.com/spark-brc/apexmf
 Keywords: python,APEX-MODFLOW,PEST
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 apexmf
 ------
@@ -54,9 +52,7 @@
    >>> apexmf_pst_utils.init_setup(wd, APEX_wd)
 
    'apex.parm.xlsx' file copied ... passed
    'beopest64.exe' file copied ... passed
    'i64pest.exe' file copied ... passed
    'i64pwtadj1.exe' file copied ... passed
    'forward_run.py' file copied ... passed
-
-
```

### Comparing `apexmf-0.3.2/apexmf.egg-info/SOURCES.txt` & `apexmf-0.4.0/apexmf.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 apexmf/opt_files/amrs_rel230127.exe
 apexmf/opt_files/apex.parm.xlsx
 apexmf/opt_files/beopest64.exe
 apexmf/opt_files/crop.parm
 apexmf/opt_files/i64pest.exe
 apexmf/opt_files/i64pwtadj1.exe
 apexmf/salt/__init__.py
+apexmf/salt/analyzer.py
 apexmf/salt/salt_handler.py
```

### Comparing `apexmf-0.3.2/setup.py` & `apexmf-0.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #     long_description = "\n" + fh.read()
 
 
 with open("README.rst", "r") as fd:
     long_desc = fd.read()
 
 
-VERSION = '0.3.2'
+VERSION = '0.4.0'
 DESCRIPTION = 'apexmf is a set of python modules for APEX-MODFLOW model evaluation and parameter estimation.'
 # LONG_DESCRIPTION = 'A package that allows to work with apex-MODFLOW model'
 
 license = "BSD-3-Clause"
 # Setting up
 setup(
     name="apexmf",
@@ -34,21 +34,21 @@
     },
     include_package_data=True,
     package_data = {
         'opt_files': ['*'],
     },
     packages=find_packages(),
     install_requires=[
-        'pandas', 'numpy', 'pyemu', 'flopy<=3.3.4', 'scipy', 'matplotlib', 'openpyxl',
+        'pandas', 'numpy', 'pyemu', 'flopy', 'scipy', 'matplotlib', 'openpyxl',
         'hydroeval', 'tqdm', 'termcolor', 'pyshp'],
     keywords=['python', 'APEX-MODFLOW', 'PEST'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         "Operating System :: Microsoft :: Windows",
         "License :: OSI Approved :: BSD License"
     ]
 )
```


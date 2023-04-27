# Comparing `tmp/pheno-utils-0.1.8.tar.gz` & `tmp/pheno-utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.1.8.tar", last modified: Tue Apr 25 08:52:35 2023, max compression
+gzip compressed data, was "pheno-utils-0.1.9.tar", last modified: Wed Apr 26 20:36:55 2023, max compression
```

## Comparing `pheno-utils-0.1.8.tar` & `pheno-utils-0.1.9.tar`

### file list

```diff
@@ -1,98 +1,31 @@
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:35.075601 pheno-utils-0.1.8/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.595014 pheno-utils-0.1.8/.github/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.685728 pheno-utils-0.1.8/.github/workflows/
--rw-rw-r--   0 jovyan    (1000) users      (100)      242 2023-01-20 02:50:04.000000 pheno-utils-0.1.8/.github/workflows/deploy.yaml
--rw-rw-r--   0 jovyan    (1000) users      (100)      148 2023-01-20 02:50:04.000000 pheno-utils-0.1.8/.github/workflows/test.yaml
--rw-r--r--   0 jovyan    (1000) users      (100)     1832 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/.gitignore
--rw-r--r--   0 jovyan    (1000) users      (100)    11357 2023-03-25 22:15:20.000000 pheno-utils-0.1.8/LICENSE
--rw-rw-r--   0 jovyan    (1000) users      (100)      111 2023-01-20 02:50:04.000000 pheno-utils-0.1.8/MANIFEST.in
--rw-r--r--   0 jovyan    (1000) users      (100)     1230 2023-04-25 08:52:35.073272 pheno-utils-0.1.8/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)      446 2023-04-15 14:49:49.000000 pheno-utils-0.1.8/README.md
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.770024 pheno-utils-0.1.8/_proc/
--rw-r--r--   0 jovyan    (1000) users      (100)       10 2023-04-15 14:49:40.000000 pheno-utils-0.1.8/_proc/.gitignore
--rw-r--r--   0 jovyan    (1000) users      (100)    11835 2023-04-15 14:49:28.000000 pheno-utils-0.1.8/_proc/00_config.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)    26441 2023-04-15 14:49:33.000000 pheno-utils-0.1.8/_proc/01_basic_plots.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)    62671 2023-04-15 14:49:33.000000 pheno-utils-0.1.8/_proc/02_blandaltman_plots.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)   393501 2023-04-15 14:49:34.000000 pheno-utils-0.1.8/_proc/03_age_reference_plots.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)   274893 2023-04-15 14:49:32.000000 pheno-utils-0.1.8/_proc/04_date_plots.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)    62496 2023-04-15 14:49:34.000000 pheno-utils-0.1.8/_proc/05_data_loader.ipynb
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.786607 pheno-utils-0.1.8/_proc/_docs/
--rw-r--r--   0 jovyan    (1000) users      (100)      229 2023-04-15 14:49:51.000000 pheno-utils-0.1.8/_proc/_docs/index.html
--rw-r--r--   0 jovyan    (1000) users      (100)       60 2023-04-15 14:49:51.000000 pheno-utils-0.1.8/_proc/_docs/robots.txt
--rw-r--r--   0 jovyan    (1000) users      (100)      110 2023-04-15 14:49:51.000000 pheno-utils-0.1.8/_proc/_docs/sitemap.xml
--rw-r--r--   0 jovyan    (1000) users      (100)      290 2023-03-25 22:16:51.000000 pheno-utils-0.1.8/_proc/_quarto.yml
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.614067 pheno-utils-0.1.8/_proc/examples/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.606836 pheno-utils-0.1.8/_proc/examples/Fundus/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.800396 pheno-utils-0.1.8/_proc/examples/Fundus/10k/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.611188 pheno-utils-0.1.8/_proc/examples/Fundus/10k/M0/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.817826 pheno-utils-0.1.8/_proc/examples/Fundus/10k/M0/images/
--rw-r--r--   0 jovyan    (1000) users      (100)     2109 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/_proc/examples/Fundus/10k/M0/images/fundus_0.png
--rw-r--r--   0 jovyan    (1000) users      (100)     2109 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/_proc/examples/Fundus/10k/M0/images/fundus_1.png
--rw-r--r--   0 jovyan    (1000) users      (100)     2109 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/_proc/examples/Fundus/10k/M0/images/fundus_2.png
--rw-r--r--   0 jovyan    (1000) users      (100)    69919 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/_proc/examples/Fundus/10k/fundus.parquet
--rw-r--r--   0 jovyan    (1000) users      (100)      576 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/_proc/examples/Fundus/10k/fundus_data_dictionary.csv
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.615776 pheno-utils-0.1.8/_proc/examples/Population_Characteristics/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.823281 pheno-utils-0.1.8/_proc/examples/Population_Characteristics/10k/
--rw-r--r--   0 jovyan    (1000) users      (100)     5066 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/_proc/examples/Population_Characteristics/10k/events.parquet
--rw-r--r--   0 jovyan    (1000) users      (100)     2889 2023-04-15 14:49:33.000000 pheno-utils-0.1.8/_proc/index.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)      247 2023-04-15 14:49:22.000000 pheno-utils-0.1.8/_proc/nbdev.yml
--rw-rw-r--   0 jovyan    (1000) users      (100)      600 2023-01-20 02:50:04.000000 pheno-utils-0.1.8/_proc/styles.css
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.929154 pheno-utils-0.1.8/nbs/
--rw-r--r--   0 jovyan    (1000) users      (100)    12888 2023-04-24 09:14:42.000000 pheno-utils-0.1.8/nbs/00_config.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)    24935 2023-04-17 11:06:13.000000 pheno-utils-0.1.8/nbs/01_basic_plots.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)    63698 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/nbs/02_blandaltman_plots.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)   402245 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/nbs/03_age_reference_plots.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)   274749 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/nbs/04_date_plots.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)    72862 2023-04-25 08:51:36.000000 pheno-utils-0.1.8/nbs/05_data_loader.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)    17273 2023-04-17 10:44:14.000000 pheno-utils-0.1.8/nbs/06_sleep_plots.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)    11057 2023-04-24 09:14:42.000000 pheno-utils-0.1.8/nbs/07_basic_analysis.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)   233579 2023-04-17 10:44:19.000000 pheno-utils-0.1.8/nbs/08_cgm_plots.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)     3749 2023-04-19 15:24:28.000000 pheno-utils-0.1.8/nbs/09_ecg_analysis.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)     2558 2023-04-25 08:46:08.000000 pheno-utils-0.1.8/nbs/10_subset_loader.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)      290 2023-03-25 22:16:51.000000 pheno-utils-0.1.8/nbs/_quarto.yml
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.637135 pheno-utils-0.1.8/nbs/examples/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.935432 pheno-utils-0.1.8/nbs/examples/cgm/
--rw-r--r--   0 jovyan    (1000) users      (100)     8182 2023-04-15 20:19:05.000000 pheno-utils-0.1.8/nbs/examples/cgm/cgm_sample_data.parquet
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.940269 pheno-utils-0.1.8/nbs/examples/diet_logging/
--rw-r--r--   0 jovyan    (1000) users      (100)     5795 2023-04-15 20:25:33.000000 pheno-utils-0.1.8/nbs/examples/diet_logging/diet_sample_data.parquet
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.629828 pheno-utils-0.1.8/nbs/examples/fundus/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.950778 pheno-utils-0.1.8/nbs/examples/fundus/10k/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.634289 pheno-utils-0.1.8/nbs/examples/fundus/10k/M0/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.966399 pheno-utils-0.1.8/nbs/examples/fundus/10k/M0/images/
--rw-r--r--   0 jovyan    (1000) users      (100)     2109 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/nbs/examples/fundus/10k/M0/images/fundus_0.png
--rw-r--r--   0 jovyan    (1000) users      (100)     2109 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/nbs/examples/fundus/10k/M0/images/fundus_1.png
--rw-r--r--   0 jovyan    (1000) users      (100)     2109 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/nbs/examples/fundus/10k/M0/images/fundus_2.png
--rw-r--r--   0 jovyan    (1000) users      (100)    69919 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/nbs/examples/fundus/10k/fundus.parquet
--rw-r--r--   0 jovyan    (1000) users      (100)      576 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/nbs/examples/fundus/10k/fundus_data_dictionary.csv
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.638748 pheno-utils-0.1.8/nbs/examples/population/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:34.971717 pheno-utils-0.1.8/nbs/examples/population/10k/
--rw-r--r--   0 jovyan    (1000) users      (100)     5066 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/nbs/examples/population/10k/events.parquet
--rw-r--r--   0 jovyan    (1000) users      (100)     2879 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/nbs/index.ipynb
--rw-r--r--   0 jovyan    (1000) users      (100)      247 2023-04-25 08:52:20.000000 pheno-utils-0.1.8/nbs/nbdev.yml
--rw-r--r--   0 jovyan    (1000) users      (100)      265 2023-04-14 12:58:24.000000 pheno-utils-0.1.8/nbs/sidebar.yml
--rw-rw-r--   0 jovyan    (1000) users      (100)      600 2023-01-20 02:50:04.000000 pheno-utils-0.1.8/nbs/styles.css
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:35.032002 pheno-utils-0.1.8/pheno_utils/
--rw-r--r--   0 jovyan    (1000) users      (100)      328 2023-04-25 08:52:00.000000 pheno-utils-0.1.8/pheno_utils/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)    13907 2023-04-25 08:52:00.000000 pheno-utils-0.1.8/pheno_utils/_modidx.py
--rw-r--r--   0 jovyan    (1000) users      (100)    16963 2023-04-25 08:52:00.000000 pheno-utils-0.1.8/pheno_utils/age_reference_plots.py
--rw-r--r--   0 jovyan    (1000) users      (100)     5300 2023-04-25 08:52:00.000000 pheno-utils-0.1.8/pheno_utils/basic_analysis.py
--rw-r--r--   0 jovyan    (1000) users      (100)     2789 2023-04-25 08:52:00.000000 pheno-utils-0.1.8/pheno_utils/basic_plots.py
--rw-r--r--   0 jovyan    (1000) users      (100)     2517 2023-04-25 08:52:00.000000 pheno-utils-0.1.8/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 jovyan    (1000) users      (100)     7865 2023-04-25 08:52:00.000000 pheno-utils-0.1.8/pheno_utils/cgm_plots.py
--rw-r--r--   0 jovyan    (1000) users      (100)     3599 2023-04-25 08:52:00.000000 pheno-utils-0.1.8/pheno_utils/config.py
--rw-r--r--   0 jovyan    (1000) users      (100)    17037 2023-04-25 08:52:00.000000 pheno-utils-0.1.8/pheno_utils/data_loader.py
--rw-r--r--   0 jovyan    (1000) users      (100)     2825 2023-04-25 08:52:00.000000 pheno-utils-0.1.8/pheno_utils/dates_plots.py
--rw-r--r--   0 jovyan    (1000) users      (100)     2113 2023-04-25 08:52:00.000000 pheno-utils-0.1.8/pheno_utils/ecg_analysis.py
--rw-r--r--   0 jovyan    (1000) users      (100)    13210 2023-04-25 08:52:00.000000 pheno-utils-0.1.8/pheno_utils/sleep_plots.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1225 2023-04-25 08:52:00.000000 pheno-utils-0.1.8/pheno_utils/subset_loader.py
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-25 08:52:35.068961 pheno-utils-0.1.8/pheno_utils.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)     1230 2023-04-25 08:52:34.000000 pheno-utils-0.1.8/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     2081 2023-04-25 08:52:34.000000 pheno-utils-0.1.8/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-04-25 08:52:34.000000 pheno-utils-0.1.8/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       44 2023-04-25 08:52:34.000000 pheno-utils-0.1.8/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-03-25 22:29:41.000000 pheno-utils-0.1.8/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 jovyan    (1000) users      (100)      127 2023-04-25 08:52:34.000000 pheno-utils-0.1.8/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       12 2023-04-25 08:52:34.000000 pheno-utils-0.1.8/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 jovyan    (1000) users      (100)     1068 2023-04-25 08:46:47.000000 pheno-utils-0.1.8/settings.ini
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-04-25 08:52:35.076572 pheno-utils-0.1.8/setup.cfg
--rw-rw-r--   0 jovyan    (1000) users      (100)     2560 2023-01-20 02:50:04.000000 pheno-utils-0.1.8/setup.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-26 20:36:55.770380 pheno-utils-0.1.9/
+-rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.9/LICENSE
+-rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.9/MANIFEST.in
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-26 20:36:55.769989 pheno-utils-0.1.9/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.9/README.md
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-26 20:36:55.765544 pheno-utils-0.1.9/pheno_utils/
+-rw-r--r--   0 alondmnt   (501) staff       (20)      355 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/__init__.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16451 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/_modidx.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     5300 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/basic_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/basic_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/cgm_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     3599 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/config.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    17193 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/data_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/dates_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     7306 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/meta_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/sleep_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1225 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/subset_loader.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-26 20:36:55.769322 pheno-utils-0.1.9/pheno_utils.egg-info/
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-26 20:36:55.000000 pheno-utils-0.1.9/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      681 2023-04-26 20:36:55.000000 pheno-utils-0.1.9/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-26 20:36:55.000000 pheno-utils-0.1.9/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-26 20:36:55.000000 pheno-utils-0.1.9/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.9/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 alondmnt   (501) staff       (20)      143 2023-04-26 20:36:55.000000 pheno-utils-0.1.9/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-26 20:36:55.000000 pheno-utils-0.1.9/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1086 2023-04-26 20:20:39.000000 pheno-utils-0.1.9/settings.ini
+-rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-26 20:36:55.770561 pheno-utils-0.1.9/setup.cfg
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.9/setup.py
```

### Comparing `pheno-utils-0.1.8/LICENSE` & `pheno-utils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.8/PKG-INFO` & `pheno-utils-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
+Description: pheno-utils
+        ================
+        
+        <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+        
+        Viz functions, loaders, mergers.
+        
+        WORK IN PROGRESS
+        
+        ## Install
+        
+        ``` sh
+        pip install pheno_utils
+        ```
+        
+        ## How to use
+        
+        Examples:
+        
+        ``` python
+        data = generate_synthetic_data(n=1000)
+        hist_ecdf_plots(data=data, col="val1")
+        ```
+        
+            NameError: name 'hist_ecdf_plots' is not defined
+        
+        ``` python
+        age_refplots = GenderAgeRefPlot(data, "val1")
+        age_refplots.plot()
+        ```
+        
 Keywords: nbdev jupyter notebook python
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSE
-
-pheno-utils
-================
-
-<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
-
-Viz functions, loaders, mergers.
-
-WORK IN PROGRESS
-
-## Install
-
-``` sh
-pip install pheno_utils
-```
-
-## How to use
-
-Examples:
-
-``` python
-data = generate_synthetic_data(n=1000)
-hist_ecdf_plots(data=data, col="val1")
-```
-
-    NameError: name 'hist_ecdf_plots' is not defined
-
-``` python
-age_refplots = GenderAgeRefPlot(data, "val1")
-age_refplots.plot()
-```
```

### Comparing `pheno-utils-0.1.8/pheno_utils/_modidx.py` & `pheno-utils-0.1.9/pheno_utils/_modidx.py`

 * *Files 12% similar despite different names*

```diff
@@ -91,14 +91,34 @@
                                          'pheno_utils.data_loader.DataLoader.load_sample_data': ( 'data_loader.html#dataloader.load_sample_data',
                                                                                                   'pheno_utils/data_loader.py')},
             'pheno_utils.dates_plots': { 'pheno_utils.dates_plots.dates_dist_plot': ( 'date_plots.html#dates_dist_plot',
                                                                                       'pheno_utils/dates_plots.py')},
             'pheno_utils.ecg_analysis': { 'pheno_utils.ecg_analysis.get_hrv_df': ( 'ecg_analysis.html#get_hrv_df',
                                                                                    'pheno_utils/ecg_analysis.py'),
                                           'pheno_utils.ecg_analysis.vis_ecg': ('ecg_analysis.html#vis_ecg', 'pheno_utils/ecg_analysis.py')},
+            'pheno_utils.meta_loader': { 'pheno_utils.meta_loader.MetaLoader': ( 'meta_loader.html#metaloader',
+                                                                                 'pheno_utils/meta_loader.py'),
+                                         'pheno_utils.meta_loader.MetaLoader.__concat__': ( 'meta_loader.html#metaloader.__concat__',
+                                                                                            'pheno_utils/meta_loader.py'),
+                                         'pheno_utils.meta_loader.MetaLoader.__get_dataset_path__': ( 'meta_loader.html#metaloader.__get_dataset_path__',
+                                                                                                      'pheno_utils/meta_loader.py'),
+                                         'pheno_utils.meta_loader.MetaLoader.__getitem__': ( 'meta_loader.html#metaloader.__getitem__',
+                                                                                             'pheno_utils/meta_loader.py'),
+                                         'pheno_utils.meta_loader.MetaLoader.__init__': ( 'meta_loader.html#metaloader.__init__',
+                                                                                          'pheno_utils/meta_loader.py'),
+                                         'pheno_utils.meta_loader.MetaLoader.__load_dictionaries__': ( 'meta_loader.html#metaloader.__load_dictionaries__',
+                                                                                                       'pheno_utils/meta_loader.py'),
+                                         'pheno_utils.meta_loader.MetaLoader.__repr__': ( 'meta_loader.html#metaloader.__repr__',
+                                                                                          'pheno_utils/meta_loader.py'),
+                                         'pheno_utils.meta_loader.MetaLoader.__str__': ( 'meta_loader.html#metaloader.__str__',
+                                                                                         'pheno_utils/meta_loader.py'),
+                                         'pheno_utils.meta_loader.MetaLoader.get': ( 'meta_loader.html#metaloader.get',
+                                                                                     'pheno_utils/meta_loader.py'),
+                                         'pheno_utils.meta_loader.MetaLoader.load': ( 'meta_loader.html#metaloader.load',
+                                                                                      'pheno_utils/meta_loader.py')},
             'pheno_utils.sleep_plots': { 'pheno_utils.sleep_plots.format_xticks': ( 'sleep_plots.html#format_xticks',
                                                                                     'pheno_utils/sleep_plots.py'),
                                          'pheno_utils.sleep_plots.get_legend_colors': ( 'sleep_plots.html#get_legend_colors',
                                                                                         'pheno_utils/sleep_plots.py'),
                                          'pheno_utils.sleep_plots.plot_channels': ( 'sleep_plots.html#plot_channels',
                                                                                     'pheno_utils/sleep_plots.py'),
                                          'pheno_utils.sleep_plots.plot_events': ( 'sleep_plots.html#plot_events',
```

### Comparing `pheno-utils-0.1.8/pheno_utils/age_reference_plots.py` & `pheno-utils-0.1.9/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.8/pheno_utils/basic_analysis.py` & `pheno-utils-0.1.9/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.8/pheno_utils/basic_plots.py` & `pheno-utils-0.1.9/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.8/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.1.9/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.8/pheno_utils/cgm_plots.py` & `pheno-utils-0.1.9/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.8/pheno_utils/config.py` & `pheno-utils-0.1.9/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.8/pheno_utils/data_loader.py` & `pheno-utils-0.1.9/pheno_utils/data_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,19 +119,17 @@
                 research_stage = [research_stage]
             query_str += ' and research_stage in @research_stage'
         if array_index is not None:
             if not isinstance(array_index, list):
                 array_index = [array_index]
             query_str += ' and array_index in @array_index'
 
-        where_field = self.dict.loc[field_name]
-        if isinstance(where_field['parent_dataframe'], str):
-            field_name = where_field['parent_dataframe']
-
-        sample = self[[field_name] + ['participant_id']].query(query_str).astype({field_name: str})
+        sample = self[[field_name] + ['participant_id']].query(query_str)
+        col = sample.columns[0]  # can be different from field_name is a parent_dataframe is implied
+        sample = sample.astype({col: str})
         missing_participants = np.setdiff1d(participant_id, sample['participant_id'].unique())
         sample = self.dataset_path + '/' + sample.iloc[:, 0]
 
         if len(missing_participants):
             if self.errors == 'raise':
                 raise ValueError(f'Missing samples: {missing_participants}')
             elif self.errors == 'warn':
@@ -205,14 +203,18 @@
             pd.DataFrame: Data for the specified fields from all tables
         """
         if flexible is None:
             flexible = self.flexible_field_search
         if isinstance(fields, str):
             fields = [fields]
 
+        # check whether any field points to a parent_dataframe
+        has_parent = self.dict.loc[self.dict.index.isin(fields), 'parent_dataframe'].dropna()
+        fields += has_parent.unique().tolist()
+
         data = pd.DataFrame()
         for df in self.dfs.values():
             if flexible:
                 # use fuzzy matching including regex to find fields
                 fields_in_col = np.unique([col for f in fields for col in df.columns if re.search(f, col)])
             else:
                 fields_in_col = df.columns.intersection(fields).difference(data.columns)
```

### Comparing `pheno-utils-0.1.8/pheno_utils/dates_plots.py` & `pheno-utils-0.1.9/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.8/pheno_utils/ecg_analysis.py` & `pheno-utils-0.1.9/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.8/pheno_utils/sleep_plots.py` & `pheno-utils-0.1.9/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.8/pheno_utils/subset_loader.py` & `pheno-utils-0.1.9/pheno_utils/subset_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.8/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.1.9/pheno_utils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
+Description: pheno-utils
+        ================
+        
+        <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+        
+        Viz functions, loaders, mergers.
+        
+        WORK IN PROGRESS
+        
+        ## Install
+        
+        ``` sh
+        pip install pheno_utils
+        ```
+        
+        ## How to use
+        
+        Examples:
+        
+        ``` python
+        data = generate_synthetic_data(n=1000)
+        hist_ecdf_plots(data=data, col="val1")
+        ```
+        
+            NameError: name 'hist_ecdf_plots' is not defined
+        
+        ``` python
+        age_refplots = GenderAgeRefPlot(data, "val1")
+        age_refplots.plot()
+        ```
+        
 Keywords: nbdev jupyter notebook python
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSE
-
-pheno-utils
-================
-
-<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
-
-Viz functions, loaders, mergers.
-
-WORK IN PROGRESS
-
-## Install
-
-``` sh
-pip install pheno_utils
-```
-
-## How to use
-
-Examples:
-
-``` python
-data = generate_synthetic_data(n=1000)
-hist_ecdf_plots(data=data, col="val1")
-```
-
-    NameError: name 'hist_ecdf_plots' is not defined
-
-``` python
-age_refplots = GenderAgeRefPlot(data, "val1")
-age_refplots.plot()
-```
```

### Comparing `pheno-utils-0.1.8/settings.ini` & `pheno-utils-0.1.9/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.1.8
+version = 0.1.9
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
@@ -34,10 +34,10 @@
 description = Pheno data utils - viz, loaders, mergers
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = hrossman
 
 ### Optional ###
-requirements = fastcore pandas==1.5.2 numpy scipy fastparquet matplotlib seaborn scikit-learn pyCompare tsmoothie smart_open neurokit2
+requirements = fastcore pandas==1.5.2 numpy scipy fastparquet matplotlib seaborn scikit-learn pyCompare tsmoothie smart_open neurokit2 "dask[dataframe]"
 # dev_requirements = 
 # console_scripts =
```

### Comparing `pheno-utils-0.1.8/setup.py` & `pheno-utils-0.1.9/setup.py`

 * *Files identical despite different names*


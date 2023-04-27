# Comparing `tmp/moftransformer-1.1.3.tar.gz` & `tmp/moftransformer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moftransformer-1.1.3.tar", last modified: Tue Apr 25 05:16:40 2023, max compression
+gzip compressed data, was "moftransformer-2.0.0.tar", last modified: Thu Apr 27 12:01:12 2023, max compression
```

## Comparing `moftransformer-1.1.3.tar` & `moftransformer-2.0.0.tar`

### file list

```diff
@@ -1,284 +1,285 @@
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.306906 moftransformer-1.1.3/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8389 2023-04-25 05:16:40.306906 moftransformer-1.1.3/PKG-INFO
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8011 2023-04-25 05:00:17.000000 moftransformer-1.1.3/README.md
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.262907 moftransformer-1.1.3/moftransformer/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2023-04-25 05:05:10.000000 moftransformer-1.1.3/moftransformer/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.262907 moftransformer-1.1.3/moftransformer/assets/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       40 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/assets/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12616 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/assets/bbs.json
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9431 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/assets/colors.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12647 2023-01-26 02:06:32.000000 moftransformer-1.1.3/moftransformer/assets/topology.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.266907 moftransformer-1.1.3/moftransformer/cli/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        0 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/cli/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2316 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/cli/download.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      290 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/cli/install_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3117 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/cli/main.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      537 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/cli/run.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      294 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/cli/uninstall_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3929 2023-04-25 05:00:17.000000 moftransformer-1.1.3/moftransformer/config.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10275 2023-04-25 04:35:31.000000 moftransformer-1.1.3/moftransformer/config_ex.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.266907 moftransformer-1.1.3/moftransformer/database/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      430 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/database/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.266907 moftransformer-1.1.3/moftransformer/datamodules/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      176 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/datamodules/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2906 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/datamodules/datamodule.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10145 2023-04-25 04:35:31.000000 moftransformer-1.1.3/moftransformer/datamodules/dataset.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.266907 moftransformer-1.1.3/moftransformer/examples/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      468 2023-01-05 12:04:50.000000 moftransformer-1.1.3/moftransformer/examples/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.266907 moftransformer-1.1.3/moftransformer/examples/dataset/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.266907 moftransformer-1.1.3/moftransformer/examples/dataset/test/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-04-04 13:23:21.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       73 2023-04-04 13:24:22.000000 moftransformer-1.1.3/moftransformer/examples/dataset/test_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.278907 moftransformer-1.1.3/moftransformer/examples/dataset/total/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-01-05 12:09:32.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-01-05 12:09:32.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:32.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:32.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:28.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:31.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-01-05 12:09:30.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-01-05 12:09:30.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:30.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:30.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:33.000000 moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.286907 moftransformer-1.1.3/moftransformer/examples/dataset/train/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      206 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/train_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.286907 moftransformer-1.1.3/moftransformer/examples/dataset/val/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/acs+N270+E33.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/acs+N270+E33.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/acs+N270+E33.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/acs+N270+E33.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/smm+N577+E166.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/smm+N577+E166.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/smm+N577+E166.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val/smm+N577+E166.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       43 2023-01-05 12:09:34.000000 moftransformer-1.1.3/moftransformer/examples/dataset/val_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.286907 moftransformer-1.1.3/moftransformer/examples/raw/
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7496 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/acs+N270+E33.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    17441 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9738 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/fee+N254+E185.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11392 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/mok+N109+E146.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    30404 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18345 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/raw_example.json
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11939 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/sml+N696+E182.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    24953 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/smm+N577+E166.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    28256 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/ukg+N387+E203.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    39904 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/vmk+N489+E8.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18930 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/vna+N650+E120.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    48803 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/raw/zzz+N96+N373+E34.cif
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.262907 moftransformer-1.1.3/moftransformer/examples/visualize/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.286907 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.290907 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9162 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12083 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6405 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8339 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7074 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9292 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    98728 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6419 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8357 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    93472 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6410 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8347 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6845 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8961 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   170530 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      164 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.294906 moftransformer-1.1.3/moftransformer/gadgets/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       45 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/gadgets/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1774 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/gadgets/my_metrics.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.262907 moftransformer-1.1.3/moftransformer/libs/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.298906 moftransformer-1.1.3/moftransformer/libs/GRIDAY/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2799 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/AtomTypeMap.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      654 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/AtomTypeMap.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    41808 2022-12-19 08:32:53.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/AtomTypeMap.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2448 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Cell.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7789 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      414 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ChannelAnalyzer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    33448 2022-12-19 08:32:54.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ChannelAnalyzer.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54588 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18619 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3812 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   143440 2022-12-19 08:32:55.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.o
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.302906 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4751 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/UFF_FF.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      845 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/UFF_Type.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      202 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/Zeolite_FF.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      190 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      318 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_Si.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       26 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/Zeolite_Type.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7197 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ForceField.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      866 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ForceField.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    67552 2022-12-19 08:32:55.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ForceField.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13991 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      865 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    57152 2022-12-19 08:32:56.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/FourierAnalyzer.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7362 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Framework.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1197 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Framework.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    47328 2022-12-19 08:32:57.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Framework.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3007 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Gaussian.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Gaussian.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15032 2022-12-19 08:32:57.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Gaussian.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9534 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridMaker.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      936 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridMaker.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    80288 2022-12-19 08:32:58.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridMaker.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      320 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Griday.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      948 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayException.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      669 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayException.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15752 2022-12-19 08:32:58.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayException.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      567 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayTypes.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4380 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/LennardJones.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/LennardJones.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    14896 2022-12-19 08:32:58.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/LennardJones.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      334 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Makefile
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    21824 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/MaterialGrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2366 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/MaterialGrid.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    75600 2022-12-19 08:32:59.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/MaterialGrid.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5664 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/NlistMaker.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      922 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/NlistMaker.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    65096 2022-12-19 08:32:59.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/NlistMaker.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      730 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/PairEnergy.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      570 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Random.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5106 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ShiftedLJ.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      764 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ShiftedLJ.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15360 2022-12-19 08:33:00.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/ShiftedLJ.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      811 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Timer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2277 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/Vector.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   698550 2022-12-19 08:33:00.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/libgriday.a
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.302906 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      563 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/Makefile
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5834 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2022-12-19 08:33:06.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid2COTA
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   278928 2022-12-19 08:33:05.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid2props
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2022-12-19 08:33:04.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid2visit
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   161656 2022-12-19 08:33:03.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid_gen
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1046 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/main_cota.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1742 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      900 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/main_visit.cpp
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.306906 moftransformer-1.1.3/moftransformer/modules/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       90 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/modules/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5607 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/modules/cgcnn.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3217 2023-01-26 02:06:32.000000 moftransformer-1.1.3/moftransformer/modules/heads.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11246 2023-04-25 05:00:17.000000 moftransformer-1.1.3/moftransformer/modules/module.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7329 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/modules/module_utils.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7934 2023-04-25 04:35:31.000000 moftransformer-1.1.3/moftransformer/modules/objectives.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12841 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/modules/vision_transformer_3d.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11715 2023-04-07 05:19:12.000000 moftransformer-1.1.3/moftransformer/run.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.306906 moftransformer-1.1.3/moftransformer/utils/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      210 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/utils/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5316 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/utils/download.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3705 2023-02-13 06:37:39.000000 moftransformer-1.1.3/moftransformer/utils/install_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15554 2023-04-25 04:35:31.000000 moftransformer-1.1.3/moftransformer/utils/prepare_data.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2449 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/utils/validation.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.306906 moftransformer-1.1.3/moftransformer/visualize/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       98 2023-03-09 07:32:31.000000 moftransformer-1.1.3/moftransformer/visualize/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3887 2022-12-19 08:03:14.000000 moftransformer-1.1.3/moftransformer/visualize/drawer.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3628 2023-03-09 07:32:31.000000 moftransformer-1.1.3/moftransformer/visualize/setting.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9107 2023-04-10 08:03:54.000000 moftransformer-1.1.3/moftransformer/visualize/utils.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26335 2023-03-09 07:32:31.000000 moftransformer-1.1.3/moftransformer/visualize/visualizer.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-25 05:16:40.262907 moftransformer-1.1.3/moftransformer.egg-info/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8389 2023-04-25 05:16:40.000000 moftransformer-1.1.3/moftransformer.egg-info/PKG-INFO
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13237 2023-04-25 05:16:40.000000 moftransformer-1.1.3/moftransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        1 2023-04-25 05:16:40.000000 moftransformer-1.1.3/moftransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       64 2023-04-25 05:16:40.000000 moftransformer-1.1.3/moftransformer.egg-info/entry_points.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      321 2023-04-25 05:16:40.000000 moftransformer-1.1.3/moftransformer.egg-info/requires.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       15 2023-04-25 05:16:40.000000 moftransformer-1.1.3/moftransformer.egg-info/top_level.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       38 2023-04-25 05:16:40.306906 moftransformer-1.1.3/setup.cfg
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1548 2022-12-19 08:03:14.000000 moftransformer-1.1.3/setup.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8153 2023-04-27 12:01:12.629117 moftransformer-2.0.0/PKG-INFO
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7775 2023-04-27 05:35:23.000000 moftransformer-2.0.0/README.md
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      398 2023-04-27 11:58:33.000000 moftransformer-2.0.0/moftransformer/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/assets/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       72 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/assets/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12616 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/assets/bbs.json
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8140 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/assets/colors.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12647 2023-01-26 02:06:32.000000 moftransformer-2.0.0/moftransformer/assets/topology.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/cli/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       31 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/cli/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2443 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/cli/download.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      324 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/cli/install_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3040 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/cli/main.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      576 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/cli/run.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      328 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/cli/uninstall_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3427 2023-04-27 11:43:43.000000 moftransformer-2.0.0/moftransformer/config.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10515 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/config_ex.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/database/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      633 2023-04-27 04:48:37.000000 moftransformer-2.0.0/moftransformer/database/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/datamodules/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      210 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/datamodules/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2938 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/datamodules/datamodule.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10088 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/datamodules/dataset.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/examples/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      477 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/examples/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/examples/dataset/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.621117 moftransformer-2.0.0/moftransformer/examples/dataset/test/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/acs+N270+E33.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/acs+N270+E33.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/acs+N270+E33.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/acs+N270+E33.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/smm+N577+E166.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/smm+N577+E166.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/smm+N577+E166.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-04-04 13:23:21.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test/smm+N577+E166.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       73 2023-04-04 13:24:22.000000 moftransformer-2.0.0/moftransformer/examples/dataset/test_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.621117 moftransformer-2.0.0/moftransformer/examples/dataset/total/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-01-05 12:09:32.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/acs+N270+E33.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-01-05 12:09:32.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/acs+N270+E33.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:32.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/acs+N270+E33.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:32.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/acs+N270+E33.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/fee+N254+E185.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/fee+N254+E185.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/fee+N254+E185.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/fee+N254+E185.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mok+N109+E146.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mok+N109+E146.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mok+N109+E146.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:28.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mok+N109+E146.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/msp+N624+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/msp+N624+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/msp+N624+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/sml+N696+E182.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/sml+N696+E182.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/sml+N696+E182.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:31.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/sml+N696+E182.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/smm+N577+E166.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/smm+N577+E166.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/smm+N577+E166.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/smm+N577+E166.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/ukg+N387+E203.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/ukg+N387+E203.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:29.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vmk+N489+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vmk+N489+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-01-05 12:09:30.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vna+N650+E120.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-01-05 12:09:30.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vna+N650+E120.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:30.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vna+N650+E120.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:30.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/vna+N650+E120.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:33.000000 moftransformer-2.0.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.625117 moftransformer-2.0.0/moftransformer/examples/dataset/train/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/fee+N254+E185.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/fee+N254+E185.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/fee+N254+E185.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/fee+N254+E185.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mok+N109+E146.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mok+N109+E146.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mok+N109+E146.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mok+N109+E146.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/msp+N624+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/msp+N624+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/msp+N624+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/sml+N696+E182.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/sml+N696+E182.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/sml+N696+E182.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/sml+N696+E182.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/ukg+N387+E203.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/ukg+N387+E203.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vmk+N489+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vmk+N489+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vna+N650+E120.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vna+N650+E120.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vna+N650+E120.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/vna+N650+E120.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      206 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/train_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.625117 moftransformer-2.0.0/moftransformer/examples/dataset/val/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/acs+N270+E33.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/acs+N270+E33.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/acs+N270+E33.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/acs+N270+E33.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/smm+N577+E166.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/smm+N577+E166.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/smm+N577+E166.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val/smm+N577+E166.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       43 2023-01-05 12:09:34.000000 moftransformer-2.0.0/moftransformer/examples/dataset/val_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.625117 moftransformer-2.0.0/moftransformer/examples/raw/
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7496 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/acs+N270+E33.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    17441 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9738 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/fee+N254+E185.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11392 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/mok+N109+E146.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    30404 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18345 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/raw_example.json
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11939 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/sml+N696+E182.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    24953 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/smm+N577+E166.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    28256 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/ukg+N387+E203.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    39904 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/vmk+N489+E8.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18930 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/vna+N650+E120.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    48803 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/raw/zzz+N96+N373+E34.cif
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/examples/visualize/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.625117 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.625117 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9162 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12083 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6405 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8339 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7074 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9292 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    98728 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6419 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8357 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    93472 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6410 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8347 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6845 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8961 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   170530 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      164 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.625117 moftransformer-2.0.0/moftransformer/gadgets/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       77 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/gadgets/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1806 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/gadgets/my_metrics.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer/libs/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/moftransformer/libs/GRIDAY/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2799 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/AtomTypeMap.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      654 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/AtomTypeMap.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    41808 2022-12-19 08:32:53.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/AtomTypeMap.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2448 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Cell.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7789 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      414 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    33448 2022-12-19 08:32:54.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54588 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18619 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3812 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   143440 2022-12-19 08:32:55.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.o
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4751 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/UFF_FF.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      845 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/UFF_Type.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      202 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/Zeolite_FF.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      190 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      318 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_Si.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       26 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/Zeolite_Type.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7197 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ForceField.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      866 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ForceField.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    67552 2022-12-19 08:32:55.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ForceField.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13991 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      865 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    57152 2022-12-19 08:32:56.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/FourierAnalyzer.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7362 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Framework.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1197 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Framework.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    47328 2022-12-19 08:32:57.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Framework.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3007 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Gaussian.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Gaussian.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15032 2022-12-19 08:32:57.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Gaussian.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9534 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridMaker.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      936 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridMaker.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    80288 2022-12-19 08:32:58.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridMaker.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      320 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Griday.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      948 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayException.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      669 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayException.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15752 2022-12-19 08:32:58.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayException.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      567 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayTypes.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4380 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/LennardJones.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/LennardJones.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    14896 2022-12-19 08:32:58.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/LennardJones.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      334 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Makefile
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    21824 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/MaterialGrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2366 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/MaterialGrid.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    75600 2022-12-19 08:32:59.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/MaterialGrid.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5664 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/NlistMaker.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      922 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/NlistMaker.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    65096 2022-12-19 08:32:59.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/NlistMaker.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      730 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/PairEnergy.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      570 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Random.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5106 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ShiftedLJ.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      764 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ShiftedLJ.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15360 2022-12-19 08:33:00.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/ShiftedLJ.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      811 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Timer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2277 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/Vector.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   698550 2022-12-19 08:33:00.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/libgriday.a
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      563 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/Makefile
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5834 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2022-12-19 08:33:06.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/grid2COTA
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   278928 2022-12-19 08:33:05.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/grid2props
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2022-12-19 08:33:04.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/grid2visit
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   161656 2022-12-19 08:33:03.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/grid_gen
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1046 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/main_cota.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1742 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      900 2022-12-19 08:03:14.000000 moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/main_visit.cpp
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/moftransformer/modules/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      122 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/modules/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5783 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/modules/cgcnn.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3255 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/modules/heads.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11518 2023-04-27 06:22:20.000000 moftransformer-2.0.0/moftransformer/modules/module.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7374 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/modules/module_utils.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8004 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/modules/objectives.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12812 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/modules/vision_transformer_3d.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10096 2023-04-27 07:30:12.000000 moftransformer-2.0.0/moftransformer/run.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11715 2023-04-07 05:19:12.000000 moftransformer-2.0.0/moftransformer/run_cp.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/moftransformer/utils/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      242 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/utils/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5552 2023-04-27 04:54:01.000000 moftransformer-2.0.0/moftransformer/utils/download.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3913 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/utils/install_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16072 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/utils/prepare_data.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4355 2023-04-27 11:41:45.000000 moftransformer-2.0.0/moftransformer/utils/validation.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.629117 moftransformer-2.0.0/moftransformer/visualize/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      130 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/visualize/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3994 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/visualize/drawer.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3705 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/visualize/setting.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9201 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/visualize/utils.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    27623 2023-04-26 04:12:45.000000 moftransformer-2.0.0/moftransformer/visualize/visualizer.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-04-27 12:01:12.617117 moftransformer-2.0.0/moftransformer.egg-info/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8153 2023-04-27 12:01:12.000000 moftransformer-2.0.0/moftransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13262 2023-04-27 12:01:12.000000 moftransformer-2.0.0/moftransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        1 2023-04-27 12:01:12.000000 moftransformer-2.0.0/moftransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       64 2023-04-27 12:01:12.000000 moftransformer-2.0.0/moftransformer.egg-info/entry_points.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      321 2023-04-27 12:01:12.000000 moftransformer-2.0.0/moftransformer.egg-info/requires.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       15 2023-04-27 12:01:12.000000 moftransformer-2.0.0/moftransformer.egg-info/top_level.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       38 2023-04-27 12:01:12.629117 moftransformer-2.0.0/setup.cfg
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1654 2023-04-27 05:16:55.000000 moftransformer-2.0.0/setup.py
```

### Comparing `moftransformer-1.1.3/PKG-INFO` & `moftransformer-2.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,151 +1,113 @@
 Metadata-Version: 2.1
 Name: moftransformer
-Version: 1.1.3
+Version: 2.0.0
 Summary: moftransformer
 Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer
 Author: Yeonghun Kang, Hyunsoo Park
 Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v1.1.3-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.0.0-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v1.1.3-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.0.0-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
- <a href="https://doi.org/10.1038/s42256-023-00628-2">
+ <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
  <a href="https://pypi.org/project/moftransformer/">
      <img alt="Lincense" src="https://img.shields.io/badge/License-MIT-lightgrey.svg?style=plastic">
  </a>
 </p>
 
-# [MOFTransformer](https://hspark1212.github.io/MOFTransformer/index.html)
+# [PMTransformer (MOFTransformer)](https://hspark1212.github.io/MOFTransformer/index.html)
 
- This package provides universal transfer learing for metal-organic frameworks(MOFs) to construct structure-property relationships. `MOFTransformer` obtains state-of-the-art performance to predict accross various properties that include gas adsorption, diffusion, electronic properties regardless of gas types. Beyond its universal transfer learning capabilityies, it provides feature importance analysis from its attentions scores to capture chemical intution.
+ This package provides a universal transfer learning model, `PMTransformer` (Porous Materials Transformer), which obtains the state-of-the-art performance in predicting various properties of porous materials. The PMTRansformer was pre-trainied with 1.9 million hypothetical porous materials including Metal-Organic Frameworks (MOFs), Covalent-Organic Frameworks (COFs), Porous Polymer Networks (PPNs), and zeolites. By fine-tuning the pre-trained `PMTransformer`, you can easily obtain machine learning models to accurately predict various properties of porous materials .
+ 
+ NOTE: From version 2.0.0, the default pre-training model has been changed from `MOFTransformer` to `PMTransformer`, which was pre-trained with a larger dataset, containing other porous materials as well as MOFs. The `PMTransformer` outperforms the `MOFTransformer` in predicting various properties of porous materials.
 
 ## [Install](https://hspark1212.github.io/MOFTransformer/installation.html)
 
-### OS and hardware requirements
-The package development version is tested on following systems:
-
-Linux : Ubuntu 20.04, 22.04
-
-For optimal performance, we recommend running with GPUs
-
 ### Depedencies
 ```
 python>=3.8
 ```
-Given that MOFTransformer is based on pytorch, please install pytorch (>= 1.10.0) according to your environments.
+Given that MOFTransformer is based on pytorch, please install pytorch (>= 1.12.0) according to your environments.
 
 ### Installation using PIP 
 ```
 $ pip install moftransformer
 ```
-which should install in about 50 seconds.
 
-### Download the pretrained model (ckpt file)
-- you can download the pretrained model with 1 M hMOFs in [figshare](https://figshare.com/articles/dataset/MOFTransformer/21155506)
+### Download the pretrained models (ckpt file)
+- you can download the pretrained models (`PMTransformer.ckpt` and `MOFTransformer.ckpt`) [figshare](https://figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2)
+
 or you can download with a command line:
 ```
 $ moftransformer download pretrain_model
 ```
-### (Optional) Download dataset for CoREMOF, QMOF
-- we've provide the dataset of MOFTransformer (i.e., atom-based graph embeddings and energy-grid embeddings) for CoREMOF, QMOF
+### (Optional) Download pre-embeddings for CoREMOF, QMOF
+- we've provide the pre-embeddings (i.e., atom-based graph embeddings and energy-grid embeddings), inputs of `PMTransformer`, for CoREMOF, QMOF database.
 ```
 $ moftransformer download coremof
 $ moftransformer download qmof
 ```
 
 ## [Getting Started](https://hspark1212.github.io/MOFTransformer/tutorial.html)
-
-1. At first, you can run `prepare_data` with 10 cifs in `moftransformer/examples/raw` directory.
-
-In order to run `prepare_data`, you need to install `GRIDAY` to calculate energy grid.
-You can download GRIDAY using command-line.
-
-```bash
-$ moftransformer install-griday
+1. At first, you download dataset of hMOFs (20,000 MOFs) as an example.
 ```
-
-Example for running `prepare-data`
-
-```python
-from moftransformer.examples import example_path
-from moftransformer.utils import prepare_data
-
-# Get example path
-root_cifs = example_path['root_cif']
-root_dataset = example_path['root_dataset']
-downstream = example_path['downstream']
-
-train_fraction = 0.7
-test_fraction = 0.2
-
-# Run prepare data
-prepare_data(root_cifs, root_dataset, downstream=downstream, 
-             train_fraciton=train_fraction, test_fraciton=test_fraction)
+$ moftransformer download hmof
 ```
-
 2. Fine-tune the pretrained MOFTransformer.
 ```python
 import moftransformer
 from moftransformer.examples import example_path
 
 # data root and downstream from example
-root_dataset = example_path['root_dataset']
+data_root = example_path['data_root']
 downstream = example_path['downstream']
 log_dir = './logs/'
+# load_path = "pmtransformer" (default)
 
-# kwargs (optional)
-max_epochs = 10
-batch_size = 8
-
-moftransformer.run(root_dataset, downstream, log_dir=log_dir, 
+moftransformer.run(data_root, downstream, log_dir=log_dir, 
                    max_epochs=max_epochs, batch_size=batch_size,)
 ```
-which will run in about 35 seconds.
-
-
 3. Visualize analysis of feature importance for the fine-tuned model.
-
-download finetuned-bandgap model before visualize.
-```bash
-moftransformer download finetuned_model -o ./examples
-```
-
 ```python
 %matplotlib widget
-from moftransformer.visualize import PatchVisualizer
-from moftransformer.examples import visualize_example_path
+from visualize import PatchVisualizer
 
 model_path = "examples/finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt'
-data_path = visualize_example_path
+data_path = 'examples/visualize/dataset/'
 cifname = 'MIBQAR01_FSR'
 
 vis = PatchVisualizer.from_cifname(cifname, model_path, data_path)
 vis.draw_graph() # or vis.draw_grid()
 ```
 
 ## [Architecture](https://hspark1212.github.io/MOFTransformer/introduction.html)
-`MOFTransformer`is a multi-modal Transformer pre-trained with 1 million hypothetical MOFs so that it efficiently capture both local and global feeatures of MOFs.
+It is a multi-modal pre-training Transformer encoder which is designed to capture both local and global features of porous materials. 
 
-- `MOFformer` takes two different representations as input
+The pre-traning tasks are as follows:
+(1) Topology Prediction
+(2) Void Fraction Prediction
+(3) Building Block Classification
+ 
+It takes two different representations as input
   - Atom-based Graph Embedding : CGCNN w/o pooling layer -> local features
   - Energy-grid Embedding : 1D flatten patches of 3D energy grid -> global features
   
 <p align="center">
   <img src="https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig2.jpg" width="700")
 </p>
 
@@ -163,32 +125,38 @@
 vis.draw_graph()
 ```
 <p align="center">
 <img src="https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/getting_started/assets/1.gif" width="400">
 </p>
 
 ```python
+vis = PatchVisualizer.from_cifname(cifname, model_path, data_path)
 vis.draw_grid()
 ```
 <p align="center">
 <img src="https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/getting_started/assets/3.gif" width="400">
 </p>
 
 ## Universal Transfer Learning
-| Property                                 | MOFTransformer | Original Paper | Number of Data | Remarks          | Reference |
-|------------------------------------------|----------------|----------------|----------------|------------------|-----------|
-|N<sub>2</sub> uptake                     | R2: 0.78       | R2: 0.71       | 5,286          | CoRE MOF         | 1         |
-|O<sub>2</sub> uptake                     | R2: 0.83       | R2: 0.74       | 5,286          | CoRE MOF         | 1         |
-|N<sub>2</sub> diffusivity                | R2: 0.77       | R2: 0.76       | 5,286          | CoRE MOF         | 1         |
-|O<sub>2</sub> diffusivity                | R2: 0.78       | R2: 0.74       | 5,286          | CoRE MOF         | 1         |
-|CO<sub>2</sub> Henry coefficient         | MAE : 0.30     | MAE : 0.42     | 8,183          | CoRE MOF         | 2         |
-|Solvent removal stability classification | ACC : 0.76     | ACC : 0.76     | 2,148          | Text-mining data | 3         |
-|Thermal stability regression             | R2 : 0.44      | R2 : 0.46      | 3,098          | Text-mining data | 3         |
-### Reference
-1. [Prediction of O2/N2 Selectivity in Metal−Organic Frameworks via High-Throughput Computational Screening and Machine Learning](https://pubs.acs.org/doi/abs/10.1021/acsami.1c18521)
-2. [Understanding the diversity of the metal-organic framework ecosystem](https://www.nature.com/articles/s41467-020-17755-8)
-3. [Using Machine Learning and Data Mining to Leverage Community Knowledge for the Engineering of Stable Metal–Organic Frameworks](https://pubs.acs.org/doi/10.1021/jacs.1c07217)
 
-## Citation
-If you want to cite the MOFTransformer and the pre-training and fine-tuning dataset, please refer to the publication:
+Comparison of mean absolute error (MAE) values for various baseline models, scratch, MOFTransformer, and PMTransformer on different properties of MOFs, COFs, PPNs, and zeolites. The bold values indicate the lowest MAE value for each property. The details of information can be found in [PMTransformer paper]()
+
+| Material | Property | Number of Dataset | Energy histogram | Descriptor-based ML | CGCNN | Scratch | MOFTransformer | PMTransformer |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| MOF | H<sub>2</sub> Uptake (100 bar) | 20,000 | 9.183 | 9.456 | 32.864 | 7.018 | 6.377 | **5.963** |
+| MOF | H<sub>2</sub> diffusivity (dilute) | 20,000 | 0.644 | 0.398 | 0.6600 | 0.391 | 0.367 | 0.**366** |
+| MOF | Band-gap | 20.373 | 0.913 | 0.590 | 0.290 | 0.271 | 0.224 | **0.216** |
+| MOF | N<sub>2</sub> uptake (1 bar) | 5,286 | 0.178 | 0.115 | 0.108 | 0.102 | 0.071 | **0.069** |
+| MOF | O<sub>2</sub> uptake (1 bar) | 5,286 | 0.162 | 0.076 | 0.083 | 0.071 | **0.051** | 0.053 |
+| MOF | N<sub>2</sub> diffusivity (1 bar) | 5,286 | 7.82e-5 | 5.22e-5 | 7.19e-5 | 5.82e-05 | **4.52e-05** | 4.53e-05 |
+| MOF | O<sub>2</sub> diffusivity (1 bar) | 5,286 | 7.14e-5 | 4.59e-5 | 6.56e-5 | 5.00e-05 | 4.04e-05 | **3.99e-05** |
+| MOF | CO<sub>2</sub> Henry coefficient | 8,183 | 0.737 | 0.468 | 0.426 | 0.362 | 0.295 | **0.288** |
+| MOF | Thermal stability | 3,098 | 68.74 | 49.27 | 52.38 | 52.557 | 45.875 | **45.766** |
+| COF | CH<sub>4</sub> uptake (65bar) | 39,304 | 5.588 | 4.630 | 15.31 | 2.883 | 2.268 | **2.126** |
+| COF | CH<sub>4</sub> uptake (5.8bar) | 39,304 | 3.444 | 1.853 | 5.620 | 1.255 | **0.999** | 1.009 | 
+| COF | CO<sub>2</sub> heat of adsorption | 39,304 | 2.101 | 1.341 | 1.846 | 1.058 | 0.874 | **0.842** |
+| COF | CO<sub>2</sub> log KH | 39,304 | 0.242 | 0.169 | 0.238 | 0.134 | 0.108 | **0.103** |
+| PPN | CH<sub>4</sub> uptake (65bar) | 17,870 | 6.260 | 4.233 | 9.731 | 3.748 | 3.187 | **2.995** | 
+| PPN | CH<sub>4</sub> uptake (1bar) | 17,870  | 1.356	| 0.563	| 1.525	| 0.602	| 0.493	| **0.461** | 
+| Zeolite | CH<sub>4</sub>  KH (unitless) | 99,204	| 8.032	| 6.268	| 6.334	| 4.286	| 4.103	| **3.998** |
+| Zeolite | CH<sub>4</sub>  Heat of adsorption | 99,204	| 1.612	|1.033	| 1.603	| 0.670	| 0.647	|**0.639** |
 
-Y. Kang, H. Park, B. Smit, J. Kim. "A multi-modal pre-training transformer for universal transfer learning in metal–organic frameworks", *Nature Machine Intelligence*, **(2023)** DOI: [https://doi.org/10.1038/s42256-023-00628-2](https://doi.org/10.1038/s42256-023-00628-2)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1 Name: moftransformer Version: 1.1.3 Summary:
+Metadata-Version: 2.1 Name: moftransformer Version: 2.0.0 Summary:
 moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
 Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
 docs/source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
-# [MOFTransformer](https://hspark1212.github.io/MOFTransformer/index.html) This
-package provides universal transfer learing for metal-organic frameworks(MOFs)
-to construct structure-property relationships. `MOFTransformer` obtains state-
-of-the-art performance to predict accross various properties that include gas
-adsorption, diffusion, electronic properties regardless of gas types. Beyond
-its universal transfer learning capabilityies, it provides feature importance
-analysis from its attentions scores to capture chemical intution. ## [Install]
-(https://hspark1212.github.io/MOFTransformer/installation.html) ### OS and
-hardware requirements The package development version is tested on following
-systems: Linux : Ubuntu 20.04, 22.04 For optimal performance, we recommend
-running with GPUs ### Depedencies ``` python>=3.8 ``` Given that MOFTransformer
-is based on pytorch, please install pytorch (>= 1.10.0) according to your
-environments. ### Installation using PIP ``` $ pip install moftransformer ```
-which should install in about 50 seconds. ### Download the pretrained model
-(ckpt file) - you can download the pretrained model with 1 M hMOFs in
-[figshare](https://figshare.com/articles/dataset/MOFTransformer/21155506) or
+# [PMTransformer (MOFTransformer)](https://hspark1212.github.io/MOFTransformer/
+index.html) This package provides a universal transfer learning model,
+`PMTransformer` (Porous Materials Transformer), which obtains the state-of-the-
+art performance in predicting various properties of porous materials. The
+PMTRansformer was pre-trainied with 1.9 million hypothetical porous materials
+including Metal-Organic Frameworks (MOFs), Covalent-Organic Frameworks (COFs),
+Porous Polymer Networks (PPNs), and zeolites. By fine-tuning the pre-trained
+`PMTransformer`, you can easily obtain machine learning models to accurately
+predict various properties of porous materials . NOTE: From version 2.0.0, the
+default pre-training model has been changed from `MOFTransformer` to
+`PMTransformer`, which was pre-trained with a larger dataset, containing other
+porous materials as well as MOFs. The `PMTransformer` outperforms the
+`MOFTransformer` in predicting various properties of porous materials. ##
+[Install](https://hspark1212.github.io/MOFTransformer/installation.html) ###
+Depedencies ``` python>=3.8 ``` Given that MOFTransformer is based on pytorch,
+please install pytorch (>= 1.12.0) according to your environments. ###
+Installation using PIP ``` $ pip install moftransformer ``` ### Download the
+pretrained models (ckpt file) - you can download the pretrained models
+(`PMTransformer.ckpt` and `MOFTransformer.ckpt`) [figshare](https://
+figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2) or
 you can download with a command line: ``` $ moftransformer download
-pretrain_model ``` ### (Optional) Download dataset for CoREMOF, QMOF - we've
-provide the dataset of MOFTransformer (i.e., atom-based graph embeddings and
-energy-grid embeddings) for CoREMOF, QMOF ``` $ moftransformer download coremof
-$ moftransformer download qmof ``` ## [Getting Started](https://
-hspark1212.github.io/MOFTransformer/tutorial.html) 1. At first, you can run
-`prepare_data` with 10 cifs in `moftransformer/examples/raw` directory. In
-order to run `prepare_data`, you need to install `GRIDAY` to calculate energy
-grid. You can download GRIDAY using command-line. ```bash $ moftransformer
-install-griday ``` Example for running `prepare-data` ```python from
-moftransformer.examples import example_path from moftransformer.utils import
-prepare_data # Get example path root_cifs = example_path['root_cif']
-root_dataset = example_path['root_dataset'] downstream = example_path
-['downstream'] train_fraction = 0.7 test_fraction = 0.2 # Run prepare data
-prepare_data(root_cifs, root_dataset, downstream=downstream,
-train_fraciton=train_fraction, test_fraciton=test_fraction) ``` 2. Fine-tune
-the pretrained MOFTransformer. ```python import moftransformer from
-moftransformer.examples import example_path # data root and downstream from
-example root_dataset = example_path['root_dataset'] downstream = example_path
-['downstream'] log_dir = './logs/' # kwargs (optional) max_epochs = 10
-batch_size = 8 moftransformer.run(root_dataset, downstream, log_dir=log_dir,
-max_epochs=max_epochs, batch_size=batch_size,) ``` which will run in about 35
-seconds. 3. Visualize analysis of feature importance for the fine-tuned model.
-download finetuned-bandgap model before visualize. ```bash moftransformer
-download finetuned_model -o ./examples ``` ```python %matplotlib widget from
-moftransformer.visualize import PatchVisualizer from moftransformer.examples
-import visualize_example_path model_path = "examples/finetuned_bandgap.ckpt" #
-or 'examples/finetuned_h2_uptake.ckpt' data_path = visualize_example_path
-cifname = 'MIBQAR01_FSR' vis = PatchVisualizer.from_cifname(cifname,
-model_path, data_path) vis.draw_graph() # or vis.draw_grid() ``` ##
-[Architecture](https://hspark1212.github.io/MOFTransformer/introduction.html)
-`MOFTransformer`is a multi-modal Transformer pre-trained with 1 million
-hypothetical MOFs so that it efficiently capture both local and global
-feeatures of MOFs. - `MOFformer` takes two different representations as input -
-Atom-based Graph Embedding : CGCNN w/o pooling layer -> local features -
-Energy-grid Embedding : 1D flatten patches of 3D energy grid -> global features
+pretrain_model ``` ### (Optional) Download pre-embeddings for CoREMOF, QMOF -
+we've provide the pre-embeddings (i.e., atom-based graph embeddings and energy-
+grid embeddings), inputs of `PMTransformer`, for CoREMOF, QMOF database. ``` $
+moftransformer download coremof $ moftransformer download qmof ``` ## [Getting
+Started](https://hspark1212.github.io/MOFTransformer/tutorial.html) 1. At
+first, you download dataset of hMOFs (20,000 MOFs) as an example. ``` $
+moftransformer download hmof ``` 2. Fine-tune the pretrained MOFTransformer.
+```python import moftransformer from moftransformer.examples import
+example_path # data root and downstream from example data_root = example_path
+['data_root'] downstream = example_path['downstream'] log_dir = './logs/' #
+load_path = "pmtransformer" (default) moftransformer.run(data_root, downstream,
+log_dir=log_dir, max_epochs=max_epochs, batch_size=batch_size,) ``` 3.
+Visualize analysis of feature importance for the fine-tuned model. ```python
+%matplotlib widget from visualize import PatchVisualizer model_path =
+"examples/finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt'
+data_path = 'examples/visualize/dataset/' cifname = 'MIBQAR01_FSR' vis =
+PatchVisualizer.from_cifname(cifname, model_path, data_path) vis.draw_graph() #
+or vis.draw_grid() ``` ## [Architecture](https://hspark1212.github.io/
+MOFTransformer/introduction.html) It is a multi-modal pre-training Transformer
+encoder which is designed to capture both local and global features of porous
+materials. The pre-traning tasks are as follows: (1) Topology Prediction (2)
+Void Fraction Prediction (3) Building Block Classification It takes two
+different representations as input - Atom-based Graph Embedding : CGCNN w/
+o pooling layer -> local features - Energy-grid Embedding : 1D flatten patches
+of 3D energy grid -> global features
 ## [Feature Importance Anaylsis](https://hspark1212.github.io/MOFTransformer/
 getting_started/visualization.html) you can easily visualize feature importance
 analysis of atom-based graph embeddings and energy-grid embeddings. ```python
 %matplotlib widget from visualize import PatchVisualizer model_path =
 "examples/finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt'
 data_path = 'examples/visualize/dataset/' cifname = 'MIBQAR01_FSR' vis =
 PatchVisualizer.from_cifname(cifname, model_path, data_path) vis.draw_graph()
 ```
    [https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/
                      source/getting_started/assets/1.gif]
-```python vis.draw_grid() ```
+```python vis = PatchVisualizer.from_cifname(cifname, model_path, data_path)
+vis.draw_grid() ```
    [https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/
                      source/getting_started/assets/3.gif]
-## Universal Transfer Learning | Property | MOFTransformer | Original Paper |
-Number of Data | Remarks | Reference | |---------------------------------------
----|----------------|----------------|----------------|------------------|-----
-------| |N2 uptake | R2: 0.78 | R2: 0.71 | 5,286 | CoRE MOF | 1 | |O2 uptake |
-R2: 0.83 | R2: 0.74 | 5,286 | CoRE MOF | 1 | |N2 diffusivity | R2: 0.77 | R2:
-0.76 | 5,286 | CoRE MOF | 1 | |O2 diffusivity | R2: 0.78 | R2: 0.74 | 5,286 |
-CoRE MOF | 1 | |CO2 Henry coefficient | MAE : 0.30 | MAE : 0.42 | 8,183 | CoRE
-MOF | 2 | |Solvent removal stability classification | ACC : 0.76 | ACC : 0.76 |
-2,148 | Text-mining data | 3 | |Thermal stability regression | R2 : 0.44 | R2 :
-0.46 | 3,098 | Text-mining data | 3 | ### Reference 1. [Prediction of O2/N2
-Selectivity in MetalâOrganic Frameworks via High-Throughput Computational
-Screening and Machine Learning](https://pubs.acs.org/doi/abs/10.1021/
-acsami.1c18521) 2. [Understanding the diversity of the metal-organic framework
-ecosystem](https://www.nature.com/articles/s41467-020-17755-8) 3. [Using
-Machine Learning and Data Mining to Leverage Community Knowledge for the
-Engineering of Stable MetalâOrganic Frameworks](https://pubs.acs.org/doi/
-10.1021/jacs.1c07217) ## Citation If you want to cite the MOFTransformer and
-the pre-training and fine-tuning dataset, please refer to the publication: Y.
-Kang, H. Park, B. Smit, J. Kim. "A multi-modal pre-training transformer for
-universal transfer learning in metalâorganic frameworks", *Nature Machine
-Intelligence*, **(2023)** DOI: [https://doi.org/10.1038/s42256-023-00628-2]
-(https://doi.org/10.1038/s42256-023-00628-2)
+## Universal Transfer Learning Comparison of mean absolute error (MAE) values
+for various baseline models, scratch, MOFTransformer, and PMTransformer on
+different properties of MOFs, COFs, PPNs, and zeolites. The bold values
+indicate the lowest MAE value for each property. The details of information can
+be found in [PMTransformer paper]() | Material | Property | Number of Dataset |
+Energy histogram | Descriptor-based ML | CGCNN | Scratch | MOFTransformer |
+PMTransformer | | --- | --- | --- | --- | --- | --- | --- | --- | --- | | MOF |
+H2 Uptake (100 bar) | 20,000 | 9.183 | 9.456 | 32.864 | 7.018 | 6.377 |
+**5.963** | | MOF | H2 diffusivity (dilute) | 20,000 | 0.644 | 0.398 | 0.6600 |
+0.391 | 0.367 | 0.**366** | | MOF | Band-gap | 20.373 | 0.913 | 0.590 | 0.290 |
+0.271 | 0.224 | **0.216** | | MOF | N2 uptake (1 bar) | 5,286 | 0.178 | 0.115 |
+0.108 | 0.102 | 0.071 | **0.069** | | MOF | O2 uptake (1 bar) | 5,286 | 0.162 |
+0.076 | 0.083 | 0.071 | **0.051** | 0.053 | | MOF | N2 diffusivity (1 bar) |
+5,286 | 7.82e-5 | 5.22e-5 | 7.19e-5 | 5.82e-05 | **4.52e-05** | 4.53e-05 | |
+MOF | O2 diffusivity (1 bar) | 5,286 | 7.14e-5 | 4.59e-5 | 6.56e-5 | 5.00e-05 |
+4.04e-05 | **3.99e-05** | | MOF | CO2 Henry coefficient | 8,183 | 0.737 | 0.468
+| 0.426 | 0.362 | 0.295 | **0.288** | | MOF | Thermal stability | 3,098 | 68.74
+| 49.27 | 52.38 | 52.557 | 45.875 | **45.766** | | COF | CH4 uptake (65bar) |
+39,304 | 5.588 | 4.630 | 15.31 | 2.883 | 2.268 | **2.126** | | COF | CH4 uptake
+(5.8bar) | 39,304 | 3.444 | 1.853 | 5.620 | 1.255 | **0.999** | 1.009 | | COF |
+CO2 heat of adsorption | 39,304 | 2.101 | 1.341 | 1.846 | 1.058 | 0.874 |
+**0.842** | | COF | CO2 log KH | 39,304 | 0.242 | 0.169 | 0.238 | 0.134 | 0.108
+| **0.103** | | PPN | CH4 uptake (65bar) | 17,870 | 6.260 | 4.233 | 9.731 |
+3.748 | 3.187 | **2.995** | | PPN | CH4 uptake (1bar) | 17,870 | 1.356 | 0.563
+| 1.525 | 0.602 | 0.493 | **0.461** | | Zeolite | CH4 KH (unitless) | 99,204 |
+8.032 | 6.268 | 6.334 | 4.286 | 4.103 | **3.998** | | Zeolite | CH4 Heat of
+adsorption | 99,204 | 1.612 |1.033 | 1.603 | 0.670 | 0.647 |**0.639** |
```

### Comparing `moftransformer-1.1.3/moftransformer/assets/bbs.json` & `moftransformer-2.0.0/moftransformer/assets/bbs.json`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/assets/colors.py` & `moftransformer-2.0.0/moftransformer/assets/colors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,223 +1,229 @@
+# MOFTransformer version 2.0.0
 # flake8: noqa
 import numpy as np
 
 # Jmol colors.  See: http://jmol.sourceforge.net/jscolors/#color_U
-jmol_colors = np.array([(1.000, 0.000, 0.000),  # None
-                        (1.000, 1.000, 1.000),  # H
-                        (0.851, 1.000, 1.000),  # He
-                        (0.800, 0.502, 1.000),  # Li
-                        (0.761, 1.000, 0.000),  # Be
-                        (1.000, 0.710, 0.710),  # B
-                        (0.565, 0.565, 0.565),  # C
-                        (0.188, 0.314, 0.973),  # N
-                        (1.000, 0.051, 0.051),  # O
-                        (0.565, 0.878, 0.314),  # F
-                        (0.702, 0.890, 0.961),  # Ne
-                        (0.671, 0.361, 0.949),  # Na
-                        (0.541, 1.000, 0.000),  # Mg
-                        (0.749, 0.651, 0.651),  # Al
-                        (0.941, 0.784, 0.627),  # Si
-                        (1.000, 0.502, 0.000),  # P
-                        (1.000, 1.000, 0.188),  # S
-                        (0.122, 0.941, 0.122),  # Cl
-                        (0.502, 0.820, 0.890),  # Ar
-                        (0.561, 0.251, 0.831),  # K
-                        (0.239, 1.000, 0.000),  # Ca
-                        (0.902, 0.902, 0.902),  # Sc
-                        (0.749, 0.761, 0.780),  # Ti
-                        (0.651, 0.651, 0.671),  # V
-                        (0.541, 0.600, 0.780),  # Cr
-                        (0.612, 0.478, 0.780),  # Mn
-                        (0.878, 0.400, 0.200),  # Fe
-                        (0.941, 0.565, 0.627),  # Co
-                        (0.314, 0.816, 0.314),  # Ni
-                        (0.784, 0.502, 0.200),  # Cu
-                        (0.490, 0.502, 0.690),  # Zn
-                        (0.761, 0.561, 0.561),  # Ga
-                        (0.400, 0.561, 0.561),  # Ge
-                        (0.741, 0.502, 0.890),  # As
-                        (1.000, 0.631, 0.000),  # Se
-                        (0.651, 0.161, 0.161),  # Br
-                        (0.361, 0.722, 0.820),  # Kr
-                        (0.439, 0.180, 0.690),  # Rb
-                        (0.000, 1.000, 0.000),  # Sr
-                        (0.580, 1.000, 1.000),  # Y
-                        (0.580, 0.878, 0.878),  # Zr
-                        (0.451, 0.761, 0.788),  # Nb
-                        (0.329, 0.710, 0.710),  # Mo
-                        (0.231, 0.620, 0.620),  # Tc
-                        (0.141, 0.561, 0.561),  # Ru
-                        (0.039, 0.490, 0.549),  # Rh
-                        (0.000, 0.412, 0.522),  # Pd
-                        (0.753, 0.753, 0.753),  # Ag
-                        (1.000, 0.851, 0.561),  # Cd
-                        (0.651, 0.459, 0.451),  # In
-                        (0.400, 0.502, 0.502),  # Sn
-                        (0.620, 0.388, 0.710),  # Sb
-                        (0.831, 0.478, 0.000),  # Te
-                        (0.580, 0.000, 0.580),  # I
-                        (0.259, 0.620, 0.690),  # Xe
-                        (0.341, 0.090, 0.561),  # Cs
-                        (0.000, 0.788, 0.000),  # Ba
-                        (0.439, 0.831, 1.000),  # La
-                        (1.000, 1.000, 0.780),  # Ce
-                        (0.851, 1.000, 0.780),  # Pr
-                        (0.780, 1.000, 0.780),  # Nd
-                        (0.639, 1.000, 0.780),  # Pm
-                        (0.561, 1.000, 0.780),  # Sm
-                        (0.380, 1.000, 0.780),  # Eu
-                        (0.271, 1.000, 0.780),  # Gd
-                        (0.188, 1.000, 0.780),  # Tb
-                        (0.122, 1.000, 0.780),  # Dy
-                        (0.000, 1.000, 0.612),  # Ho
-                        (0.000, 0.902, 0.459),  # Er
-                        (0.000, 0.831, 0.322),  # Tm
-                        (0.000, 0.749, 0.220),  # Yb
-                        (0.000, 0.671, 0.141),  # Lu
-                        (0.302, 0.761, 1.000),  # Hf
-                        (0.302, 0.651, 1.000),  # Ta
-                        (0.129, 0.580, 0.839),  # W
-                        (0.149, 0.490, 0.671),  # Re
-                        (0.149, 0.400, 0.588),  # Os
-                        (0.090, 0.329, 0.529),  # Ir
-                        (0.816, 0.816, 0.878),  # Pt
-                        (1.000, 0.820, 0.137),  # Au
-                        (0.722, 0.722, 0.816),  # Hg
-                        (0.651, 0.329, 0.302),  # Tl
-                        (0.341, 0.349, 0.380),  # Pb
-                        (0.620, 0.310, 0.710),  # Bi
-                        (0.671, 0.361, 0.000),  # Po
-                        (0.459, 0.310, 0.271),  # At
-                        (0.259, 0.510, 0.588),  # Rn
-                        (0.259, 0.000, 0.400),  # Fr
-                        (0.000, 0.490, 0.000),  # Ra
-                        (0.439, 0.671, 0.980),  # Ac
-                        (0.000, 0.729, 1.000),  # Th
-                        (0.000, 0.631, 1.000),  # Pa
-                        (0.000, 0.561, 1.000),  # U
-                        (0.000, 0.502, 1.000),  # Np
-                        (0.000, 0.420, 1.000),  # Pu
-                        (0.329, 0.361, 0.949),  # Am
-                        (0.471, 0.361, 0.890),  # Cm
-                        (0.541, 0.310, 0.890),  # Bk
-                        (0.631, 0.212, 0.831),  # Cf
-                        (0.702, 0.122, 0.831),  # Es
-                        (0.702, 0.122, 0.729),  # Fm
-                        (0.702, 0.051, 0.651),  # Md
-                        (0.741, 0.051, 0.529),  # No
-                        (0.780, 0.000, 0.400),  # Lr
-                        (0.800, 0.000, 0.349),  # Rf
-                        (0.820, 0.000, 0.310),  # Db
-                        (0.851, 0.000, 0.271),  # Sg
-                        (0.878, 0.000, 0.220),  # Bh
-                        (0.902, 0.000, 0.180),  # Hs
-                        (0.922, 0.000, 0.149),  # Mt
-                        ])
+jmol_colors = np.array(
+    [
+        (1.000, 0.000, 0.000),  # None
+        (1.000, 1.000, 1.000),  # H
+        (0.851, 1.000, 1.000),  # He
+        (0.800, 0.502, 1.000),  # Li
+        (0.761, 1.000, 0.000),  # Be
+        (1.000, 0.710, 0.710),  # B
+        (0.565, 0.565, 0.565),  # C
+        (0.188, 0.314, 0.973),  # N
+        (1.000, 0.051, 0.051),  # O
+        (0.565, 0.878, 0.314),  # F
+        (0.702, 0.890, 0.961),  # Ne
+        (0.671, 0.361, 0.949),  # Na
+        (0.541, 1.000, 0.000),  # Mg
+        (0.749, 0.651, 0.651),  # Al
+        (0.941, 0.784, 0.627),  # Si
+        (1.000, 0.502, 0.000),  # P
+        (1.000, 1.000, 0.188),  # S
+        (0.122, 0.941, 0.122),  # Cl
+        (0.502, 0.820, 0.890),  # Ar
+        (0.561, 0.251, 0.831),  # K
+        (0.239, 1.000, 0.000),  # Ca
+        (0.902, 0.902, 0.902),  # Sc
+        (0.749, 0.761, 0.780),  # Ti
+        (0.651, 0.651, 0.671),  # V
+        (0.541, 0.600, 0.780),  # Cr
+        (0.612, 0.478, 0.780),  # Mn
+        (0.878, 0.400, 0.200),  # Fe
+        (0.941, 0.565, 0.627),  # Co
+        (0.314, 0.816, 0.314),  # Ni
+        (0.784, 0.502, 0.200),  # Cu
+        (0.490, 0.502, 0.690),  # Zn
+        (0.761, 0.561, 0.561),  # Ga
+        (0.400, 0.561, 0.561),  # Ge
+        (0.741, 0.502, 0.890),  # As
+        (1.000, 0.631, 0.000),  # Se
+        (0.651, 0.161, 0.161),  # Br
+        (0.361, 0.722, 0.820),  # Kr
+        (0.439, 0.180, 0.690),  # Rb
+        (0.000, 1.000, 0.000),  # Sr
+        (0.580, 1.000, 1.000),  # Y
+        (0.580, 0.878, 0.878),  # Zr
+        (0.451, 0.761, 0.788),  # Nb
+        (0.329, 0.710, 0.710),  # Mo
+        (0.231, 0.620, 0.620),  # Tc
+        (0.141, 0.561, 0.561),  # Ru
+        (0.039, 0.490, 0.549),  # Rh
+        (0.000, 0.412, 0.522),  # Pd
+        (0.753, 0.753, 0.753),  # Ag
+        (1.000, 0.851, 0.561),  # Cd
+        (0.651, 0.459, 0.451),  # In
+        (0.400, 0.502, 0.502),  # Sn
+        (0.620, 0.388, 0.710),  # Sb
+        (0.831, 0.478, 0.000),  # Te
+        (0.580, 0.000, 0.580),  # I
+        (0.259, 0.620, 0.690),  # Xe
+        (0.341, 0.090, 0.561),  # Cs
+        (0.000, 0.788, 0.000),  # Ba
+        (0.439, 0.831, 1.000),  # La
+        (1.000, 1.000, 0.780),  # Ce
+        (0.851, 1.000, 0.780),  # Pr
+        (0.780, 1.000, 0.780),  # Nd
+        (0.639, 1.000, 0.780),  # Pm
+        (0.561, 1.000, 0.780),  # Sm
+        (0.380, 1.000, 0.780),  # Eu
+        (0.271, 1.000, 0.780),  # Gd
+        (0.188, 1.000, 0.780),  # Tb
+        (0.122, 1.000, 0.780),  # Dy
+        (0.000, 1.000, 0.612),  # Ho
+        (0.000, 0.902, 0.459),  # Er
+        (0.000, 0.831, 0.322),  # Tm
+        (0.000, 0.749, 0.220),  # Yb
+        (0.000, 0.671, 0.141),  # Lu
+        (0.302, 0.761, 1.000),  # Hf
+        (0.302, 0.651, 1.000),  # Ta
+        (0.129, 0.580, 0.839),  # W
+        (0.149, 0.490, 0.671),  # Re
+        (0.149, 0.400, 0.588),  # Os
+        (0.090, 0.329, 0.529),  # Ir
+        (0.816, 0.816, 0.878),  # Pt
+        (1.000, 0.820, 0.137),  # Au
+        (0.722, 0.722, 0.816),  # Hg
+        (0.651, 0.329, 0.302),  # Tl
+        (0.341, 0.349, 0.380),  # Pb
+        (0.620, 0.310, 0.710),  # Bi
+        (0.671, 0.361, 0.000),  # Po
+        (0.459, 0.310, 0.271),  # At
+        (0.259, 0.510, 0.588),  # Rn
+        (0.259, 0.000, 0.400),  # Fr
+        (0.000, 0.490, 0.000),  # Ra
+        (0.439, 0.671, 0.980),  # Ac
+        (0.000, 0.729, 1.000),  # Th
+        (0.000, 0.631, 1.000),  # Pa
+        (0.000, 0.561, 1.000),  # U
+        (0.000, 0.502, 1.000),  # Np
+        (0.000, 0.420, 1.000),  # Pu
+        (0.329, 0.361, 0.949),  # Am
+        (0.471, 0.361, 0.890),  # Cm
+        (0.541, 0.310, 0.890),  # Bk
+        (0.631, 0.212, 0.831),  # Cf
+        (0.702, 0.122, 0.831),  # Es
+        (0.702, 0.122, 0.729),  # Fm
+        (0.702, 0.051, 0.651),  # Md
+        (0.741, 0.051, 0.529),  # No
+        (0.780, 0.000, 0.400),  # Lr
+        (0.800, 0.000, 0.349),  # Rf
+        (0.820, 0.000, 0.310),  # Db
+        (0.851, 0.000, 0.271),  # Sg
+        (0.878, 0.000, 0.220),  # Bh
+        (0.902, 0.000, 0.180),  # Hs
+        (0.922, 0.000, 0.149),  # Mt
+    ]
+)
 
 # CPK colors in units of RGB values:
-cpk_colors = np.array([
-    (1.000, 0.000, 0.000),  # None
-    (1.000, 1.000, 1.000),  # H
-    (1.000, 0.753, 0.796),  # He
-    (0.698, 0.133, 0.133),  # Li
-    (1.000, 0.078, 0.576),  # Be
-    (0.000, 1.000, 0.000),  # B
-    (0.784, 0.784, 0.784),  # C
-    (0.561, 0.561, 1.000),  # N
-    (0.941, 0.000, 0.000),  # O
-    (0.855, 0.647, 0.125),  # F
-    (1.000, 0.078, 0.576),  # Ne
-    (0.000, 0.000, 1.000),  # Na
-    (0.133, 0.545, 0.133),  # Mg
-    (0.502, 0.502, 0.565),  # Al
-    (0.855, 0.647, 0.125),  # Si
-    (1.000, 0.647, 0.000),  # P
-    (1.000, 0.784, 0.196),  # S
-    (0.000, 1.000, 0.000),  # Cl
-    (1.000, 0.078, 0.576),  # Ar
-    (1.000, 0.078, 0.576),  # K
-    (0.502, 0.502, 0.565),  # Ca
-    (1.000, 0.078, 0.576),  # Sc
-    (0.502, 0.502, 0.565),  # Ti
-    (1.000, 0.078, 0.576),  # V
-    (0.502, 0.502, 0.565),  # Cr
-    (0.502, 0.502, 0.565),  # Mn
-    (1.000, 0.647, 0.000),  # Fe
-    (1.000, 0.078, 0.576),  # Co
-    (0.647, 0.165, 0.165),  # Ni
-    (0.647, 0.165, 0.165),  # Cu
-    (0.647, 0.165, 0.165),  # Zn
-    (1.000, 0.078, 0.576),  # Ga
-    (1.000, 0.078, 0.576),  # Ge
-    (1.000, 0.078, 0.576),  # As
-    (1.000, 0.078, 0.576),  # Se
-    (0.647, 0.165, 0.165),  # Br
-    (1.000, 0.078, 0.576),  # Kr
-    (1.000, 0.078, 0.576),  # Rb
-    (1.000, 0.078, 0.576),  # Sr
-    (1.000, 0.078, 0.576),  # Y
-    (1.000, 0.078, 0.576),  # Zr
-    (1.000, 0.078, 0.576),  # Nb
-    (1.000, 0.078, 0.576),  # Mo
-    (1.000, 0.078, 0.576),  # Tc
-    (1.000, 0.078, 0.576),  # Ru
-    (1.000, 0.078, 0.576),  # Rh
-    (1.000, 0.078, 0.576),  # Pd
-    (0.502, 0.502, 0.565),  # Ag
-    (1.000, 0.078, 0.576),  # Cd
-    (1.000, 0.078, 0.576),  # In
-    (1.000, 0.078, 0.576),  # Sn
-    (1.000, 0.078, 0.576),  # Sb
-    (1.000, 0.078, 0.576),  # Te
-    (0.627, 0.125, 0.941),  # I
-    (1.000, 0.078, 0.576),  # Xe
-    (1.000, 0.078, 0.576),  # Cs
-    (1.000, 0.647, 0.000),  # Ba
-    (1.000, 0.078, 0.576),  # La
-    (1.000, 0.078, 0.576),  # Ce
-    (1.000, 0.078, 0.576),  # Pr
-    (1.000, 0.078, 0.576),  # Nd
-    (1.000, 0.078, 0.576),  # Pm
-    (1.000, 0.078, 0.576),  # Sm
-    (1.000, 0.078, 0.576),  # Eu
-    (1.000, 0.078, 0.576),  # Gd
-    (1.000, 0.078, 0.576),  # Tb
-    (1.000, 0.078, 0.576),  # Dy
-    (1.000, 0.078, 0.576),  # Ho
-    (1.000, 0.078, 0.576),  # Er
-    (1.000, 0.078, 0.576),  # Tm
-    (1.000, 0.078, 0.576),  # Yb
-    (1.000, 0.078, 0.576),  # Lu
-    (1.000, 0.078, 0.576),  # Hf
-    (1.000, 0.078, 0.576),  # Ta
-    (1.000, 0.078, 0.576),  # W
-    (1.000, 0.078, 0.576),  # Re
-    (1.000, 0.078, 0.576),  # Os
-    (1.000, 0.078, 0.576),  # Ir
-    (1.000, 0.078, 0.576),  # Pt
-    (0.855, 0.647, 0.125),  # Au
-    (1.000, 0.078, 0.576),  # Hg
-    (1.000, 0.078, 0.576),  # Tl
-    (1.000, 0.078, 0.576),  # Pb
-    (1.000, 0.078, 0.576),  # Bi
-    (1.000, 0.078, 0.576),  # Po
-    (1.000, 0.078, 0.576),  # At
-    (1.000, 1.000, 1.000),  # Rn
-    (1.000, 1.000, 1.000),  # Fr
-    (1.000, 1.000, 1.000),  # Ra
-    (1.000, 1.000, 1.000),  # Ac
-    (1.000, 0.078, 0.576),  # Th
-    (1.000, 1.000, 1.000),  # Pa
-    (1.000, 0.078, 0.576),  # U
-    (1.000, 1.000, 1.000),  # Np
-    (1.000, 1.000, 1.000),  # Pu
-    (1.000, 1.000, 1.000),  # Am
-    (1.000, 1.000, 1.000),  # Cm
-    (1.000, 1.000, 1.000),  # Bk
-    (1.000, 1.000, 1.000),  # Cf
-    (1.000, 1.000, 1.000),  # Es
-    (1.000, 1.000, 1.000),  # Fm
-    (1.000, 1.000, 1.000),  # Md
-    (1.000, 1.000, 1.000),  # No
-    (1.000, 1.000, 1.000)  # Lw
-])
+cpk_colors = np.array(
+    [
+        (1.000, 0.000, 0.000),  # None
+        (1.000, 1.000, 1.000),  # H
+        (1.000, 0.753, 0.796),  # He
+        (0.698, 0.133, 0.133),  # Li
+        (1.000, 0.078, 0.576),  # Be
+        (0.000, 1.000, 0.000),  # B
+        (0.784, 0.784, 0.784),  # C
+        (0.561, 0.561, 1.000),  # N
+        (0.941, 0.000, 0.000),  # O
+        (0.855, 0.647, 0.125),  # F
+        (1.000, 0.078, 0.576),  # Ne
+        (0.000, 0.000, 1.000),  # Na
+        (0.133, 0.545, 0.133),  # Mg
+        (0.502, 0.502, 0.565),  # Al
+        (0.855, 0.647, 0.125),  # Si
+        (1.000, 0.647, 0.000),  # P
+        (1.000, 0.784, 0.196),  # S
+        (0.000, 1.000, 0.000),  # Cl
+        (1.000, 0.078, 0.576),  # Ar
+        (1.000, 0.078, 0.576),  # K
+        (0.502, 0.502, 0.565),  # Ca
+        (1.000, 0.078, 0.576),  # Sc
+        (0.502, 0.502, 0.565),  # Ti
+        (1.000, 0.078, 0.576),  # V
+        (0.502, 0.502, 0.565),  # Cr
+        (0.502, 0.502, 0.565),  # Mn
+        (1.000, 0.647, 0.000),  # Fe
+        (1.000, 0.078, 0.576),  # Co
+        (0.647, 0.165, 0.165),  # Ni
+        (0.647, 0.165, 0.165),  # Cu
+        (0.647, 0.165, 0.165),  # Zn
+        (1.000, 0.078, 0.576),  # Ga
+        (1.000, 0.078, 0.576),  # Ge
+        (1.000, 0.078, 0.576),  # As
+        (1.000, 0.078, 0.576),  # Se
+        (0.647, 0.165, 0.165),  # Br
+        (1.000, 0.078, 0.576),  # Kr
+        (1.000, 0.078, 0.576),  # Rb
+        (1.000, 0.078, 0.576),  # Sr
+        (1.000, 0.078, 0.576),  # Y
+        (1.000, 0.078, 0.576),  # Zr
+        (1.000, 0.078, 0.576),  # Nb
+        (1.000, 0.078, 0.576),  # Mo
+        (1.000, 0.078, 0.576),  # Tc
+        (1.000, 0.078, 0.576),  # Ru
+        (1.000, 0.078, 0.576),  # Rh
+        (1.000, 0.078, 0.576),  # Pd
+        (0.502, 0.502, 0.565),  # Ag
+        (1.000, 0.078, 0.576),  # Cd
+        (1.000, 0.078, 0.576),  # In
+        (1.000, 0.078, 0.576),  # Sn
+        (1.000, 0.078, 0.576),  # Sb
+        (1.000, 0.078, 0.576),  # Te
+        (0.627, 0.125, 0.941),  # I
+        (1.000, 0.078, 0.576),  # Xe
+        (1.000, 0.078, 0.576),  # Cs
+        (1.000, 0.647, 0.000),  # Ba
+        (1.000, 0.078, 0.576),  # La
+        (1.000, 0.078, 0.576),  # Ce
+        (1.000, 0.078, 0.576),  # Pr
+        (1.000, 0.078, 0.576),  # Nd
+        (1.000, 0.078, 0.576),  # Pm
+        (1.000, 0.078, 0.576),  # Sm
+        (1.000, 0.078, 0.576),  # Eu
+        (1.000, 0.078, 0.576),  # Gd
+        (1.000, 0.078, 0.576),  # Tb
+        (1.000, 0.078, 0.576),  # Dy
+        (1.000, 0.078, 0.576),  # Ho
+        (1.000, 0.078, 0.576),  # Er
+        (1.000, 0.078, 0.576),  # Tm
+        (1.000, 0.078, 0.576),  # Yb
+        (1.000, 0.078, 0.576),  # Lu
+        (1.000, 0.078, 0.576),  # Hf
+        (1.000, 0.078, 0.576),  # Ta
+        (1.000, 0.078, 0.576),  # W
+        (1.000, 0.078, 0.576),  # Re
+        (1.000, 0.078, 0.576),  # Os
+        (1.000, 0.078, 0.576),  # Ir
+        (1.000, 0.078, 0.576),  # Pt
+        (0.855, 0.647, 0.125),  # Au
+        (1.000, 0.078, 0.576),  # Hg
+        (1.000, 0.078, 0.576),  # Tl
+        (1.000, 0.078, 0.576),  # Pb
+        (1.000, 0.078, 0.576),  # Bi
+        (1.000, 0.078, 0.576),  # Po
+        (1.000, 0.078, 0.576),  # At
+        (1.000, 1.000, 1.000),  # Rn
+        (1.000, 1.000, 1.000),  # Fr
+        (1.000, 1.000, 1.000),  # Ra
+        (1.000, 1.000, 1.000),  # Ac
+        (1.000, 0.078, 0.576),  # Th
+        (1.000, 1.000, 1.000),  # Pa
+        (1.000, 0.078, 0.576),  # U
+        (1.000, 1.000, 1.000),  # Np
+        (1.000, 1.000, 1.000),  # Pu
+        (1.000, 1.000, 1.000),  # Am
+        (1.000, 1.000, 1.000),  # Cm
+        (1.000, 1.000, 1.000),  # Bk
+        (1.000, 1.000, 1.000),  # Cf
+        (1.000, 1.000, 1.000),  # Es
+        (1.000, 1.000, 1.000),  # Fm
+        (1.000, 1.000, 1.000),  # Md
+        (1.000, 1.000, 1.000),  # No
+        (1.000, 1.000, 1.000),  # Lw
+    ]
+)
```

### Comparing `moftransformer-1.1.3/moftransformer/assets/topology.json` & `moftransformer-2.0.0/moftransformer/assets/topology.json`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/cli/download.py` & `moftransformer-2.0.0/moftransformer/cli/download.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,70 @@
+# MOFTransformer version 2.0.0
 class CLICommand:
     """
     Download pre-trained model, database, and fine-tuned model
     """
 
     @staticmethod
     def add_arguments(parser):
-        from moftransformer.utils.download import DEFAULT_PRETRAIN_MODEL_PATH, DEFAULT_COREMOF_PATH, DEFAULT_QMOF_PATH
+        from moftransformer.utils.download import (
+            DEFAULT_PRETRAIN_MODEL_PATH,
+            DEFAULT_COREMOF_PATH,
+            DEFAULT_QMOF_PATH,
+        )
+
         add = parser.add_argument
-        add ('target', nargs='+', help='(str) pretrain_model, finetuned_model, coremof, qmof, or hmof\n'
-                                       'pre-trained model (MTP/MOC/VFP), fine-tuned model (h2 uptake and band gap),\n'
-                                       'and database which contain graph-data and grid-data for "coremof", "qmof", and "hmof"\n')
-        add ('--outdir', '-o', help=f'The Path where downloaded data will be stored. \n'
-                                    f'default : (pretrain_model) {DEFAULT_PRETRAIN_MODEL_PATH} \n'
-                                    f'          (coremof) {DEFAULT_COREMOF_PATH}/\n'
-                                    f'          (qmof) {DEFAULT_QMOF_PATH}/\n'
-                                    f'          (hmof) {DEFAULT_QMOF_PATH}/hmof/\n'
-                                    f'          (finetuned_model) [path_moftransformer]/example/finetuned_model/', default=None)
-        add ('--remove_tarfile', '-r', action='store_true', help='remove tar.gz file for download database (coremof, qmof, and hmof)')
+        add(
+            "target",
+            nargs="+",
+            help="(str) pretrain_model, finetuned_model, coremof, qmof, or hmof\n"
+            "pre-trained model (MTP/MOC/VFP), fine-tuned model (h2 uptake and band gap),\n"
+            'and database which contain graph-data and grid-data for "coremof", "qmof", and "hmof"\n',
+        )
+        add(
+            "--outdir",
+            "-o",
+            help=f"The Path where downloaded data will be stored. \n"
+            f"default : (pretrain_model) {DEFAULT_PRETRAIN_MODEL_PATH} \n"
+            f"          (coremof) {DEFAULT_COREMOF_PATH}/\n"
+            f"          (qmof) {DEFAULT_QMOF_PATH}/\n"
+            f"          (hmof) {DEFAULT_QMOF_PATH}/hmof/\n"
+            f"          (finetuned_model) [path_moftransformer]/example/finetuned_model/",
+            default=None,
+        )
+        add(
+            "--remove_tarfile",
+            "-r",
+            action="store_true",
+            help="remove tar.gz file for download database (coremof, qmof, and hmof)",
+        )
 
     @staticmethod
     def run(args):
         from moftransformer.utils.download import (
             download_pretrain_model,
             download_coremof,
             download_finetuned_model,
             download_hmof,
             download_qmof,
         )
 
-        func_dic = {'pretrain_model':download_pretrain_model,
-                    'coremof':download_coremof,
-                    'hmof':download_hmof,
-                    'qmof':download_qmof,
-                    'finetuned_model':download_finetuned_model}
+        func_dic = {
+            "pretrain_model": download_pretrain_model,
+            "coremof": download_coremof,
+            "hmof": download_hmof,
+            "qmof": download_qmof,
+            "finetuned_model": download_finetuned_model,
+        }
 
         for stuff in args.target:
             if stuff not in func_dic.keys():
-                raise ValueError(f'target must be {", ".join(func_dic.keys())}, not {stuff}')
+                raise ValueError(
+                    f'target must be {", ".join(func_dic.keys())}, not {stuff}'
+                )
 
         for stuff in args.target:
             func = func_dic[stuff]
             if func.__code__.co_argcount == 1:
                 func(args.outdir)
             else:
                 func(args.outdir, args.remove_tarfile)
```

### Comparing `moftransformer-1.1.3/moftransformer/cli/main.py` & `moftransformer-2.0.0/moftransformer/cli/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,76 @@
+# MOFTransformer version 2.0.0
 import argparse
 import textwrap
 from importlib import import_module
 from argparse import RawTextHelpFormatter
 from moftransformer import __version__
 
 commands = [
-    #('info' , 'moftransformer.cli.info'),
-    ('install-griday' , 'moftransformer.cli.install_griday'),
-    ('uninstall-griday', 'moftransformer.cli.uninstall_griday'),
-    ('run', 'moftransformer.cli.run'),
-    ('download', 'moftransformer.cli.download'),
+    # ('info' , 'moftransformer.cli.info'),
+    ("install-griday", "moftransformer.cli.install_griday"),
+    ("uninstall-griday", "moftransformer.cli.uninstall_griday"),
+    ("run", "moftransformer.cli.run"),
+    ("download", "moftransformer.cli.download"),
 ]
 
 
-def main(prog='moftransformer', version=__version__, commands=commands, args=None):
-    parser = argparse.ArgumentParser(prog=prog, )
-    parser.add_argument('--version', action='version',
-                        version= '%(prog)s-{}'.format(version))
-    parser.add_argument('-T', '--traceback', action='store_true')
-    subparsers = parser.add_subparsers(title='Sub-command', dest='command')
-
-    subparser = subparsers.add_parser('help',
-                                      description='Help',
-                                      help='Help for sub-command.')
-
-    subparser.add_argument('helpcommand',
-                           nargs='?',
-                           metavar='sub-command',
-                           help='Provide help for sub-command.')
-
+def main(prog="moftransformer", version=__version__, commands=commands, args=None):
+    parser = argparse.ArgumentParser(
+        prog=prog,
+    )
+    parser.add_argument(
+        "--version", action="version", version="%(prog)s-{}".format(version)
+    )
+    parser.add_argument("-T", "--traceback", action="store_true")
+    subparsers = parser.add_subparsers(title="Sub-command", dest="command")
+
+    subparser = subparsers.add_parser(
+        "help", description="Help", help="Help for sub-command."
+    )
+
+    subparser.add_argument(
+        "helpcommand",
+        nargs="?",
+        metavar="sub-command",
+        help="Provide help for sub-command.",
+    )
 
     functions = {}
     parsers = {}
     for command, module_name in commands:
         cmd = import_module(module_name).CLICommand
         docstring = cmd.__doc__
         if docstring is None:
             # Backwards compatibility with GPAW
             short = cmd.short_description
-            long = getattr(cmd, 'description', short)
+            long = getattr(cmd, "description", short)
         else:
-            parts = docstring.split('\n', 1)
+            parts = docstring.split("\n", 1)
             if len(parts) == 1:
                 short = docstring
                 long = docstring
             else:
                 short, body = parts
                 long = short
-                #long = short + '\n' + textwrap.dedent(body)
+                # long = short + '\n' + textwrap.dedent(body)
         subparser = subparsers.add_parser(
-            command,
-            formatter_class=RawTextHelpFormatter,
-            help=short,
-            description=long)
+            command, formatter_class=RawTextHelpFormatter, help=short, description=long
+        )
         cmd.add_arguments(subparser)
         functions[command] = cmd.run
         parsers[command] = subparser
 
-    #if hook:
+    # if hook:
     #    args = hook(parser, args)
     #    args = hook(parser, args)
-    #else:
+    # else:
     args = parser.parse_args(args)
 
-    if args.command == 'help':
+    if args.command == "help":
         if args.helpcommand is None:
             parser.print_help()
         else:
             parsers[args.helpcommand].print_help()
     elif args.command is None:
         parser.print_usage()
     else:
@@ -79,11 +82,12 @@
                 f(args, parsers[args.command])
         except KeyboardInterrupt:
             pass
         except Exception as x:
             if args.traceback:
                 raise
             else:
-                l1 = '{}: {}\n'.format(x.__class__.__name__, x)
-                l2 = ('To get a full traceback, use: {} -T {} ...'
-                      .format(prog, args.command))
-                parser.error(l1 + l2)
+                l1 = "{}: {}\n".format(x.__class__.__name__, x)
+                l2 = "To get a full traceback, use: {} -T {} ...".format(
+                    prog, args.command
+                )
+                parser.error(l1 + l2)
```

### Comparing `moftransformer-1.1.3/moftransformer/cli/run.py` & `moftransformer-2.0.0/moftransformer/cli/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+# MOFTransformer version 2.0.0
 from pathlib import Path
 import os
 
+
 class CLICommand:
     """
     run moftransformer code
 
     ex) moftransformer run downstream='example' num_gpus=1 max_epochs=10
 
     """
 
     @staticmethod
     def add_arguments(parser):
-        parser.add_argument('args', nargs='*')
+        parser.add_argument("args", nargs="*")
 
     @staticmethod
     def run(args):
         from moftransformer import __root_dir__
-        run_path = Path(__root_dir__)/'run.py'
+
+        run_path = Path(__root_dir__) / "run.py"
         config = args.args
-        print (config)
-        os.system(f"python {run_path} with {' '.join(config)}")
+        print(config)
+        os.system(f"python {run_path} with {' '.join(config)}")
```

### Comparing `moftransformer-1.1.3/moftransformer/config.py` & `moftransformer-2.0.0/moftransformer/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,15 @@
+# MOFTransformer version 2.0.0
 import os
 from sacred import Experiment
 from moftransformer import __root_dir__
-from moftransformer.utils.download import DEFAULT_PRETRAIN_MODEL_PATH
+from moftransformer.utils.validation import _set_load_path, _loss_names
 
 ex = Experiment("pretrained_mof", save_git_info=False)
 
-
-def _loss_names(d):
-    ret = {
-        "ggm": 0,  # graph grid matching
-        "mpp": 0,  # masked patch prediction
-        "mtp": 0,  # mof topology prediction
-        "vfp": 0,  # (accessible) void fraction prediction
-        "moc": 0,  # metal organic classification
-        "bbc": 0,  # building block classification
-        "classification": 0,  # classification
-        "regression": 0,  # regression
-    }
-    ret.update(d)
-    return ret
-
-
 @ex.config
 def config():
     """
     # prepare_data
     max_num_atoms = 300
     min_length = 30
     max_length = 60
@@ -63,16 +48,18 @@
     downstream = ""
     n_classes = 0
 
     # Optimizer Setting
     optim_type = "adamw"  # adamw, adam, sgd (momentum=0.9)
     learning_rate = 1e-4
     weight_decay = 1e-2
-    decay_power = 1  # default polynomial decay, [cosine, constant, constant_with_warmup]
-    max_epochs = 100
+    decay_power = (
+        1  # default polynomial decay, [cosine, constant, constant_with_warmup]
+    )
+    max_epochs = 20
     max_steps = -1  # num_data * max_epoch // batch_size (accumulate_grad_batches)
     warmup_steps = 0.05  # int or float ( max_steps * warmup_steps)
     end_lr = 0
     lr_mult = 1  # multiply lr for downstream heads
 
     # PL Trainer Setting
     resume_from = None
@@ -80,22 +67,19 @@
     test_only = False
 
     # below params varies with the environment
     root_dataset = os.path.join(__root_dir__, "examples/dataset")
     log_dir = "logs/"
     batch_size = 1024  # desired batch size; for gradient accumulation
     per_gpu_batchsize = 8  # you should define this manually with per_gpu_batch_size
-    accelerator = 'gpu'
+    accelerator = "gpu"
     devices = 1
     num_nodes = 1
 
-    if os.path.exists(DEFAULT_PRETRAIN_MODEL_PATH):
-        load_path = DEFAULT_PRETRAIN_MODEL_PATH
-    else:
-        load_path = ""
+    load_path = _set_load_path('pmtransformer')
 
     num_workers = 16  # the number of cpu's core
     precision = 16
 
     # normalization target
     mean = None
     std = None
@@ -149,8 +133,8 @@
 def qmof_bandgap():
     exp_name = "qmof_bandgap"
     # root_dataset = ##
     downstream = "qmof_bandgap"
     max_epochs = 20
     batch_size = 32
     mean = 2.086
-    std = 1.131
+    std = 1.131
```

### Comparing `moftransformer-1.1.3/moftransformer/config_ex.py` & `moftransformer-2.0.0/moftransformer/config_ex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# MOFTransformer version 2.0.0
 import os
 from sacred import Experiment
 from moftransformer import __root_dir__
 from moftransformer.utils.download import DEFAULT_PRETRAIN_MODEL_PATH
 
 ex = Experiment("pretrained_mof", save_git_info=False)
 
@@ -63,15 +64,17 @@
     downstream = ""
     n_classes = 0
 
     # Optimizer Setting
     optim_type = "adamw"  # adamw, adam, sgd (momentum=0.9)
     learning_rate = 1e-4
     weight_decay = 1e-2
-    decay_power = 1  # default polynomial decay, [cosine, constant, constant_with_warmup]
+    decay_power = (
+        1  # default polynomial decay, [cosine, constant, constant_with_warmup]
+    )
     max_epochs = 100
     max_steps = -1  # num_data * max_epoch // batch_size (accumulate_grad_batches)
     warmup_steps = 0.05  # int or float ( max_steps * warmup_steps)
     end_lr = 0
     lr_mult = 1  # multiply lr for downstream heads
 
     # PL Trainer Setting
@@ -80,15 +83,15 @@
     test_only = False
 
     # below params varies with the environment
     root_dataset = os.path.join(__root_dir__, "examples/dataset")
     log_dir = "logs/"
     batch_size = 1024  # desired batch size; for gradient accumulation
     per_gpu_batchsize = 8  # you should define this manually with per_gpu_batch_size
-    accelerator = 'gpu'
+    accelerator = "gpu"
     devices = 1
     num_nodes = 1
 
     if os.path.exists(DEFAULT_PRETRAIN_MODEL_PATH):
         load_path = DEFAULT_PRETRAIN_MODEL_PATH
     else:
         load_path = ""
@@ -131,26 +134,30 @@
 fine-tuning (transfer learining)
 """
 
 
 @ex.named_config
 def ppn_1bar():
     exp_name = "ppn_1bar"
-    root_dataset = "/usr/data/transfer_learning/downstream_public/0_insilico_ppn/dataset"
+    root_dataset = (
+        "/usr/data/transfer_learning/downstream_public/0_insilico_ppn/dataset"
+    )
     downstream = "1bar"
     max_epochs = 20
     batch_size = 32
     mean = 3.79
     std = 5.32
 
 
 @ex.named_config
 def ppn_65bar():
     exp_name = "ppn_65bar"
-    root_dataset = "/usr/data/transfer_learning/downstream_public/0_insilico_ppn/dataset"
+    root_dataset = (
+        "/usr/data/transfer_learning/downstream_public/0_insilico_ppn/dataset"
+    )
     downstream = "65bar"
     max_epochs = 20
     batch_size = 32
     mean = 117.78
     std = 30.75
 
 
@@ -158,48 +165,56 @@
 in silico COF
 """
 
 
 @ex.named_config
 def cof_lowbar():
     exp_name = "cof_lowbar"
-    root_dataset = "/usr/data/transfer_learning/downstream_public/1_insilico_cof/dataset"
+    root_dataset = (
+        "/usr/data/transfer_learning/downstream_public/1_insilico_cof/dataset"
+    )
     downstream = "lowbar"
     max_epochs = 20
     batch_size = 32
     mean = 23.750
     std = 17.166
 
 
 @ex.named_config
 def cof_highbar():
     exp_name = "cof_highbar"
-    root_dataset = "/usr/data/transfer_learning/downstream_public/1_insilico_cof/dataset"
+    root_dataset = (
+        "/usr/data/transfer_learning/downstream_public/1_insilico_cof/dataset"
+    )
     downstream = "highbar"
     max_epochs = 20
     batch_size = 32
     mean = 159.076
     std = 38.164
 
 
 @ex.named_config
 def cof_logkh():
     exp_name = "cof_logkh"
-    root_dataset = "/usr/data/transfer_learning/downstream_public/1_insilico_cof/dataset"
+    root_dataset = (
+        "/usr/data/transfer_learning/downstream_public/1_insilico_cof/dataset"
+    )
     downstream = "logkh"
     max_epochs = 20
     batch_size = 32
     mean = -10.975
     std = 0.563
 
 
 @ex.named_config
 def cof_qst():
     exp_name = "cof_qst"
-    root_dataset = "/usr/data/transfer_learning/downstream_public/1_insilico_cof/dataset"
+    root_dataset = (
+        "/usr/data/transfer_learning/downstream_public/1_insilico_cof/dataset"
+    )
     downstream = "qst"
     max_epochs = 20
     batch_size = 32
     mean = -14.793
     std = 4.542
 
 
@@ -207,97 +222,108 @@
 pcod zeolite
 """
 
 
 @ex.named_config
 def zeo_qst():
     exp_name = "zeo_qst"
-    root_dataset = "/usr/data/transfer_learning/downstream_public/2_pcod_zeolite/dataset"
+    root_dataset = (
+        "/usr/data/transfer_learning/downstream_public/2_pcod_zeolite/dataset"
+    )
     downstream = "qst"
     max_epochs = 20
     batch_size = 32
     mean = 19.052
     std = 3.169
 
 
 @ex.named_config
 def zeo_unitlesskh():
     exp_name = "zeo_unitlesskh"
-    root_dataset = "/usr/data/transfer_learning/downstream_public/2_pcod_zeolite/dataset"
+    root_dataset = (
+        "/usr/data/transfer_learning/downstream_public/2_pcod_zeolite/dataset"
+    )
     downstream = "unitlesskh"
     max_epochs = 20
     batch_size = 32
     mean = 19.725
     std = 12.317
 
 
 """
 mof downstream
 """
 
+
 @ex.named_config
 def mof_raspa_100bar():
     exp_name = "mof_raspa_100bar"
     # root_dataset = ##
     downstream = "raspa_100bar"
     max_epochs = 20
     batch_size = 32
     mean = 487.866
     std = 63.504
 
+
 @ex.named_config
 def mof_diffusivity_log():
     exp_name = "mof_diffusivity_log"
     # root_dataset = ##
     downstream = "diffusivity_log"
     max_epochs = 20
     batch_size = 32
     mean = -8.306
     std = 1.490
 
+
 @ex.named_config
 def mof_bandgap():
     exp_name = "mof_bandgap"
     # root_dataset = ##
     downstream = "bandgap"
     max_epochs = 20
     batch_size = 32
     mean = 2.086
     std = 1.131
 
+
 @ex.named_config
 def mof_n2uptake():
     exp_name = "mof_n2uptake"
     # root_dataset = ##
     downstream = "n2uptake"
     max_epochs = 20
     batch_size = 32
     mean = 0.3999
     std = 0.337
 
+
 @ex.named_config
 def mof_o2uptake():
     exp_name = "mof_o2uptake"
     # root_dataset = ##
     downstream = "o2uptake"
     max_epochs = 20
     batch_size = 32
     mean = 0.387
     std = 0.241
 
+
 @ex.named_config
 def mof_n2diffusivity_dilute():
     exp_name = "mof_n2diffusivity_dilute"
     # root_dataset = ##
     downstream = "n2diffusivity_dilute"
     max_epochs = 20
     batch_size = 32
     mean = 0.000187
     std = 0.000176
 
+
 @ex.named_config
 def mof_o2diffusivity_dilute():
     exp_name = "mof_o2diffusivity_dilute"
     # root_dataset = ##
     downstream = "o2diffusivity_dilute"
     max_epochs = 20
     batch_size = 32
@@ -337,90 +363,102 @@
     max_epochs = 20
     batch_size = 32
     mean = 0.592
     std = 0.491
     loss_names = _loss_names({"classification": 1})
     n_classes = 2
 
+
 """
 downstream example (H2 uptake)
 """
+
+
 @ex.named_config
 def mof_h2_uptake():
     exp_name = "mof_h2_uptake"
     # root_dataset = ##
     downstream = "h2_uptake"
     max_epochs = 20
     batch_size = 32
     mean = 488.029
     std = 62.690
 
+
 @ex.named_config
 def cof_h2_uptake():
     exp_name = "cof_h2_uptake"
     # root_dataset = ##
     downstream = "h2_uptake"
     max_epochs = 20
     batch_size = 32
     mean = 485.978
     std = 80.930
 
+
 @ex.named_config
 def ppn_h2_uptake():
     exp_name = "ppn_h2_uptake"
     # root_dataset = ##
     downstream = "h2_uptake"
     max_epochs = 20
     batch_size = 32
     mean = 465.196
     std = 117.529
 
+
 @ex.named_config
 def zeo_h2_uptake():
     exp_name = "zeo_h2_uptake"
     # root_dataset = ##
     downstream = "h2_uptake"
     max_epochs = 20
     batch_size = 32
     mean = 259.878
     std = 112.928
 
+
 """
 downstream example (H2 working capacity)
 """
+
+
 @ex.named_config
 def mof_h2_wc():
     exp_name = "mof_h2_wc"
     # root_dataset = ##
     downstream = "h2_wc"
     max_epochs = 20
     batch_size = 32
     mean = 320.019
     std = 87.993
 
+
 @ex.named_config
 def cof_h2_wc():
     exp_name = "cof_h2_wc"
     # root_dataset = ##
     downstream = "h2_wc"
     max_epochs = 20
     batch_size = 32
     mean = 326.740
     std = 84.470
 
+
 @ex.named_config
 def ppn_h2_wc():
     exp_name = "ppn_h2_wc"
     # root_dataset = ##
     downstream = "h2_wc"
     max_epochs = 20
     batch_size = 32
     mean = 300.407
     std = 116.746
 
+
 @ex.named_config
 def zeo_h2_wc():
     exp_name = "zeo_h2_wc"
     # root_dataset = ##
     downstream = "h2_wc"
     max_epochs = 20
     batch_size = 32
@@ -434,17 +472,20 @@
     # root_dataset = ##
     downstream = "h2_wc"
     max_epochs = 20
     batch_size = 32
     mean = 241.300
     std = 152.052
 
+
 """
 curated COF few shot
 """
+
+
 @ex.named_config
 def ccof_bandgap():
     exp_name = "ccof_bandgap"
     # root_dataset = ##
     downstream = "ccof_bandgap"
     max_epochs = 20
     batch_size = 32
@@ -456,8 +497,8 @@
 def qmof_bandgap():
     exp_name = "qmof_bandgap"
     # root_dataset = ##
     downstream = "qmof_bandgap"
     max_epochs = 20
     batch_size = 32
     mean = 2.086
-    std = 1.131
+    std = 1.131
```

### Comparing `moftransformer-1.1.3/moftransformer/datamodules/datamodule.py` & `moftransformer-2.0.0/moftransformer/datamodules/datamodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# MOFTransformer version 2.0.0
 import functools
 from typing import Optional
 
 from torch.utils.data import DataLoader
 
 from pytorch_lightning import LightningDataModule
 from moftransformer.datamodules.dataset import Dataset
```

### Comparing `moftransformer-1.1.3/moftransformer/datamodules/dataset.py` & `moftransformer-2.0.0/moftransformer/datamodules/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+# MOFTransformer version 2.0.0
 import os
 import random
 import json
 import pickle
 
 import numpy as np
 
 import torch
 from torch.nn.functional import interpolate
 
 
 class Dataset(torch.utils.data.Dataset):
     def __init__(
-            self,
-            data_dir: str,
-            split: str,
-            nbr_fea_len: int,
-            draw_false_grid=True,
-            downstream="",
-            tasks=[],
+        self,
+        data_dir: str,
+        split: str,
+        nbr_fea_len: int,
+        draw_false_grid=True,
+        downstream="",
+        tasks=[],
     ):
         """
         Dataset for pretrained MOF.
         Args:
             data_dir (str): where dataset cif files and energy grid file; exist via model.utils.prepare_data.py
             split(str) : train, test, split
             draw_false_grid (int, optional):  how many generating false_grid_data
@@ -36,39 +37,45 @@
         if downstream:
             path_file = os.path.join(data_dir, f"{split}_{downstream}.json")
         else:
             path_file = os.path.join(data_dir, f"{split}.json")
         print(f"read {path_file}...")
 
         if not os.path.isfile(path_file):
-            raise FileNotFoundError(f"{path_file} doesn't exist. Check 'root_dataset' in config")
+            raise FileNotFoundError(
+                f"{path_file} doesn't exist. Check 'root_dataset' in config"
+            )
 
         dict_target = json.load(open(path_file, "r"))
         self.cif_ids, self.targets = zip(*dict_target.items())
 
         self.nbr_fea_len = nbr_fea_len
 
         self.tasks = {}
 
         for task in tasks:
             if task in ["mtp", "vfp", "moc", "bbc"]:
                 path_file = os.path.join(data_dir, f"{split}_{task}.json")
                 print(f"read {path_file}...")
-                assert os.path.isfile(path_file), f"{path_file} doesn't exist in {data_dir}"
+                assert os.path.isfile(
+                    path_file
+                ), f"{path_file} doesn't exist in {data_dir}"
 
                 dict_task = json.load(open(path_file, "r"))
                 cif_ids, t = zip(*dict_task.items())
                 self.tasks[task] = list(t)
-                assert self.cif_ids == cif_ids, print("order of keys is different in the json file")
+                assert self.cif_ids == cif_ids, print(
+                    "order of keys is different in the json file"
+                )
 
     def __len__(self):
         return len(self.cif_ids)
 
     @staticmethod
-    def make_grid_data(grid_data, emin=-5000., emax=5000, bins=101):
+    def make_grid_data(grid_data, emin=-5000.0, emax=5000, bins=101):
         """
         make grid_data within range (emin, emax) and
         make bins with logit function
         and digitize (0, bins)
         ****
             caution : 'zero' should be padding !!
             when you change bins, heads.MPP_heads should be changed
@@ -84,15 +91,15 @@
 
     @staticmethod
     def calculate_volume(a, b, c, angle_a, angle_b, angle_c):
         a_ = np.cos(angle_a * np.pi / 180)
         b_ = np.cos(angle_b * np.pi / 180)
         c_ = np.cos(angle_c * np.pi / 180)
 
-        v = a * b * c * np.sqrt(1 - a_ ** 2 - b_ ** 2 - c_ ** 2 + 2 * a_ * b_ * c_)
+        v = a * b * c * np.sqrt(1 - a_**2 - b_**2 - c_**2 + 2 * a_ * b_ * c_)
 
         return v.item() / (60 * 60 * 60)  # normalized volume
 
     def get_raw_grid_data(self, cif_id):
         file_grid = os.path.join(self.data_dir, self.split, f"{cif_id}.grid")
         file_griddata = os.path.join(self.data_dir, self.split, f"{cif_id}.griddata16")
 
@@ -109,15 +116,14 @@
         grid_data = pickle.load(open(file_griddata, "rb"))
         grid_data = self.make_grid_data(grid_data)
         grid_data = torch.FloatTensor(grid_data)
 
         return cell, volume, grid_data
 
     def get_grid_data(self, cif_id, draw_false_grid=False):
-
         cell, volume, grid_data = self.get_raw_grid_data(cif_id)
         ret = {
             "cell": cell,
             "volume": volume,
             "grid_data": grid_data,
         }
 
@@ -125,42 +131,45 @@
             random_index = random.randint(0, len(self.cif_ids) - 1)
             cif_id = self.cif_ids[random_index]
             cell, volume, grid_data = self.get_raw_grid_data(cif_id)
             ret.update(
                 {
                     "false_cell": cell,
                     "fale_volume": volume,
-                    "false_grid_data": grid_data
+                    "false_grid_data": grid_data,
                 }
             )
         return ret
 
     @staticmethod
     def get_gaussian_distance(distances, num_step, dmax, dmin=0, var=0.2):
         """
         Expands the distance by Gaussian basis
         (https://github.com/txie-93/cgcnn.git)
         """
 
         assert dmin < dmax
-        _filter = np.linspace(dmin, dmax, num_step)  # = np.arange(dmin, dmax + step, step) with step = 0.2
+        _filter = np.linspace(
+            dmin, dmax, num_step
+        )  # = np.arange(dmin, dmax + step, step) with step = 0.2
 
-        return np.exp(-(distances[..., np.newaxis] - _filter) ** 2 /
-                      var ** 2).float()
+        return np.exp(-((distances[..., np.newaxis] - _filter) ** 2) / var**2).float()
 
     def get_graph(self, cif_id):
         file_graph = os.path.join(self.data_dir, self.split, f"{cif_id}.graphdata")
 
         graphdata = pickle.load(open(file_graph, "rb"))
         # graphdata = ["cif_id", "atom_num", "nbr_idx", "nbr_dist", "uni_idx", "uni_count"]
         atom_num = torch.LongTensor(graphdata[1].copy())
         nbr_idx = torch.LongTensor(graphdata[2].copy()).view(len(atom_num), -1)
         nbr_dist = torch.FloatTensor(graphdata[3].copy()).view(len(atom_num), -1)
 
-        nbr_fea = torch.FloatTensor(self.get_gaussian_distance(nbr_dist, num_step=self.nbr_fea_len, dmax=8))
+        nbr_fea = torch.FloatTensor(
+            self.get_gaussian_distance(nbr_dist, num_step=self.nbr_fea_len, dmax=8)
+        )
 
         uni_idx = graphdata[4]
         uni_count = graphdata[5]
 
         return {
             "atom_num": atom_num,
             "nbr_idx": nbr_idx,
@@ -168,24 +177,19 @@
             "uni_idx": uni_idx,
             "uni_count": uni_count,
         }
 
     def get_tasks(self, index):
         ret = dict()
         for task, value in self.tasks.items():
-            ret.update(
-                {
-                    task: value[index]
-                }
-            )
+            ret.update({task: value[index]})
 
         return ret
 
     def __getitem__(self, index):
-
         ret = dict()
         cif_id = self.cif_ids[index]
         target = self.targets[index]
 
         ret.update(
             {
                 "cif_id": cif_id,
@@ -222,17 +226,15 @@
         batch_nbr_idx = dict_batch["nbr_idx"]
         batch_nbr_fea = dict_batch["nbr_fea"]
 
         crystal_atom_idx = []
         base_idx = 0
         for i, nbr_idx in enumerate(batch_nbr_idx):
             n_i = nbr_idx.shape[0]
-            crystal_atom_idx.append(
-                torch.arange(n_i) + base_idx
-            )
+            crystal_atom_idx.append(torch.arange(n_i) + base_idx)
             nbr_idx += base_idx
             base_idx += n_i
 
         dict_batch["atom_num"] = torch.cat(batch_atom_num, dim=0)
         dict_batch["nbr_idx"] = torch.cat(batch_nbr_idx, dim=0)
         dict_batch["nbr_fea"] = torch.cat(batch_nbr_fea, dim=0)
         dict_batch["crystal_atom_idx"] = crystal_atom_idx
@@ -240,41 +242,42 @@
         # grid
         batch_grid_data = dict_batch["grid_data"]
         batch_cell = dict_batch["cell"]
         new_grids = []
 
         for bi in range(batch_size):
             orig = batch_grid_data[bi].view(batch_cell[bi][::-1]).transpose(0, 2)
-            if batch_cell[bi] == [30, 30, 30]:      # version >= 1.1.2
+            if batch_cell[bi] == [30, 30, 30]:  # version >= 1.1.2
                 orig = orig[None, None, :, :, :]
             else:
-                orig = interpolate(orig[None, None, :, :, :],
-                                   size=[img_size, img_size, img_size],
-                                   mode="trilinear",
-                                   align_corners=True,
-                                   )
+                orig = interpolate(
+                    orig[None, None, :, :, :],
+                    size=[img_size, img_size, img_size],
+                    mode="trilinear",
+                    align_corners=True,
+                )
             new_grids.append(orig)
         new_grids = torch.concat(new_grids, axis=0)
         dict_batch["grid"] = new_grids
 
         if "false_grid_data" in dict_batch.keys():
-
             batch_false_grid_data = dict_batch["false_grid_data"]
             batch_false_cell = dict_batch["false_cell"]
             new_false_grids = []
             for bi in range(batch_size):
                 orig = batch_false_grid_data[bi].view(batch_false_cell[bi])
                 if batch_cell[bi] == [30, 30, 30]:  # version >= 1.1.2
                     orig = orig[None, None, :, :, :]
                 else:
-                    orig = interpolate(orig[None, None, :, :, :],
-                                       size=[img_size, img_size, img_size],
-                                       mode="trilinear",
-                                       align_corners=True,
-                                       )
+                    orig = interpolate(
+                        orig[None, None, :, :, :],
+                        size=[img_size, img_size, img_size],
+                        mode="trilinear",
+                        align_corners=True,
+                    )
                 new_false_grids.append(orig)
             new_false_grids = torch.concat(new_false_grids, axis=0)
             dict_batch["false_grid"] = new_false_grids
 
         dict_batch.pop("grid_data", None)
         dict_batch.pop("false_grid_data", None)
         dict_batch.pop("cell", None)
```

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/test/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/test/acs+N270+E33.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/test/acs+N270+E33.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/test/acs+N270+E33.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/test/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/test/smm+N577+E166.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/test/smm+N577+E166.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/test/smm+N577+E166.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/acs+N270+E33.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/acs+N270+E33.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/acs+N270+E33.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/fee+N254+E185.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/fee+N254+E185.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/fee+N254+E185.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/mok+N109+E146.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/mok+N109+E146.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/mok+N109+E146.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/msp+N624+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/msp+N624+E8.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/msp+N624+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/sml+N696+E182.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/sml+N696+E182.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/sml+N696+E182.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/smm+N577+E166.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/smm+N577+E166.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/smm+N577+E166.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/ukg+N387+E203.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/vna+N650+E120.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/vna+N650+E120.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/vna+N650+E120.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/fee+N254+E185.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/fee+N254+E185.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/fee+N254+E185.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/mok+N109+E146.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/mok+N109+E146.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/mok+N109+E146.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/msp+N624+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/msp+N624+E8.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/msp+N624+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/sml+N696+E182.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/sml+N696+E182.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/sml+N696+E182.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/ukg+N387+E203.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/vna+N650+E120.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/vna+N650+E120.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/vna+N650+E120.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/val/acs+N270+E33.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/val/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/val/acs+N270+E33.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/val/acs+N270+E33.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/val/acs+N270+E33.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/val/acs+N270+E33.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/val/smm+N577+E166.cif` & `moftransformer-2.0.0/moftransformer/examples/dataset/val/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/val/smm+N577+E166.graphdata` & `moftransformer-2.0.0/moftransformer/examples/dataset/val/smm+N577+E166.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/dataset/val/smm+N577+E166.griddata16` & `moftransformer-2.0.0/moftransformer/examples/dataset/val/smm+N577+E166.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/raw/acs+N270+E33.cif` & `moftransformer-2.0.0/moftransformer/examples/raw/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif` & `moftransformer-2.0.0/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/raw/fee+N254+E185.cif` & `moftransformer-2.0.0/moftransformer/examples/raw/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/raw/mok+N109+E146.cif` & `moftransformer-2.0.0/moftransformer/examples/raw/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif` & `moftransformer-2.0.0/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/raw/msp+N624+E8.cif` & `moftransformer-2.0.0/moftransformer/examples/raw/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/raw/sml+N696+E182.cif` & `moftransformer-2.0.0/moftransformer/examples/raw/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/raw/smm+N577+E166.cif` & `moftransformer-2.0.0/moftransformer/examples/raw/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/raw/ukg+N387+E203.cif` & `moftransformer-2.0.0/moftransformer/examples/raw/ukg+N387+E203.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/raw/vmk+N489+E8.cif` & `moftransformer-2.0.0/moftransformer/examples/raw/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/raw/vna+N650+E120.cif` & `moftransformer-2.0.0/moftransformer/examples/raw/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/raw/zzz+N96+N373+E34.cif` & `moftransformer-2.0.0/moftransformer/examples/raw/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16` & `moftransformer-2.0.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/gadgets/my_metrics.py` & `moftransformer-2.0.0/moftransformer/gadgets/my_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# MOFTransformer version 2.0.0
 import torch
 from torchmetrics import Metric
 
 
 class Accuracy(Metric):
     def __init__(self, dist_sync_on_step=False):
         super().__init__(dist_sync_on_step=dist_sync_on_step)
```

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/AtomTypeMap.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/AtomTypeMap.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/AtomTypeMap.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/AtomTypeMap.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/AtomTypeMap.o` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/AtomTypeMap.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Cell.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Cell.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ChannelAnalyzer.o` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/EnergyGrid.o` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/EnergyGrid.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/UFF_FF.def` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/UFF_FF.def`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/FF/UFF_Type.def` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/FF/UFF_Type.def`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ForceField.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/ForceField.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ForceField.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/ForceField.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ForceField.o` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/ForceField.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/FourierAnalyzer.o` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/FourierAnalyzer.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Framework.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Framework.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Framework.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Framework.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Framework.o` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Framework.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Gaussian.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Gaussian.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Gaussian.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Gaussian.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Gaussian.o` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Gaussian.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridMaker.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridMaker.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridMaker.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridMaker.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridMaker.o` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridMaker.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayException.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayException.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayException.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayException.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayException.o` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayException.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/GridayTypes.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/GridayTypes.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/LennardJones.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/LennardJones.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/LennardJones.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/LennardJones.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/LennardJones.o` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/LennardJones.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/MaterialGrid.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/MaterialGrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/MaterialGrid.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/MaterialGrid.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/MaterialGrid.o` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/MaterialGrid.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/NlistMaker.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/NlistMaker.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/NlistMaker.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/NlistMaker.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/NlistMaker.o` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/NlistMaker.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/PairEnergy.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/PairEnergy.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Random.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Random.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ShiftedLJ.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/ShiftedLJ.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ShiftedLJ.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/ShiftedLJ.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/ShiftedLJ.o` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/ShiftedLJ.o`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Timer.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Timer.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/Vector.hpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/Vector.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/libgriday.a` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/libgriday.a`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/Makefile` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/Makefile`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid2COTA` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/grid2COTA`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid2props` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/grid2props`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid2visit` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/grid2visit`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/grid_gen` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/grid_gen`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/main_cota.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/main_cota.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/libs/GRIDAY/scripts/main_visit.cpp` & `moftransformer-2.0.0/moftransformer/libs/GRIDAY/scripts/main_visit.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/modules/cgcnn.py` & `moftransformer-2.0.0/moftransformer/modules/cgcnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# MOFTransformer version 2.0.0
 import random
 
 import torch
 import torch.nn as nn
 
 
 class ConvLayer(nn.Module):
@@ -10,16 +11,17 @@
     (https://github.com/txie-93/cgcnn)
     """
 
     def __init__(self, atom_fea_len, nbr_fea_len):
         super().__init__()
         self.atom_fea_len = atom_fea_len
         self.nbr_fea_len = nbr_fea_len
-        self.fc_full = nn.Linear(2 * self.atom_fea_len + self.nbr_fea_len,
-                                 2 * self.atom_fea_len)
+        self.fc_full = nn.Linear(
+            2 * self.atom_fea_len + self.nbr_fea_len, 2 * self.atom_fea_len
+        )
         self.sigmoid = nn.Sigmoid()
         self.softplus1 = nn.Softplus()
         self.bn1 = nn.BatchNorm1d(2 * self.atom_fea_len)
         self.bn2 = nn.BatchNorm1d(self.atom_fea_len)
         self.softplus2 = nn.Softplus()
 
     def forward(self, atom_in_fea, nbr_fea, nbr_fea_idx):
@@ -45,24 +47,30 @@
         """
 
         N, M = nbr_fea_idx.shape
         # convolution
         atom_nbr_fea = atom_in_fea[nbr_fea_idx, :]  # [N, M, atom_fea_len]
 
         total_nbr_fea = torch.cat(
-            [atom_in_fea.unsqueeze(1).expand(N, M, self.atom_fea_len),
-             # [N, atom_fea_len] -> [N, M, atom_fea_len] -> v_i
-             atom_nbr_fea,  # [N, M, atom_fea_len] -> v_j
-             nbr_fea],  # [N, M, nbr_fea_len] -> u(i,j)_k
-            dim=2)
+            [
+                atom_in_fea.unsqueeze(1).expand(N, M, self.atom_fea_len),
+                # [N, atom_fea_len] -> [N, M, atom_fea_len] -> v_i
+                atom_nbr_fea,  # [N, M, atom_fea_len] -> v_j
+                nbr_fea,
+            ],  # [N, M, nbr_fea_len] -> u(i,j)_k
+            dim=2,
+        )
         # [N, M, atom_fea_len*2+nrb_fea_len]
 
         total_gated_fea = self.fc_full(total_nbr_fea)  # [N, M, atom_fea_len*2]
-        total_gated_fea = self.bn1(total_gated_fea.view(
-            -1, self.atom_fea_len * 2)).view(N, M, self.atom_fea_len * 2)  # [N, M, atom_fea_len*2]
+        total_gated_fea = self.bn1(
+            total_gated_fea.view(-1, self.atom_fea_len * 2)
+        ).view(
+            N, M, self.atom_fea_len * 2
+        )  # [N, M, atom_fea_len*2]
         nbr_filter, nbr_core = total_gated_fea.chunk(2, dim=2)  # [N, M, atom_fea_len]
         nbr_filter = self.sigmoid(nbr_filter)
         nbr_core = self.softplus1(nbr_core)
         nbr_sumed = torch.sum(nbr_filter * nbr_core, dim=1)  # [N, atom_fea_len]
         nbr_sumed = self.bn2(nbr_sumed)
         out = self.softplus2(atom_in_fea + nbr_sumed)  # [N, atom_fea_len]
         return out
@@ -70,15 +78,17 @@
 
 class GraphEmbeddings(nn.Module):
     """
     Generate Embedding layers made by only convolution layers of CGCNN (not pooling)
     (https://github.com/txie-93/cgcnn)
     """
 
-    def __init__(self, atom_fea_len, nbr_fea_len, max_graph_len, hid_dim, n_conv=3, vis=False):
+    def __init__(
+        self, atom_fea_len, nbr_fea_len, max_graph_len, hid_dim, n_conv=3, vis=False
+    ):
         super().__init__()
         self.atom_fea_len = atom_fea_len
         self.nbr_fea_len = nbr_fea_len
         self.max_graph_len = max_graph_len
         self.hid_dim = hid_dim
         self.embedding = nn.Embedding(119, atom_fea_len)  # 119 -> max(atomic number)
         self.convs = nn.ModuleList(
@@ -87,15 +97,17 @@
                 for _ in range(n_conv)
             ]
         )
         self.fc = nn.Linear(atom_fea_len, hid_dim)
 
         self.vis = vis
 
-    def forward(self, atom_num, nbr_idx, nbr_fea, crystal_atom_idx, uni_idx, uni_count, moc=None):
+    def forward(
+        self, atom_num, nbr_idx, nbr_fea, crystal_atom_idx, uni_idx, uni_count, moc=None
+    ):
         """
         Args:
             atom_num (tensor): [N', atom_fea_len]
             nbr_idx (tensor): [N', M]
             nbr_fea (tensor): [N', M, nbr_fea_len]
             crystal_atom_idx (list): [B]
             uni_idx (list) : [B]
@@ -107,41 +119,43 @@
         assert self.nbr_fea_len == nbr_fea.shape[-1]
 
         atom_fea = self.embedding(atom_num)  # [N', atom_fea_len]
         for conv in self.convs:
             atom_fea = conv(atom_fea, nbr_fea, nbr_idx)  # [N', atom_fea_len]
         atom_fea = self.fc(atom_fea)  # [N', hid_dim]
 
-        new_atom_fea, mask, mo_label = self.reconstruct_batch(atom_fea, crystal_atom_idx, uni_idx, uni_count, moc)
+        new_atom_fea, mask, mo_label = self.reconstruct_batch(
+            atom_fea, crystal_atom_idx, uni_idx, uni_count, moc
+        )
         # [B, max_graph_len, hid_dim], [B, max_graph_len]
         return new_atom_fea, mask, mo_label  # None will be replaced with MOC
 
     def reconstruct_batch(self, atom_fea, crystal_atom_idx, uni_idx, uni_count, moc):
         batch_size = len(crystal_atom_idx)
 
         new_atom_fea = torch.full(
-            size=[batch_size, self.max_graph_len, self.hid_dim],
-            fill_value=0.
+            size=[batch_size, self.max_graph_len, self.hid_dim], fill_value=0.0
         ).to(atom_fea)
 
         mo_label = torch.full(
-            size=[batch_size, self.max_graph_len],
-            fill_value=-100.
+            size=[batch_size, self.max_graph_len], fill_value=-100.0
         ).to(atom_fea)
 
         for bi, c_atom_idx in enumerate(crystal_atom_idx):
             # set uni_idx with (descending count or random) and cut max_graph_len
-            idx_ = torch.LongTensor([random.choice(u) for u in uni_idx[bi]])[:self.max_graph_len]
+            idx_ = torch.LongTensor([random.choice(u) for u in uni_idx[bi]])[
+                : self.max_graph_len
+            ]
             rand_idx = idx_[torch.randperm(len(idx_))]
             if self.vis:
                 rand_idx = idx_
-            new_atom_fea[bi][:len(rand_idx)] = atom_fea[c_atom_idx][rand_idx]
+            new_atom_fea[bi][: len(rand_idx)] = atom_fea[c_atom_idx][rand_idx]
 
             if moc:
                 mo = torch.zeros(len(c_atom_idx))
                 metal_idx = moc[bi]
                 mo[metal_idx] = 1
-                mo_label[bi][:len(rand_idx)] = mo[rand_idx]
+                mo_label[bi][: len(rand_idx)] = mo[rand_idx]
 
         mask = (new_atom_fea.sum(dim=-1) != 0).float()
 
         return new_atom_fea, mask, mo_label
```

### Comparing `moftransformer-1.1.3/moftransformer/modules/heads.py` & `moftransformer-2.0.0/moftransformer/modules/heads.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+# MOFTransformer version 2.0.0
 import torch.nn as nn
 
 from transformers.models.bert.modeling_bert import (
-    BertConfig, BertPredictionHeadTransform
+    BertConfig,
+    BertPredictionHeadTransform,
 )
 
 
 class Pooler(nn.Module):
     def __init__(self, hidden_size, index=0):
         super().__init__()
         self.dense = nn.Linear(hidden_size, hidden_size)
```

### Comparing `moftransformer-1.1.3/moftransformer/modules/module.py` & `moftransformer-2.0.0/moftransformer/modules/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# MOFTransformer version 2.0.0
 import torch
 import torch.nn as nn
 from pytorch_lightning import LightningModule
 
 from moftransformer.modules import objectives, heads, module_utils
 from moftransformer.modules.cgcnn import GraphEmbeddings
 from moftransformer.modules.vision_transformer_3d import VisionTransformer3D
@@ -107,98 +108,110 @@
 
         if config["load_path"] != "" and config["test_only"]:
             ckpt = torch.load(config["load_path"], map_location="cpu")
             state_dict = ckpt["state_dict"]
             self.load_state_dict(state_dict, strict=False)
             print(f"load model : {config['load_path']}")
 
-    def infer(self,
-              batch,
-              mask_grid=False,
-              ):
-
+    def infer(
+        self,
+        batch,
+        mask_grid=False,
+    ):
         cif_id = batch["cif_id"]
         atom_num = batch["atom_num"]  # [N']
         nbr_idx = batch["nbr_idx"]  # [N', M]
         nbr_fea = batch["nbr_fea"]  # [N', M, nbr_fea_len]
         crystal_atom_idx = batch["crystal_atom_idx"]  # list [B]
         uni_idx = batch["uni_idx"]  # list [B]
         uni_count = batch["uni_count"]  # list [B]
 
         grid = batch["grid"]  # [B, C, H, W, D]
         volume = batch["volume"]  # list [B]
 
         if "moc" in batch.keys():
-            moc =  batch["moc"] # [B]
+            moc = batch["moc"]  # [B]
         elif "bbc" in batch.keys():
-            moc = batch["bbc"] # [B]
+            moc = batch["bbc"]  # [B]
         else:
             moc = None
 
         # get graph embeds
-        (graph_embeds,  # [B, max_graph_len, hid_dim],
-         graph_masks,  # [B, max_graph_len],
-         mo_labels,  # if moc: [B, max_graph_len], else: None
-         ) = self.graph_embeddings(
+        (
+            graph_embeds,  # [B, max_graph_len, hid_dim],
+            graph_masks,  # [B, max_graph_len],
+            mo_labels,  # if moc: [B, max_graph_len], else: None
+        ) = self.graph_embeddings(
             atom_num=atom_num,
             nbr_idx=nbr_idx,
             nbr_fea=nbr_fea,
             crystal_atom_idx=crystal_atom_idx,
             uni_idx=uni_idx,
             uni_count=uni_count,
             moc=moc,
         )
         # add class embeds to graph_embeds
         cls_tokens = torch.zeros(len(crystal_atom_idx)).to(graph_embeds)  # [B]
         cls_embeds = self.cls_embeddings(cls_tokens[:, None, None])  # [B, 1, hid_dim]
         cls_mask = torch.ones(len(crystal_atom_idx), 1).to(graph_masks)  # [B, 1]
 
-        graph_embeds = torch.cat([cls_embeds, graph_embeds], dim=1)  # [B, max_graph_len+1, hid_dim]
+        graph_embeds = torch.cat(
+            [cls_embeds, graph_embeds], dim=1
+        )  # [B, max_graph_len+1, hid_dim]
         graph_masks = torch.cat([cls_mask, graph_masks], dim=1)  # [B, max_graph_len+1]
 
         # get grid embeds
-        (grid_embeds,  # [B, max_grid_len+1, hid_dim]
-         grid_masks,  # [B, max_grid_len+1]
-         grid_labels,  # [B, grid+1, C] if mask_image == True
-         ) = self.transformer.visual_embed(
+        (
+            grid_embeds,  # [B, max_grid_len+1, hid_dim]
+            grid_masks,  # [B, max_grid_len+1]
+            grid_labels,  # [B, grid+1, C] if mask_image == True
+        ) = self.transformer.visual_embed(
             grid,
             max_image_len=self.max_grid_len,
             mask_it=mask_grid,
         )
 
         # add volume embeds to grid_embeds
         volume = torch.FloatTensor(volume).to(grid_embeds)  # [B]
         volume_embeds = self.volume_embeddings(volume[:, None, None])  # [B, 1, hid_dim]
         volume_mask = torch.ones(volume.shape[0], 1).to(grid_masks)
 
-        grid_embeds = torch.cat([grid_embeds, volume_embeds], dim=1)  # [B, max_grid_len+2, hid_dim]
+        grid_embeds = torch.cat(
+            [grid_embeds, volume_embeds], dim=1
+        )  # [B, max_grid_len+2, hid_dim]
         grid_masks = torch.cat([grid_masks, volume_mask], dim=1)  # [B, max_grid_len+2]
 
         # add token_type_embeddings
-        graph_embeds = graph_embeds \
-                       + self.token_type_embeddings(torch.zeros_like(graph_masks, device=self.device).long())
-        grid_embeds = grid_embeds \
-                      + self.token_type_embeddings(torch.ones_like(grid_masks, device=self.device).long())
+        graph_embeds = graph_embeds + self.token_type_embeddings(
+            torch.zeros_like(graph_masks, device=self.device).long()
+        )
+        grid_embeds = grid_embeds + self.token_type_embeddings(
+            torch.ones_like(grid_masks, device=self.device).long()
+        )
 
-        co_embeds = torch.cat([graph_embeds, grid_embeds], dim=1)  # [B, final_max_len, hid_dim]
-        co_masks = torch.cat([graph_masks, grid_masks], dim=1)  # [B, final_max_len, hid_dim]
+        co_embeds = torch.cat(
+            [graph_embeds, grid_embeds], dim=1
+        )  # [B, final_max_len, hid_dim]
+        co_masks = torch.cat(
+            [graph_masks, grid_masks], dim=1
+        )  # [B, final_max_len, hid_dim]
 
         x = co_embeds
 
         attn_weights = []
         for i, blk in enumerate(self.transformer.blocks):
             x, _attn = blk(x, mask=co_masks)
 
             if self.vis:
                 attn_weights.append(_attn)
 
         x = self.transformer.norm(x)
         graph_feats, grid_feats = (
-            x[:, :graph_embeds.shape[1]],
-            x[:, graph_embeds.shape[1]:],
+            x[:, : graph_embeds.shape[1]],
+            x[:, graph_embeds.shape[1] :],
         )  # [B, max_graph_len, hid_dim], [B, max_grid_len+2, hid_dim]
 
         cls_feats = self.pooler(x)  # [B, hid_dim]
 
         ret = {
             "graph_feats": graph_feats,
             "grid_feats": grid_feats,
@@ -266,15 +279,17 @@
 
     def validation_epoch_end(self, outputs):
         module_utils.epoch_wrapup(self)
 
     def test_step(self, batch, batch_idx):
         module_utils.set_task(self)
         output = self(batch)
-        output = {k : (v.cpu() if torch.is_tensor(v) else v) for k, v in output.items()} # update cpu for memory
+        output = {
+            k: (v.cpu() if torch.is_tensor(v) else v) for k, v in output.items()
+        }  # update cpu for memory
         return output
 
     def test_epoch_end(self, outputs):
         module_utils.epoch_wrapup(self)
 
         # calculate r2 score when regression
         if "regression_logits" in outputs[0].keys():
@@ -286,7 +301,10 @@
 
             if len(logits) > 1:
                 r2 = r2_score(np.array(labels), np.array(logits))
                 self.log(f"test/r2_score", r2)
 
     def configure_optimizers(self):
         return module_utils.set_schedule(self)
+
+    def lr_scheduler_step(self, scheduler, optimizer_idx, metric):
+        scheduler.step()
```

### Comparing `moftransformer-1.1.3/moftransformer/modules/module_utils.py` & `moftransformer-2.0.0/moftransformer/modules/module_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# MOFTransformer version 2.0.0
 import torch
 
 from torch.optim import AdamW
 from transformers import (
     get_polynomial_decay_schedule_with_warmup,
     get_cosine_schedule_with_warmup,
     get_constant_schedule,
@@ -56,17 +57,19 @@
                 batch_size=pl_module.hparams["config"]["per_gpu_batchsize"],
             )
             getattr(pl_module, f"{phase}_{loss_name}_mae").reset()
 
             value = -value
         else:
             value = getattr(pl_module, f"{phase}_{loss_name}_accuracy").compute()
-            pl_module.log(f"{loss_name}/{phase}/accuracy_epoch",
-                          value,
-                          batch_size=pl_module.hparams["config"]["per_gpu_batchsize"],)
+            pl_module.log(
+                f"{loss_name}/{phase}/accuracy_epoch",
+                value,
+                batch_size=pl_module.hparams["config"]["per_gpu_batchsize"],
+            )
             getattr(pl_module, f"{phase}_{loss_name}_accuracy").reset()
             pl_module.log(
                 f"{loss_name}/{phase}/loss_epoch",
                 getattr(pl_module, f"{phase}_{loss_name}_loss").compute(),
                 batch_size=pl_module.hparams["config"]["per_gpu_batchsize"],
             )
             getattr(pl_module, f"{phase}_{loss_name}_loss").reset()
@@ -99,35 +102,35 @@
 
     optimizer_grouped_parameters = [
         {
             "params": [
                 p
                 for n, p in pl_module.named_parameters()
                 if not any(nd in n for nd in no_decay)  # not within no_decay
-                   and not any(bb in n for bb in head_names)  # not within head_names
+                and not any(bb in n for bb in head_names)  # not within head_names
             ],
             "weight_decay": wd,
             "lr": lr,
         },
         {
             "params": [
                 p
                 for n, p in pl_module.named_parameters()
                 if any(nd in n for nd in no_decay)  # within no_decay
-                   and not any(bb in n for bb in head_names)  # not within head_names
+                and not any(bb in n for bb in head_names)  # not within head_names
             ],
             "weight_decay": 0.0,
             "lr": lr,
         },
         {
             "params": [
                 p
                 for n, p in pl_module.named_parameters()
                 if not any(nd in n for nd in no_decay)  # not within no_decay
-                   and any(bb in n for bb in head_names)  # within head_names
+                and any(bb in n for bb in head_names)  # within head_names
             ],
             "weight_decay": wd,
             "lr": lr * lr_mult,
         },
         {
             "params": [
                 p
@@ -137,44 +140,47 @@
             ],
             "weight_decay": 0.0,
             "lr": lr * lr_mult,
         },
     ]
 
     if optim_type == "adamw":
-        optimizer = AdamW(optimizer_grouped_parameters, lr=lr, eps=1e-8, betas=(0.9, 0.98)
-                          )
+        optimizer = AdamW(
+            optimizer_grouped_parameters, lr=lr, eps=1e-8, betas=(0.9, 0.98)
+        )
     elif optim_type == "adam":
         optimizer = torch.optim.Adam(optimizer_grouped_parameters, lr=lr)
     elif optim_type == "sgd":
         optimizer = torch.optim.SGD(optimizer_grouped_parameters, lr=lr, momentum=0.9)
 
     if pl_module.trainer.max_steps == -1:
         max_steps = pl_module.trainer.estimated_stepping_batches
     else:
         max_steps = pl_module.trainer.max_steps
 
     warmup_steps = pl_module.hparams.config["warmup_steps"]
     if isinstance(pl_module.hparams.config["warmup_steps"], float):
         warmup_steps = int(max_steps * warmup_steps)
 
-    print(f"max_epochs: {pl_module.trainer.max_epochs} | max_steps: {max_steps} | warmup_steps : {warmup_steps} "
-          f"| weight_decay : {wd} | decay_power : {decay_power}")
+    print(
+        f"max_epochs: {pl_module.trainer.max_epochs} | max_steps: {max_steps} | warmup_steps : {warmup_steps} "
+        f"| weight_decay : {wd} | decay_power : {decay_power}"
+    )
 
     if decay_power == "cosine":
         scheduler = get_cosine_schedule_with_warmup(
             optimizer,
             num_warmup_steps=warmup_steps,
             num_training_steps=max_steps,
         )
-    elif decay_power == 'constant':
+    elif decay_power == "constant":
         scheduler = get_constant_schedule(
             optimizer,
         )
-    elif decay_power == 'constant_with_warmup':
+    elif decay_power == "constant_with_warmup":
         scheduler = get_constant_schedule_with_warmup(
             optimizer,
             num_warmup_steps=warmup_steps,
         )
     else:
         scheduler = get_polynomial_decay_schedule_with_warmup(
             optimizer,
```

### Comparing `moftransformer-1.1.3/moftransformer/modules/objectives.py` & `moftransformer-2.0.0/moftransformer/modules/objectives.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# MOFTransformer version 2.0.0
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torchmetrics.functional import mean_absolute_error
 
 
 def init_weights(module):
@@ -45,15 +46,17 @@
 
     return ret
 
 
 def compute_classification(pl_module, batch):
     infer = pl_module.infer(batch)
 
-    logits, binary = pl_module.classification_head(infer["cls_feats"])  # [B, output_dim]
+    logits, binary = pl_module.classification_head(
+        infer["cls_feats"]
+    )  # [B, output_dim]
     labels = torch.LongTensor(batch["target"]).to(logits.device)  # [B]
     assert len(labels.shape) == 1
     if binary:
         logits = logits.squeeze(dim=-1)
         loss = F.binary_cross_entropy_with_logits(input=logits, target=labels.float())
     else:
         loss = F.cross_entropy(logits, labels)
@@ -64,33 +67,37 @@
         "classification_loss": loss,
         "classification_logits": logits,
         "classification_labels": labels,
     }
 
     # call update() loss and acc
     phase = "train" if pl_module.training else "val"
-    loss = getattr(pl_module, f"{phase}_classification_loss")(ret["classification_loss"])
+    loss = getattr(pl_module, f"{phase}_classification_loss")(
+        ret["classification_loss"]
+    )
     acc = getattr(pl_module, f"{phase}_classification_accuracy")(
         ret["classification_logits"], ret["classification_labels"]
     )
 
     pl_module.log(f"classification/{phase}/loss", loss)
     pl_module.log(f"classification/{phase}/accuracy", acc)
 
     return ret
 
 
 def compute_mpp(pl_module, batch):
     infer = pl_module.infer(batch, mask_grid=True)
 
     mpp_logits = pl_module.mpp_head(infer["grid_feats"])  # [B, max_image_len+2, bins]
-    mpp_logits = mpp_logits[:, :-1, :]  # ignore volume embedding, [B, max_image_len+1, bins]
+    mpp_logits = mpp_logits[
+        :, :-1, :
+    ]  # ignore volume embedding, [B, max_image_len+1, bins]
     mpp_labels = infer["grid_labels"]  # [B, max_image_len+1, C=1]
 
-    mask = mpp_labels != -100.  # [B, max_image_len, 1]
+    mask = mpp_labels != -100.0  # [B, max_image_len, 1]
 
     # masking
     mpp_logits = mpp_logits[mask.squeeze(-1)]  # [mask, bins]
     mpp_labels = mpp_labels[mask].long()  # [mask]
 
     mpp_loss = F.cross_entropy(mpp_logits, mpp_labels)
 
@@ -166,17 +173,17 @@
 
     return ret
 
 
 def compute_ggm(pl_module, batch):
     pos_len = len(batch["grid"]) // 2
     neg_len = len(batch["grid"]) - pos_len
-    ggm_labels = torch.cat(
-        [torch.ones(pos_len), torch.zeros(neg_len)]
-    ).to(pl_module.device)
+    ggm_labels = torch.cat([torch.ones(pos_len), torch.zeros(neg_len)]).to(
+        pl_module.device
+    )
 
     ggm_images = []
     for i, (bti, bfi) in enumerate(zip(batch["grid"], batch["false_grid"])):
         if ggm_labels[i] == 1:
             ggm_images.append(bti)
         else:
             ggm_images.append(bfi)
@@ -206,28 +213,31 @@
     pl_module.log(f"ggm/{phase}/loss", loss)
     pl_module.log(f"ggm/{phase}/accuracy", acc)
 
     return ret
 
 
 def compute_moc(pl_module, batch):
-
     if "bbc" in batch.keys():
         task = "bbc"
     else:
         task = "moc"
 
     infer = pl_module.infer(batch)
     moc_logits = pl_module.moc_head(
-        infer["graph_feats"][:, 1:, :]).flatten()  # [B, max_graph_len] -> [B * max_graph_len]
-    moc_labels = infer["mo_labels"].to(moc_logits).flatten()  # [B, max_graph_len] -> [B * max_graph_len]
+        infer["graph_feats"][:, 1:, :]
+    ).flatten()  # [B, max_graph_len] -> [B * max_graph_len]
+    moc_labels = (
+        infer["mo_labels"].to(moc_logits).flatten()
+    )  # [B, max_graph_len] -> [B * max_graph_len]
     mask = moc_labels != -100
 
-    moc_loss = F.binary_cross_entropy_with_logits(input=moc_logits[mask],
-                                                  target=moc_labels[mask])  # [B * max_graph_len]
+    moc_loss = F.binary_cross_entropy_with_logits(
+        input=moc_logits[mask], target=moc_labels[mask]
+    )  # [B * max_graph_len]
 
     ret = {
         "moc_loss": moc_loss,
         "moc_logits": moc_logits,
         "moc_labels": moc_labels,
     }
 
@@ -237,8 +247,8 @@
     acc = getattr(pl_module, f"{phase}_{task}_accuracy")(
         nn.Sigmoid()(ret["moc_logits"]), ret["moc_labels"].long()
     )
 
     pl_module.log(f"{task}/{phase}/loss", loss)
     pl_module.log(f"{task}/{phase}/accuracy", acc)
 
-    return ret
+    return ret
```

### Comparing `moftransformer-1.1.3/moftransformer/modules/vision_transformer_3d.py` & `moftransformer-2.0.0/moftransformer/modules/vision_transformer_3d.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# MOFTransformer version 2.0.0
 """ Vision Transformer (ViT) in PyTorch
 
 A PyTorch implement of Vision Transformers as described in
 'An Image Is Worth 16 x 16 Words: Transformers for Image Recognition at Scale' - https://arxiv.org/abs/2010.11929
 
 The official jax code is released and available at https://github.com/google-research/vision_transformer
 
@@ -26,20 +27,20 @@
 
 from torch.nn import AvgPool3d
 from timm.models.layers import DropPath, trunc_normal_
 
 
 class Mlp(nn.Module):
     def __init__(
-            self,
-            in_features,
-            hidden_features=None,
-            out_features=None,
-            act_layer=nn.GELU,
-            drop=0.0,
+        self,
+        in_features,
+        hidden_features=None,
+        out_features=None,
+        act_layer=nn.GELU,
+        drop=0.0,
     ):
         super().__init__()
         out_features = out_features or in_features
         hidden_features = hidden_features or in_features
         self.fc1 = nn.Linear(in_features, hidden_features)
         self.act = act_layer()
         self.fc2 = nn.Linear(hidden_features, out_features)
@@ -52,73 +53,77 @@
         x = self.fc2(x)
         x = self.drop(x)
         return x
 
 
 class Attention(nn.Module):
     def __init__(
-            self,
-            dim,
-            num_heads=8,
-            qkv_bias=False,
-            qk_scale=None,
-            attn_drop=0.0,
-            proj_drop=0.0,
+        self,
+        dim,
+        num_heads=8,
+        qkv_bias=False,
+        qk_scale=None,
+        attn_drop=0.0,
+        proj_drop=0.0,
     ):
         super().__init__()
         self.num_heads = num_heads
         head_dim = dim // num_heads
         # NOTE scale factor was wrong in my original version, can set manually to be compat with prev weights
-        self.scale = qk_scale or head_dim ** -0.5
+        self.scale = qk_scale or head_dim**-0.5
 
         self.qkv = nn.Linear(dim, dim * 3, bias=qkv_bias)
         self.attn_drop = nn.Dropout(attn_drop)
         self.proj = nn.Linear(dim, dim)
         self.proj_drop = nn.Dropout(proj_drop)
 
     def forward(self, x, mask=None):
         B, N, C = x.shape
         assert C % self.num_heads == 0
         qkv = (
             self.qkv(x)  # [B, N, 3*C]
-                .reshape(B, N, 3, self.num_heads, C // self.num_heads)  # [B, N, 3, num_heads, C//num_heads]
-                .permute(2, 0, 3, 1, 4)  # [3, B, num_heads, N, C//num_heads]
+            .reshape(
+                B, N, 3, self.num_heads, C // self.num_heads
+            )  # [B, N, 3, num_heads, C//num_heads]
+            .permute(2, 0, 3, 1, 4)  # [3, B, num_heads, N, C//num_heads]
         )
         q, k, v = (
             qkv[0],  # [B, num_heads, N, C//num_heads]
             qkv[1],  # [B, num_heads, N, C//num_heads]
             qkv[2],  # [B, num_heads, N, C//num_heads]
         )  # make torchscript happy (cannot use tensor as tuple)
 
         attn = (q @ k.transpose(-2, -1)) * self.scale  # [B, num_heads, N, N]
         if mask is not None:
             mask = mask.bool()
             attn = attn.masked_fill(~mask[:, None, None, :], float("-inf"))
         attn = attn.softmax(dim=-1)  # [B, num_heads, N, N]
         attn = self.attn_drop(attn)
 
-        x = (attn @ v).transpose(1, 2).reshape(B, N, C)  # [B, num_heads, N, C//num_heads] -> [B, N, C]
+        x = (
+            (attn @ v).transpose(1, 2).reshape(B, N, C)
+        )  # [B, num_heads, N, C//num_heads] -> [B, N, C]
         x = self.proj(x)
         x = self.proj_drop(x)
         return x, attn
 
 
 class Block(nn.Module):
     def __init__(
-            self,
-            dim,
-            num_heads,
-            mlp_ratio=4.0,
-            qkv_bias=False,
-            qk_scale=None,
-            drop=0.0,
-            attn_drop=0.0,
-            drop_path=0.0,
-            act_layer=nn.GELU,
-            norm_layer=nn.LayerNorm,
+        self,
+        dim,
+        num_heads,
+        mlp_ratio=4.0,
+        qkv_bias=False,
+        qk_scale=None,
+        drop=0.0,
+        attn_drop=0.0,
+        drop_path=0.0,
+        act_layer=nn.GELU,
+        norm_layer=nn.LayerNorm,
     ):
         super().__init__()
         self.norm1 = norm_layer(dim)
         self.attn = Attention(
             dim,
             num_heads=num_heads,
             qkv_bias=qkv_bias,
@@ -141,68 +146,72 @@
         _x, attn = self.attn(self.norm1(x), mask=mask)
         x = x + self.drop_path(_x)
         x = x + self.drop_path(self.mlp(self.norm2(x)))
         return x, attn
 
 
 class PatchEmbed3D(nn.Module):
-    """ Image to Patch Embedding for 3D"""
+    """Image to Patch Embedding for 3D"""
 
     def __init__(
-            self,
-            img_size,  # minimum of H or W ex. 384
-            patch_size,  # p -> length of fixed patch ex. 32
-            in_chans=1,
-            embed_dim=768,
-            no_patch_embed_bias=False,
+        self,
+        img_size,  # minimum of H or W ex. 384
+        patch_size,  # p -> length of fixed patch ex. 32
+        in_chans=1,
+        embed_dim=768,
+        no_patch_embed_bias=False,
     ):
         super().__init__()
 
         assert img_size % patch_size == 0
-        num_patches = (img_size ** 3) // (patch_size ** 3)
+        num_patches = (img_size**3) // (patch_size**3)
         self.img_size = img_size  # default: 30
         self.patch_size = patch_size  # default: 5
         self.num_patches = num_patches
 
         self.proj = nn.Sequential(
-            Rearrange('b c (h p1) (w p2) (d p3) -> b (h w d) (p1 p2 p3 c)',
-                      p1=patch_size, p2=patch_size, p3=patch_size),
+            Rearrange(
+                "b c (h p1) (w p2) (d p3) -> b (h w d) (p1 p2 p3 c)",
+                p1=patch_size,
+                p2=patch_size,
+                p3=patch_size,
+            ),
             nn.Linear(patch_size * patch_size * patch_size * in_chans, embed_dim),
         )
 
     def forward(self, x):
         x = self.proj(x)  # [B, num_patches,
         return x  # [B, emb_dim, px, ph, pd]
 
 
 class VisionTransformer3D(nn.Module):
-    """ Vision Transformer
+    """Vision Transformer
 
     A PyTorch impl of : `An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale`  -
         https://arxiv.org/abs/2010.11929
     """
 
     def __init__(
-            self,
-            img_size,
-            patch_size,
-            in_chans,
-            embed_dim,
-            depth=12,
-            num_heads=12,
-            mlp_ratio=4.0,
-            qkv_bias=True,
-            qk_scale=None,
-            drop_rate=0.0,
-            attn_drop_rate=0.0,
-            drop_path_rate=0.0,
-            norm_layer=None,
-            add_norm_before_transformer=False,
-            mpp_ratio=0.15,
-            config=None,
+        self,
+        img_size,
+        patch_size,
+        in_chans,
+        embed_dim,
+        depth=12,
+        num_heads=12,
+        mlp_ratio=4.0,
+        qkv_bias=True,
+        qk_scale=None,
+        drop_rate=0.0,
+        attn_drop_rate=0.0,
+        drop_path_rate=0.0,
+        norm_layer=None,
+        add_norm_before_transformer=False,
+        mpp_ratio=0.15,
+        config=None,
     ):
         """
         Args:
             img_size (int, tuple): input image size
             patch_size (int, tuple): patch size
             in_chans (int): number of input channels
             embed_dim (int): embedding dimension
@@ -290,23 +299,25 @@
 
         m = AvgPool3d(patch_size, patch_size)
         with torch.no_grad():
             img_patch = m(orig_image)
 
         labels = (
             (img_patch.long().flatten(start_dim=2, end_dim=4))  # [B, C, ph*pw*pd]
-                .permute(0, 2, 1)
-                .contiguous()
+            .permute(0, 2, 1)
+            .contiguous()
         )  # [B, ph*pw*pd, C]
 
         # We sample a few tokens in each sequence for MLM training (with probability `self.mlm_probability`)
         # probability_matrix = torch.full(labels.shape[:-1], 0.15)  # [B, ph*pw*pd]
         probability_matrix = torch.full(labels.shape[:-1], mpp_ratio)  # [B, ph*pw*pd]
         masked_indices = torch.bernoulli(probability_matrix).bool()
-        labels[~masked_indices] = -100  # We only compute loss on masked tokens [B, ph*pw*pd, C]
+        labels[
+            ~masked_indices
+        ] = -100  # We only compute loss on masked tokens [B, ph*pw*pd, C]
         """
         # 80% of the time, we replace masked input tokens with tokenizer.mask_token ([MASK])
         indices_replaced = (
                 torch.bernoulli(torch.full(labels.shape[:-1], 0.8)).bool() & masked_indices
         )  # [B, ph*pw*pd]
 
         feats[indices_replaced] = self.mask_token.to(feats)
@@ -328,18 +339,20 @@
 
         B, _, _, _, _ = _x.shape
         x = self.patch_embed(_x)  # [B, ph*pw*pd, embed_dim]
         # x = x.flatten(2).transpose(1, 2)
 
         # mpp
         if mask_it:
-            x, label = self.mask_tokens(_x, x, self.patch_size,
-                                        self.mpp_ratio)  # [B, ph*pw*pd, emb_dim], [B, ph*pw*pd, C]
+            x, label = self.mask_tokens(
+                _x, x, self.patch_size, self.mpp_ratio
+            )  # [B, ph*pw*pd, emb_dim], [B, ph*pw*pd, C]
             label = torch.cat(
-                [torch.full((label.shape[0], 1, self.in_chans), -100).to(label), label], dim=1,
+                [torch.full((label.shape[0], 1, self.in_chans), -100).to(label), label],
+                dim=1,
             )  # [B, max_len+1, C]
 
         # cls tokens
         cls_token = self.cls_token.expand(B, -1, -1)  # [B, 1, embed_dim]
         x = torch.cat([cls_token, x], dim=1)  # [B, ph*pw*pd, embed_dim]
 
         # positional embedding
```

### Comparing `moftransformer-1.1.3/moftransformer/run.py` & `moftransformer-2.0.0/moftransformer/run_cp.py`

 * *Files identical despite different names*

### Comparing `moftransformer-1.1.3/moftransformer/utils/download.py` & `moftransformer-2.0.0/moftransformer/utils/download.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,166 +1,185 @@
+# MOFTransformer version 2.0.0
 import os
 import wget
 import tarfile
 from pathlib import Path
-from moftransformer.database import DEFAULT_PRETRAIN_MODEL_PATH, DEFAULT_COREMOF_PATH, DEFAULT_QMOF_PATH, \
-    DEFAULT_FINETUNED_MODEL_PATH, DEFAULT_HMOF_PATH
+from moftransformer.database import (
+    DEFAULT_PRETRAIN_MODEL_PATH,
+    DEFAULT_COREMOF_PATH,
+    DEFAULT_QMOF_PATH,
+    DEFAULT_FINETUNED_MODEL_PATH,
+    DEFAULT_HMOF_PATH,
+)
 
 
 class DownloadError(Exception):
     pass
 
 
-def _remove_tmp_file(direc:Path):
-    tmp_list = direc.parent.glob('*.tmp')
+def _remove_tmp_file(direc: Path):
+    tmp_list = direc.parent.glob("*.tmp")
     for tmp in tmp_list:
         if tmp.exists():
             os.remove(tmp)
 
 
-def _download_file(link, direc, name='target'):
+def _download_file(link, direc, name="target"):
     if direc.exists():
-        print (f'{name} already exists.')
+        print(f"{name} already exists.")
         return
     try:
-        print(f'\n====Download {name} =============================================\n')
+        print(f"\n====Download {name} =============================================\n")
         filename = wget.download(link, out=str(direc))
     except KeyboardInterrupt:
         _remove_tmp_file(direc)
         raise
     except Exception as e:
         _remove_tmp_file(direc)
         raise DownloadError(e)
     else:
-        print (f'\n====Successfully download : {filename}=======================================\n')
+        print(
+            f"\n====Successfully download : {filename}=======================================\n"
+        )
 
 
-def download_pretrain_model(direc=None, ):
+def download_pretrain_model(
+    direc=None,
+):
     if not direc:
         direc = Path(DEFAULT_PRETRAIN_MODEL_PATH)
     else:
         direc = Path(direc)
 
-    if not direc.suffix:
-        if not direc.exists():
-            direc.mkdir(parents=True, exist_ok=True)
-        direc = direc / 'pretrained_model.ckpt'
-    elif direc.suffix == '.ckpt':
-        if not direc.parent.exists():
-            direc.parent.mkdir(parents=True, exist_ok=True)
-    else:
-        raise ValueError(f'direc must be path for directory or ~.ckpt, not {direc}')
+    if not direc.is_dir():
+        raise ValueError(f"direc must be path for directory, not {direc}")
+    if not direc.exists():
+        direc.mkdir(parents=True, exist_ok=True)
 
-    link = 'https://figshare.com/ndownloader/files/37511767'
-    name = 'pretrain_model'
-    _download_file(link, direc, name)
+    # download pmtransformer
+    link = "https://figshare.com/ndownloader/files/40298992"
+    name = "pmtransformer"
+    _download_file(link, direc / 'pmtransformer.ckpt', name)
+
+    # download moftransformer
+    link ="https://figshare.com/ndownloader/files/40298269"
+    name = 'moftransformer'
+    _download_file(link, direc / 'moftransformer.ckpt', name)
 
 
-def download_finetuned_model(direc=None, ):
+def download_finetuned_model(
+    direc=None,
+):
     if not direc:
         direc = Path(DEFAULT_FINETUNED_MODEL_PATH)
         if not direc.exists():
             direc.mkdir(parents=True, exist_ok=True)
     else:
         direc = Path(direc)
         if not direc.suffix:
             if not direc.exists():
                 direc.mkdir(parents=True, exist_ok=True)
         else:
-            raise ValueError(f'direc must be path for directory, not {direc}')
+            raise ValueError(f"direc must be path for directory, not {direc}")
 
-    link = 'https://figshare.com/ndownloader/files/37621520'
-    name = 'finetuned_bandgap'
-    _download_file(link, direc / 'finetuned_bandgap.ckpt', name)
-
-    link = 'https://figshare.com/ndownloader/files/37622693'
-    name = 'finetuned_h2_uptake'
-    _download_file(link, direc / 'finetuned_h2_uptake.ckpt', name)
+    # download band-gap model
+    link = "https://figshare.com/ndownloader/files/37621520"
+    name = "finetuned_bandgap"
+    _download_file(link, direc / "finetuned_bandgap.ckpt", name)
+
+    # download uptake model
+    link = "https://figshare.com/ndownloader/files/37622693"
+    name = "finetuned_h2_uptake"
+    _download_file(link, direc / "finetuned_h2_uptake.ckpt", name)
 
 
 def download_coremof(direc=None, remove_tarfile=False):
     if not direc:
         direc = Path(DEFAULT_COREMOF_PATH)
     else:
         direc = Path(direc)
 
     if direc.suffix:
-       raise ValueError(f'direc must be directory, not {direc}')
-    elif (direc/'raw/GIRGUL_clean.grid').exists():
-        print ('CoREMOF database is already existed')
+        raise ValueError(f"direc must be directory, not {direc}")
+    elif (direc / "raw/GIRGUL_clean.grid").exists():
+        print("CoREMOF database is already existed")
         return
     elif not direc.exists():
         direc.mkdir(parents=True, exist_ok=True)
-    direc = direc/'coremof.tar.gz'
+    direc = direc / "coremof.tar.gz"
 
-    link = 'https://figshare.com/ndownloader/files/37511746'
-    name = 'coremof_database'
+    link = "https://figshare.com/ndownloader/files/37511746"
+    name = "coremof_database"
     _download_file(link, direc, name)
 
-    print(f'\n====Unzip : {direc}===============================================\n')
+    print(f"\n====Unzip : {direc}===============================================\n")
     with tarfile.open(direc) as f:
         f.extractall(path=direc.parent)
 
-    print(f'\n====Unzip successfully: {direc}===============================================\n')
+    print(
+        f"\n====Unzip successfully: {direc}===============================================\n"
+    )
 
     if remove_tarfile:
         os.remove(direc)
 
 
 def download_qmof(direc=None, remove_tarfile=False):
     if not direc:
         direc = Path(DEFAULT_QMOF_PATH)
     else:
         direc = Path(direc)
 
     if direc.suffix:
-       raise ValueError(f'direc must be directory, not {direc}')
-    elif (direc/'raw/JORCOK_FSR.grid').exists():
-        print ('QMOF database is already existed')
+        raise ValueError(f"direc must be directory, not {direc}")
+    elif (direc / "raw/JORCOK_FSR.grid").exists():
+        print("QMOF database is already existed")
         return
     elif not direc.exists():
         direc.mkdir(parents=True, exist_ok=True)
-    direc = direc/'qmof.tar.gz'
-
+    direc = direc / "qmof.tar.gz"
 
-    link = 'https://figshare.com/ndownloader/files/37511758'
-    name = 'qmof_database'
+    link = "https://figshare.com/ndownloader/files/37511758"
+    name = "qmof_database"
     _download_file(link, direc, name)
 
-    print(f'\n====Unzip : {direc}===============================================\n')
+    print(f"\n====Unzip : {direc}===============================================\n")
     with tarfile.open(direc) as f:
         f.extractall(path=direc.parent)
 
-    print(f'\n====Unzip successfully: {direc}===============================================\n')
+    print(
+        f"\n====Unzip successfully: {direc}===============================================\n"
+    )
 
     if remove_tarfile:
         os.remove(direc)
 
 
-
 def download_hmof(direc=None, remove_tarfile=False):
     if not direc:
         direc = Path(DEFAULT_HMOF_PATH)
     else:
         direc = Path(direc)
 
     if direc.suffix:
-       raise ValueError(f'direc must be directory, not {direc}')
-    elif (direc/'downstream_release/train_raspa_100bar.json').exists():
-        print ('hMOF database is already existed')
+        raise ValueError(f"direc must be directory, not {direc}")
+    elif (direc / "downstream_release/train_raspa_100bar.json").exists():
+        print("hMOF database is already existed")
         return
     elif not direc.exists():
         direc.mkdir(parents=True, exist_ok=True)
-    direc = direc/'hmof.tar.gz'
+    direc = direc / "hmof.tar.gz"
 
-    link = 'https://figshare.com/ndownloader/files/37511755'
-    name = 'hmof_database'
+    link = "https://figshare.com/ndownloader/files/37511755"
+    name = "hmof_database"
     _download_file(link, direc, name)
 
-    print(f'\n====Unzip : {direc}===============================================\n')
+    print(f"\n====Unzip : {direc}===============================================\n")
     with tarfile.open(direc) as f:
         f.extractall(path=direc.parent)
 
-    print(f'\n====Unzip successfully: {direc}===============================================\n')
+    print(
+        f"\n====Unzip successfully: {direc}===============================================\n"
+    )
 
     if remove_tarfile:
         os.remove(direc)
```

### Comparing `moftransformer-1.1.3/moftransformer/utils/install_griday.py` & `moftransformer-2.0.0/moftransformer/utils/install_griday.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,85 @@
+# MOFTransformer version 2.0.0
 import subprocess
 from pathlib import Path
 from moftransformer.utils.prepare_data import GRIDAY_PATH
 
-__all__ = ['install_griday', 'uninstall_griday']
+__all__ = ["install_griday", "uninstall_griday"]
 
 
 class InstallationError(Exception):
     def __init__(self, error_message=None):
         self.error_message = error_message
 
     def __str__(self):
         if self.error_message:
             return f"Installation Error : {self.error_message}"
         return "Installation Error"
 
 
 def _install_make():
-    print ('=== Download gcc=9.5.0 =========================================================')
-    ps = subprocess.run('conda install -c conda-forge gcc=9.5.0 -y'.split())
+    print(
+        "=== Download gcc=9.5.0 ========================================================="
+    )
+    ps = subprocess.run("conda install -c conda-forge gcc=9.5.0 -y".split())
     if ps.returncode:
         raise InstallationError(ps.stderr)
     else:
-        print ('=== Successfully download =======================================================')
-    print ('=== Download gxx=9.5.0 =========================================================')
-    ps = subprocess.run('conda install -c conda-forge gxx=9.5.0 -y'.split())
+        print(
+            "=== Successfully download ======================================================="
+        )
+    print(
+        "=== Download gxx=9.5.0 ========================================================="
+    )
+    ps = subprocess.run("conda install -c conda-forge gxx=9.5.0 -y".split())
     if ps.returncode:
         raise InstallationError(ps.stderr)
     else:
-        print ('=== Successfully download =======================================================')
-    print ('=== Download make=4.2.1 ===============================================================')
-    ps = subprocess.run('conda install -c anaconda make=4.2.1 -y'.split())
+        print(
+            "=== Successfully download ======================================================="
+        )
+    print(
+        "=== Download make=4.2.1 ==============================================================="
+    )
+    ps = subprocess.run("conda install -c anaconda make=4.2.1 -y".split())
     if ps.returncode:
         raise InstallationError(ps.stderr)
     else:
-        print ('=== Successfully download =======================================================')
+        print(
+            "=== Successfully download ======================================================="
+        )
 
 
 def _make_griday():
     dir_griday = Path(GRIDAY_PATH).parent.parent
     if not dir_griday.exists():
-        raise InstallationError(f'Invalid path specified : {dir_griday}')
-    print('=== Install GRIDAY ==============================================================')
-    ps = subprocess.run(['make'], cwd=dir_griday)
+        raise InstallationError(f"Invalid path specified : {dir_griday}")
+    print(
+        "=== Install GRIDAY =============================================================="
+    )
+    ps = subprocess.run(["make"], cwd=dir_griday)
     if ps.returncode:
         raise InstallationError(ps.stderr)
-    ps = subprocess.run(['make'], cwd=dir_griday/'scripts')
+    ps = subprocess.run(["make"], cwd=dir_griday / "scripts")
     if ps.returncode:
         raise InstallationError(ps.stderr)
-    print('=== Successfully download =======================================================')
+    print(
+        "=== Successfully download ======================================================="
+    )
     if Path(GRIDAY_PATH).exists():
-        print(f'GRIDAY is installed to {dir_griday}')
+        print(f"GRIDAY is installed to {dir_griday}")
     else:
-        raise InstallationError(f'GRIDAY is not installed. Please try again.')
+        raise InstallationError(f"GRIDAY is not installed. Please try again.")
 
 
 def install_griday(install_make=False):
     """
     Installation a GRIDAY which calculates the energy grid for prepare-data.py
     Original code : https://github.com/Sangwon91/GRIDAY.git
-    
+
     :Param install_make : (bool) if True, install gcc, g++, and make
 
     :return: None
     """
     if install_make:
         _install_make()
     _make_griday()
@@ -73,25 +90,29 @@
     Remove a GRIDAY which calculates the energy grid for prepare-data.py
     Original code : https://github.com/Sangwon91/GRIDAY.git
     :return:
     """
 
     dir_griday = Path(GRIDAY_PATH).parent.parent
     if not dir_griday.exists():
-        raise InstallationError(f'Invalid path specified : {dir_griday}')
-    print('=== Uninstall GRIDAY ============================================================')
-    ps = subprocess.run(['make', 'clean'], cwd=dir_griday)
+        raise InstallationError(f"Invalid path specified : {dir_griday}")
+    print(
+        "=== Uninstall GRIDAY ============================================================"
+    )
+    ps = subprocess.run(["make", "clean"], cwd=dir_griday)
     if ps.returncode:
         raise InstallationError(ps.stderr)
-    ps = subprocess.run(['make', 'clean'], cwd=dir_griday / 'scripts')
+    ps = subprocess.run(["make", "clean"], cwd=dir_griday / "scripts")
     if ps.returncode:
         raise InstallationError(ps.stderr)
-    print('=== Successfully remove  =========================================================')
+    print(
+        "=== Successfully remove  ========================================================="
+    )
 
     if not Path(GRIDAY_PATH).exists():
-        print(f'GRIDAY is uninstalled')
+        print(f"GRIDAY is uninstalled")
     else:
         raise InstallationError()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     install_griday()
```

### Comparing `moftransformer-1.1.3/moftransformer/utils/prepare_data.py` & `moftransformer-2.0.0/moftransformer/utils/prepare_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 from ase.io import read
 from ase.neighborlist import natural_cutoffs
 from ase import neighborlist
 from ase.build import make_supercell
 
 from moftransformer import __root_dir__
 
-GRIDAY_PATH = os.path.join(__root_dir__, 'libs/GRIDAY/scripts/grid_gen')
-FF_PATH = os.path.join(__root_dir__, 'libs/GRIDAY/FF')
+GRIDAY_PATH = os.path.join(__root_dir__, "libs/GRIDAY/scripts/grid_gen")
+FF_PATH = os.path.join(__root_dir__, "libs/GRIDAY/FF")
 
 
 def get_logger(filename):
     logger = logging.getLogger(filename)
     logger.setLevel(logging.INFO)
 
-    formatter = logging.Formatter(fmt="%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+    formatter = logging.Formatter(
+        fmt="%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+    )
 
     # stream_handler = logging.StreamHandler()
     # stream_handler.setFormatter(formatter)
     # logger.addHandler(stream_handler)
 
     file_handler = logging.FileHandler(filename)
     file_handler.setFormatter(formatter)
@@ -45,15 +47,17 @@
 
     return logger
 
 
 def get_unique_atoms(atoms):
     # get graph
     cutoff = natural_cutoffs(atoms)
-    neighbor_list = neighborlist.NeighborList(cutoff, self_interaction=True, bothways=True)
+    neighbor_list = neighborlist.NeighborList(
+        cutoff, self_interaction=True, bothways=True
+    )
     neighbor_list.update(atoms)
     matrix = neighbor_list.get_connectivity_matrix()
 
     # Get N, N^2
     numbers = atoms.numbers
     number_sqr = np.multiply(numbers, numbers)
 
@@ -69,15 +73,17 @@
 
     for m in list_m:
         for n in list_n:
             arr.append(m.dot(n))
 
     arr = np.vstack(arr).transpose()
 
-    uni, unique_idx, unique_count = np.unique(arr, axis=0, return_index=True, return_counts=True)
+    uni, unique_idx, unique_count = np.unique(
+        arr, axis=0, return_index=True, return_counts=True
+    )
 
     # sort
     final_uni = uni[np.argsort(-unique_count)].tolist()
     final_unique_count = unique_count[np.argsort(-unique_count)].tolist()
 
     arr = arr.tolist()
     final_unique_idx = []
@@ -142,23 +148,34 @@
 def get_energy_grid(atoms, cif_id, root_dataset, eg_logger):
     # Before 1.1.1 version : num_grid = [str(round(cell)) for cell in structure.lattice.abc]
     # After 1.1.1 version : num_grid = [30, 30, 30]
     global GRIDAY_PATH, FF_PATH
 
     eg_file = os.path.join(root_dataset, cif_id)
     random_str = str(np.random.rand()).encode()
-    tmp_file = os.path.join(root_dataset, f"{hashlib.sha256(random_str).hexdigest()}.cssr")
+    tmp_file = os.path.join(
+        root_dataset, f"{hashlib.sha256(random_str).hexdigest()}.cssr"
+    )
 
     try:
         structure = AseAtomsAdaptor().get_structure(atoms)
         Cssr(structure).write_file(tmp_file)
-        num_grid = ['30', '30', '30']
+        num_grid = ["30", "30", "30"]
         proc = subprocess.Popen(
-            [GRIDAY_PATH, *num_grid, f'{FF_PATH}/UFF_Type.def', f'{FF_PATH}/UFF_FF.def', tmp_file, eg_file],
-            stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            [
+                GRIDAY_PATH,
+                *num_grid,
+                f"{FF_PATH}/UFF_Type.def",
+                f"{FF_PATH}/UFF_FF.def",
+                tmp_file,
+                eg_file,
+            ],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
         out, err = proc.communicate()
     finally:
         # remove temp_file
         if os.path.exists(tmp_file):
             os.remove(tmp_file)
 
     if err:
@@ -195,92 +212,98 @@
         - duplicate : (bool) If True, allow duplication of data in train, test, and validation. (default: False)
         - train_fraction : (float) fraction for train dataset. train_fraction + test_fraction must be smaller than 1 (default : 0.8)
         - test_fraction : (float) fraction for test dataset. train_fraction + test_fraction must be smaller than 1 (default : 0.1)
 
     :return:
     """
     # get argument from kwargs
-    seed = kwargs.get('seed', 42)
-    threshold = kwargs.get('threshold', 0.01)
-    train_fraction = kwargs.get('train_fraction', 0.8)
-    test_fraction = kwargs.get('test_fraction', 0.1)
+    seed = kwargs.get("seed", 42)
+    threshold = kwargs.get("threshold", 0.01)
+    train_fraction = kwargs.get("train_fraction", 0.8)
+    test_fraction = kwargs.get("test_fraction", 0.1)
 
     # get directories
-    total_dir = root_dataset / 'total'
+    total_dir = root_dataset / "total"
     assert total_dir.exists()
 
-    split_dir = {split: root_dataset / split for split in ['train', 'test', 'val']}
+    split_dir = {split: root_dataset / split for split in ["train", "test", "val"]}
     for direc in split_dir.values():
         direc.mkdir(exist_ok=True)
 
     # get success prepare-data list
     cif_list = {}
-    CifPath = namedtuple('CifPath', ['cif', 'graphdata', 'grid', 'griddata16'])
-    for cif in total_dir.glob('*.cif'):
+    CifPath = namedtuple("CifPath", ["cif", "graphdata", "grid", "griddata16"])
+    for cif in total_dir.glob("*.cif"):
         cif_id = cif.stem
-        graphdata = cif.with_suffix('.graphdata')
-        grid = cif.with_suffix('.grid')
-        griddata = cif.with_suffix('.griddata16')
+        graphdata = cif.with_suffix(".graphdata")
+        grid = cif.with_suffix(".grid")
+        griddata = cif.with_suffix(".griddata16")
 
         if cif.exists() and graphdata.exists() and grid.exists() and griddata.exists():
             cif_list[cif_id] = CifPath(cif, graphdata, grid, griddata)
 
     # get number of split
     if train_fraction + test_fraction > 1:
         raise ValueError(
-            f'"train_fraction + test_fraction" must be smaller than 1.0, not {train_fraction + test_fraction}')
+            f'"train_fraction + test_fraction" must be smaller than 1.0, not {train_fraction + test_fraction}'
+        )
 
     n_total = len(cif_list.keys())
     n_train = int(n_total * train_fraction)
     n_test = int(n_total * test_fraction)
     n_val = n_total - n_train - n_test
-    n_split = {'train': n_train, 'test': n_test, 'val': n_val}
+    n_split = {"train": n_train, "test": n_test, "val": n_val}
 
     # remove already-divided values
     for split, direc in split_dir.items():
-        split_cifs = {cif.stem for cif in direc.glob('*.cif')}
+        split_cifs = {cif.stem for cif in direc.glob("*.cif")}
         for cif in split_cifs:
             if cif in cif_list:
                 del cif_list[cif]
                 n_split[split] -= 1
 
-    assert sum(n_split.values()) == len(cif_list), 'Error! contact with code writer!'
+    assert sum(n_split.values()) == len(cif_list), "Error! contact with code writer!"
     if not cif_list:  # NO additional divided task
         return
 
     for split, n in n_split.items():
         if n < -n_total * threshold:
             raise ValueError(
-                "{split} folder's cif number is larger than {split}_fraction. change argument {split}_fraction.")
+                "{split} folder's cif number is larger than {split}_fraction. change argument {split}_fraction."
+            )
 
     # random split index
     cif_name = sorted(list(cif_list.keys()))
-    split_idx = ['train'] * n_split['train'] + ['test'] * n_split['test'] + ['val'] * n_split['val']
+    split_idx = (
+        ["train"] * n_split["train"]
+        + ["test"] * n_split["test"]
+        + ["val"] * n_split["val"]
+    )
     np.random.seed(seed=seed)
     np.random.shuffle(split_idx)
 
     assert len(cif_name) == len(split_idx)
 
     for cif, split in zip(cif_name, split_idx):
         cifpath = cif_list[cif]
-        for suffix in ['cif', 'graphdata', 'grid', 'griddata16']:
+        for suffix in ["cif", "graphdata", "grid", "griddata16"]:
             src = getattr(cifpath, suffix)
             dest = root_dataset / split
             shutil.copy(src, dest)
 
 
 def _split_json(root_cifs: Path, root_dataset: Path, downstream: str):
-    with open(str(root_cifs / f'raw_{downstream}.json')) as f:
+    with open(str(root_cifs / f"raw_{downstream}.json")) as f:
         src = json.load(f)
 
-    for split in ['train', 'test', 'val']:
+    for split in ["train", "test", "val"]:
         cif_folder = root_dataset / split
-        cif_list = [cif.stem for cif in cif_folder.glob('*.cif')]
+        cif_list = [cif.stem for cif in cif_folder.glob("*.cif")]
         split_json = {i: src[i] for i in cif_list if i in src}
-        with open(str(root_dataset / f'{split}_{downstream}.json'), 'w') as f:
+        with open(str(root_dataset / f"{split}_{downstream}.json"), "w") as f:
             json.dump(split_json, f)
 
 
 def _make_supercell(atoms, cutoff):
     """
     make atoms into supercell when cell length is less than cufoff (min_length)
     """
@@ -295,30 +318,33 @@
     # make supercell
     m = np.zeros([3, 3])
     np.fill_diagonal(m, scale_abc)
     atoms = make_supercell(atoms, m)
     return atoms
 
 
-def make_prepared_data(cif: Path, root_dataset_total: Path, logger=None, eg_logger=None, **kwargs):
+def make_prepared_data(
+    cif: Path, root_dataset_total: Path, logger=None, eg_logger=None, **kwargs
+):
     if logger is None:
         logger = get_logger(filename="prepare_data.log")
     if eg_logger is None:
         eg_logger = get_logger(filename="prepare_energy_grid.log")
 
     if isinstance(cif, str):
         cif = Path(cif)
     if isinstance(root_dataset_total, str):
         root_dataset_total = Path(root_dataset_total)
 
     root_dataset_total.mkdir(exist_ok=True, parents=True)
 
-    max_length = kwargs.get('max_length', 60.)
-    min_length = kwargs.get('min_length', 30.)
-    max_num_nbr = kwargs.get('max_num_nbr', 12)
+    max_length = kwargs.get("max_length", 60.0)
+    min_length = kwargs.get("min_length", 30.0)
+    max_num_nbr = kwargs.get("max_num_nbr", 12)
+    max_num_atoms = kwargs.get("max_num_atoms", 300)
 
     cif_id: str = cif.stem
 
     p_graphdata = root_dataset_total / f"{cif_id}.graphdata"
     p_griddata = root_dataset_total / f"{cif_id}.griddata16"
     p_grid = root_dataset_total / f"{cif_id}.grid"
 
@@ -339,18 +365,28 @@
     try:
         atoms = read(str(cif))
     except Exception as e:
         logger.info(f"{cif_id} failed : {e}")
         return False
 
     # 1. get crystal graph
-    atoms = _make_supercell(atoms, cutoff=8) # radius = 8
-    atom_num, nbr_idx, nbr_dist, uni_idx, uni_count = get_crystal_graph(atoms, radius=8, max_num_nbr=max_num_nbr)
+    atoms = _make_supercell(atoms, cutoff=8)  # radius = 8
+    atom_num, nbr_idx, nbr_dist, uni_idx, uni_count = get_crystal_graph(
+        atoms, radius=8, max_num_nbr=max_num_nbr
+    )
     if len(nbr_idx) < len(atom_num) * max_num_nbr:
-        logger.info(f"{cif_id} failed : num_nbr is smaller than max_num_nbr. please make radius larger")
+        logger.info(
+            f"{cif_id} failed : num_nbr is smaller than max_num_nbr. please make radius larger"
+        )
+        return False
+
+    if len(uni_idx) > max_num_atoms:
+        logger.info(
+            f"{cif_id} failed : The number of topologically unique atoms is larget than max_num_atoms ({max_num_atoms})"
+        )
         return False
 
     # 2. make supercell with min_length
     atoms_eg = _make_supercell(atoms, cutoff=min_length)
     for l in atoms_eg.cell.cellpar()[:3]:
         if l > max_length:
             logger.info(f"{cif_id} failed : supercell have more than max_length")
@@ -359,15 +395,15 @@
     # 3. calculate energy grid
     eg_success = get_energy_grid(atoms_eg, cif_id, root_dataset_total, eg_logger)
 
     if eg_success:
         logger.info(f"{cif_id} succeed : supercell length {atoms.cell.cellpar()[:3]}")
 
         # save cif files
-        save_cif_path = root_dataset_total / f'{cif_id}.cif'
+        save_cif_path = root_dataset_total / f"{cif_id}.cif"
         atoms.write(filename=save_cif_path)
 
         # save graphdata file
         data = [cif_id, atom_num, nbr_idx, nbr_dist, uni_idx, uni_count]
         with open(str(p_graphdata), "wb") as f:
             pickle.dump(data, f)
         return True
@@ -392,44 +428,48 @@
         - get_primitive (bool) : If True, use primitive cell in graph embedding
         - max_num_atoms (int): max number atoms in primitive cell
         - max_length (float) : maximum length of supercell
         - min_length (float) : minimum length of supercell
         - max_num_nbr (int) : maximum number of neighbors when calculating graph
     """
     if not os.path.exists(GRIDAY_PATH):
-        raise ImportError('GRIDAY must be installed. \n'
-                          'Run the following code in bash, \n\n'
-                          '$ moftransformer install-griday\n\n'
-                          'or run the following code on Python\n\n'
-                          '>>> from moftransformer.utils import install_griday\n'
-                          '>>> install_griday()')
+        raise ImportError(
+            "GRIDAY must be installed. \n"
+            "Run the following code in bash, \n\n"
+            "$ moftransformer install-griday\n\n"
+            "or run the following code on Python\n\n"
+            ">>> from moftransformer.utils import install_griday\n"
+            ">>> install_griday()"
+        )
 
     # set logger
     logger = get_logger(filename="prepare_data.log")
     eg_logger = get_logger(filename="prepare_energy_grid.log")
 
     # directory to "Path"
     root_cifs = Path(root_cifs)
     root_dataset = Path(root_dataset)
 
     if not root_cifs.exists():
-        raise ValueError(f'{root_cifs} does not exists.')
+        raise ValueError(f"{root_cifs} does not exists.")
 
     # make prepare_data in 'total' directory
-    root_dataset_total = Path(root_dataset) / 'total'
+    root_dataset_total = Path(root_dataset) / "total"
     root_dataset_total.mkdir(exist_ok=True, parents=True)
 
     # make *.grid, *.griddata16, and *.graphdata file
-    for cif in tqdm(root_cifs.glob('*.cif'), total=sum(1 for _ in root_cifs.glob('*.cif'))):
+    for cif in tqdm(
+        root_cifs.glob("*.cif"), total=sum(1 for _ in root_cifs.glob("*.cif"))
+    ):
         make_prepared_data(cif, root_dataset_total, logger, eg_logger, **kwargs)
 
     # automatically split data
     _split_dataset(root_dataset, **kwargs)
 
     # split json file
     if isinstance(downstream, str):
         _split_json(root_cifs, root_dataset, downstream)
     elif isinstance(downstream, Iterable):
         for single_downstream in downstream:
             _split_json(root_cifs, root_dataset, single_downstream)
     else:
-        raise TypeError(f'task must be str or Iterable, not {type(downstream)}')
+        raise TypeError(f"task must be str or Iterable, not {type(downstream)}")
```

### Comparing `moftransformer-1.1.3/moftransformer/visualize/drawer.py` & `moftransformer-2.0.0/moftransformer/visualize/drawer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,39 @@
+# MOFTransformer version 2.0.0
 import numpy as np
 from itertools import combinations
 from matplotlib import pyplot as plt
 from matplotlib.colors import Normalize
 import matplotlib.ticker as mticker
 from ase.data import covalent_radii
 from moftransformer.assets.colors import cpk_colors
 from moftransformer.visualize.utils import plot_cube
 
 
 def draw_colorbar(fig, ax, cmap, minatt, maxatt, **cbar_kwargs):
-    norm = Normalize(0., 1.)
+    norm = Normalize(0.0, 1.0)
     smap = plt.cm.ScalarMappable(cmap=cmap, norm=norm)
-    cbar = fig.colorbar(smap, ax=ax, fraction=cbar_kwargs['fraction'], shrink=cbar_kwargs['shrink'])
-    cbar.ax.tick_params(labelsize=cbar_kwargs['fontsize'])
-    ticks_loc = np.linspace(0, 1, cbar_kwargs['num_ticks'])
-    ticks_label = np.round(np.linspace(minatt, maxatt, cbar_kwargs['num_ticks']),
-                           decimals=cbar_kwargs['decimals'])
+    cbar = fig.colorbar(
+        smap, ax=ax, fraction=cbar_kwargs["fraction"], shrink=cbar_kwargs["shrink"]
+    )
+    cbar.ax.tick_params(labelsize=cbar_kwargs["fontsize"])
+    ticks_loc = np.linspace(0, 1, cbar_kwargs["num_ticks"])
+    ticks_label = np.round(
+        np.linspace(minatt, maxatt, cbar_kwargs["num_ticks"]),
+        decimals=cbar_kwargs["decimals"],
+    )
     cbar.ax.yaxis.set_major_locator(mticker.FixedLocator(ticks_loc))
     cbar.ax.set_yticklabels(ticks_label)
 
-    cbar.ax.set_ylabel('Attention score', rotation=270, labelpad=cbar_kwargs['labelpad'],
-                       fontdict={"size": cbar_kwargs['labelsize']})
+    cbar.ax.set_ylabel(
+        "Attention score",
+        rotation=270,
+        labelpad=cbar_kwargs["labelpad"],
+        fontdict={"size": cbar_kwargs["labelsize"]},
+    )
 
 
 def draw_line(ax, pos1, pos2, **kwargs):
     """
     Draw line from position 1 to position 2
     :param ax: <matplotlib.axes> figure axis
     :param pos1: <np.array> starting point position
@@ -78,16 +87,22 @@
         edgecolor="black",
         linewidths=0.8,
         alpha=1.0,
     )
 
 
 def draw_heatmap_grid(ax, positions, colors, lattice, num_patches, alpha=0.5, **kwargs):
-    cubes = plot_cube(positions, colors, lattice=lattice,
-                      num_patches=num_patches, edgecolor=None, alpha=alpha)
+    cubes = plot_cube(
+        positions,
+        colors,
+        lattice=lattice,
+        num_patches=num_patches,
+        edgecolor=None,
+        alpha=alpha,
+    )
     ax.add_collection3d(cubes, **kwargs)
 
 
 def draw_heatmap_graph(ax, atoms, uni_idx, colors, atomic_scale, alpha):
     coords = atoms.get_positions()
     for i, idxes in enumerate(uni_idx):
         uni_coords = coords[idxes]
@@ -95,11 +110,11 @@
         # c = cmap(scaler(att, minatt, maxatt))
         ax.scatter(
             xs=uni_coords[:, 0],
             ys=uni_coords[:, 1],
             zs=uni_coords[:, 2],
             color=colors[i],
             s=atomic_scale,
-            marker='o',
+            marker="o",
             linewidth=0,
             alpha=alpha,
         )
```

### Comparing `moftransformer-1.1.3/moftransformer/visualize/setting.py` & `moftransformer-2.0.0/moftransformer/visualize/setting.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,61 @@
+# MOFTransformer version 2.0.0
 import numpy as np
 import seaborn as sns
 from matplotlib import pyplot as plt
 from matplotlib.colors import ListedColormap
 
 DEFAULT_FIGSIZE = (8, 8)
 DEFAULT_VIEW_INIT = (0, 0)
 
 
 def get_default_cbar_kwargs(figsize):
-    return {'num_ticks': 6, 'decimals': 4, 'labelpad': figsize[0] * 2,
-            'labelsize': figsize[0] * 1.5, 'fontsize': figsize[0],
-            'fraction': 0.1, 'shrink': 0.5}
+    return {
+        "num_ticks": 6,
+        "decimals": 4,
+        "labelpad": figsize[0] * 2,
+        "labelsize": figsize[0] * 1.5,
+        "fontsize": figsize[0],
+        "fraction": 0.1,
+        "shrink": 0.5,
+    }
 
 
 def get_fig_ax(**kwargs):
     """
     Default setting for matplotlib figure
     :param kwargs: kwargs for matplotlib figure
         figsize : (float, float) figure size
         view_init : (float, float) view init from matplotlib
         show_axis : <bool> If True, axis are visible. (default : False)
         show_colorbar : <bool> If True, colorbar are visible. (default : True)
     :return: <matplotlib.figure>, <matplotlib.axes>, <matplotlib.cmap>
     """
-    figsize = kwargs.get('figsize', DEFAULT_FIGSIZE)
-    view_init = kwargs.get('view_init', DEFAULT_VIEW_INIT)
-    show_axis = kwargs.get('axis', False)
+    figsize = kwargs.get("figsize", DEFAULT_FIGSIZE)
+    view_init = kwargs.get("view_init", DEFAULT_VIEW_INIT)
+    show_axis = kwargs.get("axis", False)
 
     # Set default setting
     fig = plt.figure(figsize=figsize)
-    ax = fig.add_subplot(projection='3d')
+    ax = fig.add_subplot(projection="3d")
     ax.view_init(*view_init)
     ax.set_proj_type("ortho")
     ax.grid(visible=False)
     if not show_axis:
         ax.set_axis_off()
 
     return fig, ax
 
 
 def set_fig_ax(ax, **kwargs):
     if not kwargs:
         return
-    if view_init := kwargs.get('view_init'):  # view_init
+    if view_init := kwargs.get("view_init"):  # view_init
         ax.view_init(*view_init)
-    if show_axis := kwargs.get('show_axis'):  # show axis
+    if show_axis := kwargs.get("show_axis"):  # show axis
         if show_axis:
             ax.set_axis_on()
         else:
             ax.set_axis_off()
 
 
 def get_cmap(cmap=None):
@@ -64,15 +71,15 @@
 
         cmap1 = np.linspace(start_color, middle_color, num=idx)
         cmap2 = np.linspace(middle_color, end_color, num=256 - idx)
         cmap = np.concatenate((cmap1, cmap2), axis=0)
         custom_cmap = ListedColormap(cmap)
         return custom_cmap
     else:
-        raise TypeError(f'cmap must be str, ListedColormap, or None, not {type(cmap)}')
+        raise TypeError(f"cmap must be str, ListedColormap, or None, not {type(cmap)}")
 
 
 def set_axes_equal(ax, scale_factor=1):
     """Make axes of 3D plot have equal scale so that spheres appear as spheres,
     cubes as cubes, etc...  This is one possible solution to Matplotlib's
     ax.set_aspect('equal') and ax.axis('equal') not working for 3D.
     code from 'https://stackoverflow.com/questions/13685386/matplotlib-equal-unit-length-with-equal-aspect-ratio-z-axis-is-not-equal-to'
```

### Comparing `moftransformer-1.1.3/moftransformer/visualize/utils.py` & `moftransformer-2.0.0/moftransformer/visualize/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# MOFTransformer version 2.0.0
 import copy
 import math
 import ase.io
 from ase.build import make_supercell
 from itertools import product
 from functools import lru_cache
 from pathlib import Path
@@ -15,31 +16,31 @@
 import pytorch_lightning as pl
 from moftransformer.modules.module import Module
 from moftransformer.datamodules.datamodule import Datamodule
 from moftransformer.config import config
 
 
 @lru_cache
-def get_model_and_datamodule(model_path, data_root, downstream=''):
+def get_model_and_datamodule(model_path, data_root, downstream=""):
     _config = config()
-    _config['visualize'] = True
+    _config["visualize"] = True
     _config["per_gpu_batchsize"] = 1
     _config["data_root"] = data_root
     _config["root_dataset"] = data_root
     _config["load_path"] = model_path
     _config["test_only"] = True
     _config["use_transformer"] = True
-    _config["log_dir"] = 'result_visualization'
+    _config["log_dir"] = "result_visualization"
     _config["downstream"] = downstream
 
-    pl.seed_everything(_config['seed'])
+    pl.seed_everything(_config["seed"])
     model = Module(_config)
     model.setup("test")
     model.eval()
-    model.to('cpu')
+    model.to("cpu")
 
     dm = Datamodule(_config)
     dm.setup("test")
     data_iter = dm.test_dataloader()
 
     return model, data_iter
 
@@ -57,77 +58,82 @@
 def get_batch_from_cif_id(data_iter, cif_id):
     cif_id = Path(cif_id).stem
     iter_ = iter(data_iter)
     while True:
         try:
             batch = next(iter_)
         except StopIteration:
-            raise ValueError(f'There are no {cif_id} in dataset')
+            raise ValueError(f"There are no {cif_id} in dataset")
         else:
             batch_id = batch["cif_id"][0]
             if batch_id == cif_id:
                 return batch
 
 
 @lru_cache
 def get_primitive_structure(path_cif, tolerance=2.0):
-    st, = CifParser(path_cif, occupancy_tolerance=tolerance).get_structures(primitive=True)
+    (st,) = CifParser(path_cif, occupancy_tolerance=tolerance).get_structures(
+        primitive=True
+    )
     return st
 
 
 @lru_cache
-def get_structure(path_cif, make_supercell=False, dtype='ase', *,
-                  max_length=60, min_length=30):
+def get_structure(
+    path_cif, make_supercell=False, dtype="ase", *, max_length=60, min_length=30
+):
     """
     get primitive structure from path_cif
     :param path_cif: <str> path for cif file
     :param make_supercell: <bool> if True,
     :param dtype: <str> -> ['ase', 'pymatgen'] return type for structure.
     :param max_length: <int/float> max p_lattice length of structure file (Å)
     :param min_length: <int/float> min p_lattice length of structure file (Å)
     :return: <pymatgen.Structure> structure file from path cif
     """
     try:
         CifParser(path_cif).get_structures()
-    except ValueError as e:   
-        raise ValueError(f'{path_cif} failed : (read pymatgen) {e}')
+    except ValueError as e:
+        raise ValueError(f"{path_cif} failed : (read pymatgen) {e}")
 
     atoms = ase.io.read(path_cif)
 
     if make_supercell:
         atoms = get_supercell_structure(atoms, max_length, min_length)
     else:
         atoms = get_supercell_structure(atoms, max_length, 8)
 
-    if dtype == 'pymatgen':
+    if dtype == "pymatgen":
         return AseAtomsAdaptor().get_structure(atoms)
-    elif dtype == 'ase':
+    elif dtype == "ase":
         return atoms
     else:
-        raise TypeError(f'type must be ase or pymatgen, not {dtype}')
+        raise TypeError(f"type must be ase or pymatgen, not {dtype}")
 
 
 def get_supercell_structure(atoms, max_length=60, min_length=30):
     """
     get supercell atoms from <ase.Atoms>
     :param atoms: <ase.Atoms> object
     :param max_length: <int/float> max p_lattice length of structure file (Å)
     :param min_length: <int/float> min p_lattice length of structure file (Å)
     :return: <ase.Atoms or pymatgen.Structure> structure type.
     """
     scale_abc = []
     for l in atoms.cell.cellpar()[:3]:
         if l > max_length:
-            raise ValueError(f"primitive p_lattice is larger than max_length {max_length}")
+            raise ValueError(
+                f"primitive p_lattice is larger than max_length {max_length}"
+            )
         elif l < min_length:
             scale_abc.append(math.ceil(min_length / l))
         else:
             scale_abc.append(1)
 
-    m = np.zeros([3,3])
+    m = np.zeros([3, 3])
     np.fill_diagonal(m, scale_abc)
     atoms = make_supercell(atoms, m)
     return atoms
 
 
 def cuboid_data(position, color=None, num_patches=(6, 6, 6), lattice=None):
     """
@@ -137,27 +143,27 @@
     :param num_patches: number of patches in each axis (default : (6, 6, 6))
     :param lattice: <np.ndarray> p_lattice vector for unit p_lattice
     :return: <tuple> (list of plain vector, list of color vector)
     """
     if isinstance(num_patches, (tuple, list)):
         num_patches = np.array(num_patches)
     elif not isinstance(num_patches, np.ndarray):
-        raise TypeError(f'num_patches must be tuple or list, not {type(num_patches)}')
+        raise TypeError(f"num_patches must be tuple or list, not {type(num_patches)}")
 
     bound = np.array([[0, 1] for _ in range(3)]) + np.array(position)[:, np.newaxis]
     vertex = np.array(list(product(*bound)))
     plane_ls = []
     for i, (dn, up) in enumerate(bound):
         plane1 = np.matmul(vertex[vertex[:, i] == dn], lattice / num_patches)
         plane2 = np.matmul(vertex[vertex[:, i] == up], lattice / num_patches)
 
         plane_ls.append(plane1)
         plane_ls.append(plane2)
 
-    plane_ls = np.array(plane_ls).astype('float')
+    plane_ls = np.array(plane_ls).astype("float")
     plane_ls[:, [0, 1], :] = plane_ls[:, [1, 0], :]
 
     color_ls = np.repeat(color[np.newaxis, :], 6, axis=0)
 
     return plane_ls, color_ls
 
 
@@ -168,43 +174,50 @@
     :param colors: <list -> list> list of color codes [r, g, b, w]
     :param lattice: <np.ndarray> p_lattice vector for unit p_lattice
     :param num_patches: number of patches in each axis (default : (6, 6, 6))
     :param kwargs: kwargs for <matplotlib.Poly3DCollection>
     :return: <matplotlib.Poly3DCollection> cuboid matplotlib object
     """
 
-    data = [cuboid_data(pos, color, num_patches=num_patches, lattice=lattice)
-            for pos, color in zip(positions, colors)]
+    data = [
+        cuboid_data(pos, color, num_patches=num_patches, lattice=lattice)
+        for pos, color in zip(positions, colors)
+    ]
     plain_ls, color_ls = zip(*data)
 
-    return Poly3DCollection(np.concatenate(plain_ls),
-                            facecolors=np.concatenate(color_ls), **kwargs)
+    return Poly3DCollection(
+        np.concatenate(plain_ls), facecolors=np.concatenate(color_ls), **kwargs
+    )
 
 
 def get_heatmap(out, batch_idx, graph_len=300, skip_cls=True):
     """
     attention rollout  in "Quantifying Attention Flow in Transformers" paper.
     :param out: output of model.infer(batch)
     :param batch_idx: batch index
     :param graph_len: the length of grid embedding
     :param skip_cls: <bool> If True, class token is ignored.
     :return: <np.ndarray> heatmap graph, heatmap grid
     """
-    attn_weights = torch.stack(out["attn_weights"])  # [num_layers, B, num_heads, max_len, max_len]
+    attn_weights = torch.stack(
+        out["attn_weights"]
+    )  # [num_layers, B, num_heads, max_len, max_len]
     att_mat = attn_weights[:, batch_idx]  # [num_layers, num_heads, max_len, max_len]
 
     # Average the attention weights across all heads.
     att_mat = torch.mean(att_mat, dim=1)  # [num_layers, max_len, max_len]
 
     # To account for residual connections, we add an identity matrix to the
     # attention matrix and re-normalize the weights.
     residual_att = torch.eye(att_mat.size(1))
     aug_att_mat = att_mat + residual_att
 
-    aug_att_mat = aug_att_mat / aug_att_mat.sum(dim=-1).unsqueeze(-1)  # [num_layers, max_len, max_len]
+    aug_att_mat = aug_att_mat / aug_att_mat.sum(dim=-1).unsqueeze(
+        -1
+    )  # [num_layers, max_len, max_len]
     aug_att_mat = aug_att_mat.detach().numpy()  # prevent from memory leakage
 
     # Recursively multiply the weight matrices
     joint_attentions = np.zeros(aug_att_mat.shape)  # [num_layers, max_len, max_len]
     joint_attentions[0] = aug_att_mat[0]
 
     for n in range(1, aug_att_mat.shape[0]):
@@ -217,16 +230,16 @@
         v_ = v[0][1:]  # skip cls token
         cost_graph = v_[:graph_len]  # / v_.max()
         cost_grid = v_[graph_len:]  # / v_.max()
         heatmap_graph = cost_graph
         heatmap_grid = cost_grid[1:-1].reshape(6, 6, 6)  # omit cls + volume tokens
     else:
         v_ = v[0]
-        cost_graph = v_[:graph_len + 1]  # / v_.max()
-        cost_grid = v_[graph_len + 1:]  # / v_.max()
+        cost_graph = v_[: graph_len + 1]  # / v_.max()
+        cost_grid = v_[graph_len + 1 :]  # / v_.max()
         heatmap_graph = cost_graph[1:]  # omit cls token
         heatmap_grid = cost_grid[1:-1].reshape(6, 6, 6)  # omit cls + volume tokens
 
     return heatmap_graph, heatmap_grid
 
 
 def scaler(value, min_att, max_att):
@@ -239,14 +252,10 @@
 
     elif isinstance(value, np.ndarray):
         value = copy.deepcopy(value)
         value[value > max_att] = max_att
         value[value < min_att] = min_att
         return (value - min_att) / (max_att - min_att)
     elif isinstance(value, Iterable):
-        return scaler(np.array(list(value), dtype='float'), min_att, max_att)
+        return scaler(np.array(list(value), dtype="float"), min_att, max_att)
     else:
-        raise TypeError(f'value must be float, list, or np.array, not {type(value)}')
-
-
-
-
+        raise TypeError(f"value must be float, list, or np.array, not {type(value)}")
```

### Comparing `moftransformer-1.1.3/moftransformer/visualize/visualizer.py` & `moftransformer-2.0.0/moftransformer/visualize/visualizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,42 @@
+# MOFTransformer version 2.0.0
 import os
 import numpy as np
 from pathlib import Path
 from collections.abc import Iterable, Sequence
 from itertools import product
 from functools import wraps, partial
 from matplotlib import pyplot as plt
 from matplotlib.colors import ListedColormap
 from matplotlib import animation
 
-from moftransformer.visualize.utils import get_structure, get_heatmap, scaler, get_model_and_datamodule, \
-    get_batch_from_index, get_batch_from_cif_id
-from moftransformer.visualize.setting import get_fig_ax, set_fig_ax, set_axes_equal, DEFAULT_FIGSIZE, \
-    DEFAULT_VIEW_INIT, get_default_cbar_kwargs, get_cmap
-from moftransformer.visualize.drawer import draw_cell, draw_atoms, draw_heatmap_grid, draw_colorbar, draw_heatmap_graph
+from moftransformer.visualize.utils import (
+    get_structure,
+    get_heatmap,
+    scaler,
+    get_model_and_datamodule,
+    get_batch_from_index,
+    get_batch_from_cif_id,
+)
+from moftransformer.visualize.setting import (
+    get_fig_ax,
+    set_fig_ax,
+    set_axes_equal,
+    DEFAULT_FIGSIZE,
+    DEFAULT_VIEW_INIT,
+    get_default_cbar_kwargs,
+    get_cmap,
+)
+from moftransformer.visualize.drawer import (
+    draw_cell,
+    draw_atoms,
+    draw_heatmap_grid,
+    draw_colorbar,
+    draw_heatmap_graph,
+)
 
 
 class PatchVisualizer(object):
     def __init__(self, path_cif, heatmap_graph, heatmap_grid, uni_idx, **kwargs):
         """
         Attention Visualizer from "MOFTransformer model"
         :param path_cif: <str> path for original cif file.
@@ -37,22 +57,29 @@
         self.heatmap_graph = heatmap_graph
         self.heatmap_grid = heatmap_grid
         self.uni_idx = uni_idx
         self.kwargs = kwargs
         self.cbar_kwargs = get_default_cbar_kwargs(self.figsize)
 
         # get primitive structure from cif
-        p_atoms = get_structure(self.path_cif, make_supercell=False, dtype='ase')
+        p_atoms = get_structure(self.path_cif, make_supercell=False, dtype="ase")
         self.p_atoms = p_atoms
         self.p_lattice = p_atoms.cell.array
 
         # get supercell atoms from cif
-        max_length, min_length = kwargs.get('max_length', 60), kwargs.get('min_length', 30)
-        super_atoms = get_structure(self.path_cif, make_supercell=True, dtype='ase',
-                                    max_length=max_length, min_length=min_length)
+        max_length, min_length = kwargs.get("max_length", 60), kwargs.get(
+            "min_length", 30
+        )
+        super_atoms = get_structure(
+            self.path_cif,
+            make_supercell=True,
+            dtype="ase",
+            max_length=max_length,
+            min_length=min_length,
+        )
         self.s_atoms = super_atoms
         self.s_lattice = super_atoms.cell.array
 
     @classmethod
     def from_batch(cls, batch, batch_idx, model, cif_root, **kwargs):
         """
         Attention visualizer from "MOFTransformer" model and "dataloader batch"
@@ -72,18 +99,22 @@
         :return: <PatchVisualizer> patch visualizer object
         """
         output = model.infer(batch)
         heatmap_graph, heatmap_grid = get_heatmap(output, batch_idx)
         uni_idx = batch["uni_idx"][batch_idx]
         cif_id = batch["cif_id"][batch_idx]
         path_cif = os.path.join(cif_root, cif_id + ".cif")
-        return cls(path_cif, heatmap_graph, heatmap_grid, uni_idx, cif_id=cif_id, **kwargs)
+        return cls(
+            path_cif, heatmap_graph, heatmap_grid, uni_idx, cif_id=cif_id, **kwargs
+        )
 
     @classmethod
-    def from_index(cls, index, model_path, data_root, downstream="", cif_root=None, **kwargs):
+    def from_index(
+        cls, index, model_path, data_root, downstream="", cif_root=None, **kwargs
+    ):
         """
         Create PatchVisualizer from index. The index corresponds 1:1 to the MOF in the json file in dataset folder.
         The index matches the cif order of json.
         :param index: (int) index of dataset.
         :param model_path: (str) path of model from fine-tuned MOFTransformer with format '.ckpt'
         :param data_root: (str) path of dataset directory obtained from 'prepared_data.py. (see Dataset Preparation)
                 MOFs to be visualized must exist in {dataset_folder}/test.json or {dataset_folder}/test_{downstream}.json,
@@ -101,20 +132,22 @@
             max_length : <float> max p_lattice length of structure file (Å)
             min_length: <float> min p_lattice length of structure file (Å)
         :return: PatchVisualizer class for index
         """
         model, data_iter = get_model_and_datamodule(model_path, data_root, downstream)
         batch = get_batch_from_index(data_iter, index)
         if cif_root is None:
-            cif_root = os.path.join(data_root, 'test')
+            cif_root = os.path.join(data_root, "test")
 
         return cls.from_batch(batch, 0, model, cif_root, **kwargs)
 
     @classmethod
-    def from_cifname(cls, cifname, model_path, data_root, downstream="", cif_root=None, **kwargs):
+    def from_cifname(
+        cls, cifname, model_path, data_root, downstream="", cif_root=None, **kwargs
+    ):
         """
         Create PatchVisualizer from cif name. cif must be in test.json or test_{downstream}.json.
 
         :param cifname : (str) name or path of cif. Data matching the corresponding cif name is retrieved from the dataset.
         :param model_path: (str) path of model from fine-tuned MOFTransformer with format '.ckpt'
         :param data_root: (str) path of dataset directory obtained from 'prepared_data.py. (see Dataset Preparation)
                 MOFs to be visualized must exist in {dataset_folder}/test.json or {dataset_folder}/test_{downstream}.json,
@@ -132,138 +165,154 @@
             max_length : <float> max p_lattice length of structure file (Å)
             min_length: <float> min p_lattice length of structure file (Å)
         :return: PatchVisualizer class for index
         """
         model, data_iter = get_model_and_datamodule(model_path, data_root, downstream)
         batch = get_batch_from_cif_id(data_iter, cifname)
         if cif_root is None:
-            cif_root = os.path.join(data_root, 'test')
+            cif_root = os.path.join(data_root, "test")
         return cls.from_batch(batch, 0, model, cif_root, **kwargs)
 
     def __repr__(self):
         return f"class <PatchVisualizer> from {self.cif_id}"
 
     @property
     def cif_id(self):
-        if cif_id := self.kwargs.get('cifname'):
+        if cif_id := self.kwargs.get("cifname"):
             return cif_id
         else:
             return Path(self.path_cif).stem
 
     @property
     def cmap(self):
-        return self.kwargs.get('cmap', None)
+        return self.kwargs.get("cmap", None)
 
     @cmap.setter
     def cmap(self, cmap):
         if isinstance(cmap, (str, ListedColormap)) or cmap is None:
-            self.kwargs['cmap'] = cmap
+            self.kwargs["cmap"] = cmap
         else:
-            raise TypeError(f'cmap must be str, ListedColormap, or None, not {type(cmap)}')
+            raise TypeError(
+                f"cmap must be str, ListedColormap, or None, not {type(cmap)}"
+            )
 
     @property
     def num_patches(self):
-        return self.kwargs.get('num_patches', (6, 6, 6))
+        return self.kwargs.get("num_patches", (6, 6, 6))
 
     @property
     def figsize(self):
-        return self.kwargs.get('figsize', DEFAULT_FIGSIZE)
+        return self.kwargs.get("figsize", DEFAULT_FIGSIZE)
 
     @figsize.setter
     def figsize(self, figsize):
         if not isinstance(figsize, Sequence):
             raise TypeError(f"figsize must be tuple or list, not {type(figsize)}")
         elif len(figsize) != 2:
             raise ValueError(f"figsize must be (float, float) not {figsize}")
-        self.kwargs['figsize'] = figsize
+        self.kwargs["figsize"] = figsize
         self._sync_cbar_kwargs()
 
     @property
     def view_init(self):
-        return self.kwargs.get('view_init', DEFAULT_VIEW_INIT)
+        return self.kwargs.get("view_init", DEFAULT_VIEW_INIT)
 
     @view_init.setter
     def view_init(self, view_init):
         if not isinstance(view_init, Sequence):
-            raise TypeError(f'view_init must be tuple or list, not {type(view_init)}')
+            raise TypeError(f"view_init must be tuple or list, not {type(view_init)}")
         elif len(view_init) != 2:
             raise ValueError(f"view_init must be (float, float) not {view_init}")
-        self.kwargs['view_init'] = view_init
+        self.kwargs["view_init"] = view_init
 
     @property
     def show_axis(self):
-        return self.kwargs.get('show_colorbar', False)
+        return self.kwargs.get("show_colorbar", False)
 
     @show_axis.setter
     def show_axis(self, show_axis):
         if not isinstance(show_axis, bool):
-            raise TypeError(f'show_axis must be bool, not {type(show_axis)}')
-        self.kwargs['show_axis'] = show_axis
+            raise TypeError(f"show_axis must be bool, not {type(show_axis)}")
+        self.kwargs["show_axis"] = show_axis
 
     @property
     def show_colorbar(self):
-        return self.kwargs.get('show_colorbar', True)
+        return self.kwargs.get("show_colorbar", True)
 
     @show_colorbar.setter
     def show_colorbar(self, show_colorbar):
         if not isinstance(show_colorbar, bool):
-            raise TypeError(f'show_colorbar must be bool, not {type(show_colorbar)}')
-        self.kwargs['show_colorbar'] = show_colorbar
+            raise TypeError(f"show_colorbar must be bool, not {type(show_colorbar)}")
+        self.kwargs["show_colorbar"] = show_colorbar
 
     @property
     def atomic_scale(self):
         return self.figsize[0] * self.figsize[1]
 
     def set_default(self):
         self.kwargs = {}
         self._sync_cbar_kwargs()
 
     def _sync_cbar_kwargs(self):
         figsize = self.figsize
-        self.cbar_kwargs['labelpad'] = figsize[0] * 2
-        self.cbar_kwargs['labelsize'] = figsize[0] * 1.5
-        self.cbar_kwargs['fontsize'] = figsize[0]
+        self.cbar_kwargs["labelpad"] = figsize[0] * 2
+        self.cbar_kwargs["labelsize"] = figsize[0] * 1.5
+        self.cbar_kwargs["fontsize"] = figsize[0]
 
     def _get_indice_inside_patch(self, patch_position, ep=0.0):
         def is_inside_patch(r_pos, pos_patch, num_patch):
             lower_bound = (pos_patch - ep) / num_patch < r_pos
             upper_bound = r_pos < (pos_patch + 1 + ep) / num_patch
             return np.logical_and(lower_bound, upper_bound)
 
         relative_position = self.s_atoms.get_scaled_positions()
-        position_bools = [is_inside_patch(r_pos, pos_patch, num_patch)
-                          for r_pos, pos_patch, num_patch in
-                          zip(relative_position.T, patch_position, self.num_patches)]  # x, y, z
+        position_bools = [
+            is_inside_patch(r_pos, pos_patch, num_patch)
+            for r_pos, pos_patch, num_patch in zip(
+                relative_position.T, patch_position, self.num_patches
+            )
+        ]  # x, y, z
 
         position_bool = np.logical_and.reduce(position_bools)  # total
-        indice, = np.where(position_bool)
+        (indice,) = np.where(position_bool)
         return indice
 
     def _grid_attention_rank(self, rank):
         heatmap_grid = self.heatmap_grid
         sort = np.flip(
-            np.unravel_index(np.argsort(heatmap_grid, axis=None), heatmap_grid.shape), axis=-1
+            np.unravel_index(np.argsort(heatmap_grid, axis=None), heatmap_grid.shape),
+            axis=-1,
         )
         if isinstance(rank, int):
             return np.array(sort)[:, rank][np.newaxis, :]
         elif isinstance(rank, Iterable):
             return np.array(sort)[:, tuple(rank)].T
         else:
-            raise TypeError(f'rank must be int or iterable, not {type(rank)}')
+            raise TypeError(f"rank must be int or iterable, not {type(rank)}")
 
     def set_colorbar_options(self, default=False, **cbar_kwargs):
         if default:
             self.cbar_kwargs = get_default_cbar_kwargs(self.figsize)
         else:
             for key, value in cbar_kwargs.items():
                 if key in self.cbar_kwargs:
                     self.cbar_kwargs[key] = value
 
-    def draw_graph(self, minatt=0.000, maxatt=0.010, *, alpha=0.7, atomic_scale_factor=3,
-                   grid_scale_factor=1, att_scale_factor=3, return_fig=False, **kwargs):
+    def draw_graph(
+        self,
+        minatt=0.000,
+        maxatt=0.010,
+        *,
+        alpha=0.7,
+        atomic_scale_factor=3,
+        grid_scale_factor=1,
+        att_scale_factor=3,
+        return_fig=False,
+        **kwargs,
+    ):
         """
         Draw graph attention score figure in primitive unit cell
         :param minatt: (float) Minimum value of attention score (default : 0.000). A value smaller than minatt is treated as minatt.
         :param maxatt: (float) Maximum value of attention score (default : 0.010). A value larger than maxatt is treated as maxatt.
         :param alpha: (float) The alpha blending value, between 0 (transparent) and 1 (opaque).
         :param atomic_scale_factor: (float) The factors that determines atom size. (default = 1)
         :param grid_scale_factor: (float) The factors that determines grid size (default = 3)
@@ -276,35 +325,53 @@
             cmap : (str or matplotlib.colors.ListedColormap) color map used in figure. (default : None)
         """
         heatmap_graph = self.heatmap_graph
         lattice = self.p_lattice
         atoms = self.p_atoms
 
         fig, ax = get_fig_ax(**self.kwargs)
-        cmap = get_cmap(kwargs.get('cmap', self.cmap))
+        cmap = get_cmap(kwargs.get("cmap", self.cmap))
         set_fig_ax(ax, **kwargs)
 
-        draw_cell(ax, lattice, color='black')
-        draw_atoms(ax, atoms, self.atomic_scale * atomic_scale_factor * grid_scale_factor)
+        draw_cell(ax, lattice, color="black")
+        draw_atoms(
+            ax, atoms, self.atomic_scale * atomic_scale_factor * grid_scale_factor
+        )
 
         colors = cmap(scaler(heatmap_graph, minatt, maxatt))
-        atomic_scale = self.atomic_scale * att_scale_factor * grid_scale_factor * atomic_scale_factor
+        atomic_scale = (
+            self.atomic_scale
+            * att_scale_factor
+            * grid_scale_factor
+            * atomic_scale_factor
+        )
         draw_heatmap_graph(ax, atoms, self.uni_idx, colors, atomic_scale, alpha)
 
-        if kwargs.get('show_colorbar', self.show_colorbar):
+        if kwargs.get("show_colorbar", self.show_colorbar):
             draw_colorbar(fig, ax, cmap, minatt, maxatt, **self.cbar_kwargs)
 
         set_axes_equal(ax, scale_factor=grid_scale_factor)
         if return_fig:
             return fig, ax
         else:
             plt.show()
 
-    def draw_grid(self, minatt=0.000, maxatt=0.01, *, patch_list=None, remove_under_minatt=False,
-                  alpha=0.8, atomic_scale_factor=1, grid_scale_factor=1, return_fig=False, **kwargs):
+    def draw_grid(
+        self,
+        minatt=0.000,
+        maxatt=0.01,
+        *,
+        patch_list=None,
+        remove_under_minatt=False,
+        alpha=0.8,
+        atomic_scale_factor=1,
+        grid_scale_factor=1,
+        return_fig=False,
+        **kwargs,
+    ):
         """
         Draw grid attention score figure in supercell
         :param minatt: (float) Minimum value of attention score (default : 0.000). A value smaller than minatt is treated as minatt.
         :param maxatt: (float) Maximum value of attention score (default : 0.010). A value larger than maxatt is treated as maxatt.
         :param patch_list: (list) list of patch position that plot in figure. Draw all patches if not specified.
         :param remove_under_minatt: (bool) If True, do not draw a patch with an attention value lower than minatt.
         :param alpha: (float) The alpha blending value, between 0 (transparent) and 1 (opaque).
@@ -317,24 +384,26 @@
             show_colorbar : <bool> If True, colorbar are visible. (default : False)
             cmap : (str or matplotlib.colors.ListedColormap) color map used in figure. (default : None)
         """
         heatmap_grid = self.heatmap_grid
         lattice = self.s_lattice
         atoms = self.s_atoms
         fig, ax = get_fig_ax(**self.kwargs)
-        cmap = get_cmap(kwargs.get('cmap', self.cmap))
+        cmap = get_cmap(kwargs.get("cmap", self.cmap))
         set_fig_ax(ax, **kwargs)
 
         # patch_list
         if patch_list is None:
             patch_list = product(*[range(n) for n in self.num_patches])
         elif isinstance(patch_list, Iterable):
             pass
         else:
-            raise TypeError(f'patch_list must be iterable object, not {type(patch_list)}')
+            raise TypeError(
+                f"patch_list must be iterable object, not {type(patch_list)}"
+            )
 
         # get position and heatmap
         positions = []
         sc_heatmap_grid = []
         for i, j, k in patch_list:
             att = heatmap_grid[i, j, k]
             if remove_under_minatt and att < minatt:
@@ -342,30 +411,49 @@
             positions.append((i, j, k))
             sc_heatmap_grid.append(scaler(att, minatt, maxatt))
 
         sc_heatmap_grid = np.array(sc_heatmap_grid)
         heatmap = cmap(sc_heatmap_grid.flatten())
 
         # draw
-        draw_heatmap_grid(ax, positions, heatmap, lattice,
-                          num_patches=self.num_patches, alpha=alpha, )
-        draw_cell(ax, lattice, color='black')
-        draw_atoms(ax, atoms, self.atomic_scale * atomic_scale_factor * grid_scale_factor)
+        draw_heatmap_grid(
+            ax,
+            positions,
+            heatmap,
+            lattice,
+            num_patches=self.num_patches,
+            alpha=alpha,
+        )
+        draw_cell(ax, lattice, color="black")
+        draw_atoms(
+            ax, atoms, self.atomic_scale * atomic_scale_factor * grid_scale_factor
+        )
 
-        if kwargs.get('show_colorbar', self.show_colorbar):
+        if kwargs.get("show_colorbar", self.show_colorbar):
             draw_colorbar(fig, ax, cmap, minatt, maxatt, **self.cbar_kwargs)
 
         set_axes_equal(ax, scale_factor=grid_scale_factor)
         if return_fig:
             return fig, ax
         else:
             plt.show()
 
-    def draw_grid_with_attention_rank(self, rank, minatt=0.000, maxatt=0.010, *, remove_under_minatt=False,
-                                      alpha=0.8, atomic_scale_factor=1, grid_scale_factor=1, return_fig=False, **kwargs):
+    def draw_grid_with_attention_rank(
+        self,
+        rank,
+        minatt=0.000,
+        maxatt=0.010,
+        *,
+        remove_under_minatt=False,
+        alpha=0.8,
+        atomic_scale_factor=1,
+        grid_scale_factor=1,
+        return_fig=False,
+        **kwargs,
+    ):
         """
         Draw grid attention score figure in supercell
         :param rank:  (int or iterable) The rank (int) or iterable of ranks (list, np.array, tuple, range, etc) of the patch you want to draw.
                         Rank means that the attention score is listed in the order of high.
         :param minatt: (float) Minimum value of attention score (default : 0.000). A value smaller than minatt is treated as minatt.
         :param maxatt: (float) Maximum value of attention score (default : 0.010). A value larger than maxatt is treated as maxatt.
         :param remove_under_minatt: (bool) If True, do not draw a patch with an attention value lower than minatt.
@@ -376,20 +464,40 @@
         :param kwargs:
             view_init : (float, float) view init from matplotlib
             show_axis : <bool> If True, axis are visible. (default : False)
             show_colorbar : <bool> If True, colorbar are visible. (default : False)
             cmap : (str or matplotlib.colors.ListedColormap) color map used in figure. (default : None)
         """
         rank = self._grid_attention_rank(rank)
-        return self.draw_grid(minatt, maxatt, patch_list=rank, remove_under_minatt=remove_under_minatt,
-                       alpha=alpha, atomic_scale_factor=atomic_scale_factor,
-                       grid_scale_factor=grid_scale_factor, return_fig=return_fig, **kwargs)
+        return self.draw_grid(
+            minatt,
+            maxatt,
+            patch_list=rank,
+            remove_under_minatt=remove_under_minatt,
+            alpha=alpha,
+            atomic_scale_factor=atomic_scale_factor,
+            grid_scale_factor=grid_scale_factor,
+            return_fig=return_fig,
+            **kwargs,
+        )
 
-    def draw_specific_patch(self, patch_position, ep=0.5, *, color=True, alpha=0.5, minatt=0.000, maxatt=0.010,
-                            atomic_scale_factor=5, grid_scale_factor=1, return_fig=False, **kwargs):
+    def draw_specific_patch(
+        self,
+        patch_position,
+        ep=0.5,
+        *,
+        color=True,
+        alpha=0.5,
+        minatt=0.000,
+        maxatt=0.010,
+        atomic_scale_factor=5,
+        grid_scale_factor=1,
+        return_fig=False,
+        **kwargs,
+    ):
         """
         Draw one specific patch with neighbor atoms.
         :param patch_position:  (list) patch position that plot in figure.
         :param ep: (float) Distance of patches to be visualized around target patches (default = 0.5)
         :param color: (bool) If True, paint patch's color that indicate attention grid
         :param minatt: (float) Minimum value of attention score (default : 0.000). A value smaller than minatt is treated as minatt.
         :param maxatt: (float) Maximum value of attention score (default : 0.010). A value larger than maxatt is treated as maxatt.
@@ -404,45 +512,67 @@
             cmap : (str or matplotlib.colors.ListedColormap) color map used in figure. (default : None)
         """
         lattice = self.s_lattice
         atoms = self.s_atoms
         indice = self._get_indice_inside_patch(patch_position, ep=ep)
         s_point = np.sum(lattice.T / 6 * patch_position, axis=1)
         fig, ax = get_fig_ax(**self.kwargs)
-        cmap = get_cmap(kwargs.get('cmap', self.cmap))
+        cmap = get_cmap(kwargs.get("cmap", self.cmap))
         set_fig_ax(ax, **kwargs)
 
         if ep > 0.5:
-            scale_factor = self.atomic_scale * atomic_scale_factor * grid_scale_factor / ep
+            scale_factor = (
+                self.atomic_scale * atomic_scale_factor * grid_scale_factor / ep
+            )
         else:
-            scale_factor = self.atomic_scale * atomic_scale_factor * grid_scale_factor * 2
+            scale_factor = (
+                self.atomic_scale * atomic_scale_factor * grid_scale_factor * 2
+            )
 
         draw_cell(ax, lattice / 6, s_point=s_point, color="black")
         draw_atoms(ax, atoms[indice], atomic_scale=scale_factor)
 
         if color:
             heatmap_grid = self.heatmap_grid
             patch_color = scaler(heatmap_grid[tuple(patch_position)], minatt, maxatt)
             patch_color = cmap(np.array([patch_color]))
             position = [patch_position]
-            draw_heatmap_grid(ax, position, patch_color, lattice=lattice,
-                              num_patches=self.num_patches, alpha=alpha)
+            draw_heatmap_grid(
+                ax,
+                position,
+                patch_color,
+                lattice=lattice,
+                num_patches=self.num_patches,
+                alpha=alpha,
+            )
 
-        if kwargs.get('show_colorbar', self.show_colorbar):
+        if kwargs.get("show_colorbar", self.show_colorbar):
             draw_colorbar(fig, ax, cmap, minatt, maxatt, **self.cbar_kwargs)
 
         set_axes_equal(ax, grid_scale_factor)
 
         if return_fig:
             return fig, ax
         else:
             plt.show()
 
-    def draw_specific_patch_with_attention_rank(self, rank, ep=0.5, *, color=True, alpha=0.5, minatt=0.000, maxatt=0.010,
-                                                atomic_scale_factor=5, grid_scale_factor=1, return_fig=False, **kwargs):
+    def draw_specific_patch_with_attention_rank(
+        self,
+        rank,
+        ep=0.5,
+        *,
+        color=True,
+        alpha=0.5,
+        minatt=0.000,
+        maxatt=0.010,
+        atomic_scale_factor=5,
+        grid_scale_factor=1,
+        return_fig=False,
+        **kwargs,
+    ):
         """
         Draw one specific patch with neighbor atoms.
         :param rank : (int or iterable) The rank (int) of the patch you want to draw.
                         Rank means that the attention score is listed in the order of high.
         :param ep: (float) Distance of patches to be visualized around target patches (default = 0.5)
         :param color: (bool) If True, paint patch's color that indicate attention grid
         :param minatt: (float) Minimum value of attention score (default : 0.000). A value smaller than minatt is treated as minatt.
@@ -454,33 +584,48 @@
         :param kwargs:
             view_init : (float, float) view init from matplotlib
             show_axis : <bool> If True, axis are visible. (default : False)
             show_colorbar : <bool> If True, colorbar are visible. (default : False)
             cmap : (str or matplotlib.colors.ListedColormap) color map used in figure. (default : None)
         """
         if not isinstance(rank, int):
-            raise TypeError(f'rank must be int, not {type(rank)}')
+            raise TypeError(f"rank must be int, not {type(rank)}")
 
         rank = self._grid_attention_rank(rank).squeeze()
-        return self.draw_specific_patch(rank, ep=ep, color=color, minatt=minatt, maxatt=maxatt,
-                                 atomic_scale_factor=atomic_scale_factor, grid_scale_factor=grid_scale_factor,
-                                 alpha=alpha, return_fig=return_fig, **kwargs)
+        return self.draw_specific_patch(
+            rank,
+            ep=ep,
+            color=color,
+            minatt=minatt,
+            maxatt=maxatt,
+            atomic_scale_factor=atomic_scale_factor,
+            grid_scale_factor=grid_scale_factor,
+            alpha=alpha,
+            return_fig=return_fig,
+            **kwargs,
+        )
 
     def animate(self, func, frame=360, interval=20, savefile=None, fps=30):
         def turn(i, ax, fig, **kwargs):
-            view_init = kwargs.get('view_init', self.view_init)
+            view_init = kwargs.get("view_init", self.view_init)
             ax.view_init(elev=view_init[0], azim=i)
             return fig
 
         @wraps(func)
         def wrapper(*args, **kwargs):
-            kwargs['return_fig'] = True
+            kwargs["return_fig"] = True
             fig, ax = func(*args, **kwargs)
-            anim = animation.FuncAnimation(fig, partial(turn, ax=ax, fig=fig, **kwargs), init_func=lambda:fig,
-                                           frames=frame, interval=interval, blit=True)
+            anim = animation.FuncAnimation(
+                fig,
+                partial(turn, ax=ax, fig=fig, **kwargs),
+                init_func=lambda: fig,
+                frames=frame,
+                interval=interval,
+                blit=True,
+            )
             if savefile:
                 anim.save(savefile, fps=fps, dpi=300)
 
             plt.show()
             return anim
 
         return wrapper
```

### Comparing `moftransformer-1.1.3/moftransformer.egg-info/PKG-INFO` & `moftransformer-2.0.0/moftransformer.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,151 +1,113 @@
 Metadata-Version: 2.1
 Name: moftransformer
-Version: 1.1.3
+Version: 2.0.0
 Summary: moftransformer
 Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer
 Author: Yeonghun Kang, Hyunsoo Park
 Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v1.1.3-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.0.0-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v1.1.3-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.0.0-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
- <a href="https://doi.org/10.1038/s42256-023-00628-2">
+ <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
  <a href="https://pypi.org/project/moftransformer/">
      <img alt="Lincense" src="https://img.shields.io/badge/License-MIT-lightgrey.svg?style=plastic">
  </a>
 </p>
 
-# [MOFTransformer](https://hspark1212.github.io/MOFTransformer/index.html)
+# [PMTransformer (MOFTransformer)](https://hspark1212.github.io/MOFTransformer/index.html)
 
- This package provides universal transfer learing for metal-organic frameworks(MOFs) to construct structure-property relationships. `MOFTransformer` obtains state-of-the-art performance to predict accross various properties that include gas adsorption, diffusion, electronic properties regardless of gas types. Beyond its universal transfer learning capabilityies, it provides feature importance analysis from its attentions scores to capture chemical intution.
+ This package provides a universal transfer learning model, `PMTransformer` (Porous Materials Transformer), which obtains the state-of-the-art performance in predicting various properties of porous materials. The PMTRansformer was pre-trainied with 1.9 million hypothetical porous materials including Metal-Organic Frameworks (MOFs), Covalent-Organic Frameworks (COFs), Porous Polymer Networks (PPNs), and zeolites. By fine-tuning the pre-trained `PMTransformer`, you can easily obtain machine learning models to accurately predict various properties of porous materials .
+ 
+ NOTE: From version 2.0.0, the default pre-training model has been changed from `MOFTransformer` to `PMTransformer`, which was pre-trained with a larger dataset, containing other porous materials as well as MOFs. The `PMTransformer` outperforms the `MOFTransformer` in predicting various properties of porous materials.
 
 ## [Install](https://hspark1212.github.io/MOFTransformer/installation.html)
 
-### OS and hardware requirements
-The package development version is tested on following systems:
-
-Linux : Ubuntu 20.04, 22.04
-
-For optimal performance, we recommend running with GPUs
-
 ### Depedencies
 ```
 python>=3.8
 ```
-Given that MOFTransformer is based on pytorch, please install pytorch (>= 1.10.0) according to your environments.
+Given that MOFTransformer is based on pytorch, please install pytorch (>= 1.12.0) according to your environments.
 
 ### Installation using PIP 
 ```
 $ pip install moftransformer
 ```
-which should install in about 50 seconds.
 
-### Download the pretrained model (ckpt file)
-- you can download the pretrained model with 1 M hMOFs in [figshare](https://figshare.com/articles/dataset/MOFTransformer/21155506)
+### Download the pretrained models (ckpt file)
+- you can download the pretrained models (`PMTransformer.ckpt` and `MOFTransformer.ckpt`) [figshare](https://figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2)
+
 or you can download with a command line:
 ```
 $ moftransformer download pretrain_model
 ```
-### (Optional) Download dataset for CoREMOF, QMOF
-- we've provide the dataset of MOFTransformer (i.e., atom-based graph embeddings and energy-grid embeddings) for CoREMOF, QMOF
+### (Optional) Download pre-embeddings for CoREMOF, QMOF
+- we've provide the pre-embeddings (i.e., atom-based graph embeddings and energy-grid embeddings), inputs of `PMTransformer`, for CoREMOF, QMOF database.
 ```
 $ moftransformer download coremof
 $ moftransformer download qmof
 ```
 
 ## [Getting Started](https://hspark1212.github.io/MOFTransformer/tutorial.html)
-
-1. At first, you can run `prepare_data` with 10 cifs in `moftransformer/examples/raw` directory.
-
-In order to run `prepare_data`, you need to install `GRIDAY` to calculate energy grid.
-You can download GRIDAY using command-line.
-
-```bash
-$ moftransformer install-griday
+1. At first, you download dataset of hMOFs (20,000 MOFs) as an example.
 ```
-
-Example for running `prepare-data`
-
-```python
-from moftransformer.examples import example_path
-from moftransformer.utils import prepare_data
-
-# Get example path
-root_cifs = example_path['root_cif']
-root_dataset = example_path['root_dataset']
-downstream = example_path['downstream']
-
-train_fraction = 0.7
-test_fraction = 0.2
-
-# Run prepare data
-prepare_data(root_cifs, root_dataset, downstream=downstream, 
-             train_fraciton=train_fraction, test_fraciton=test_fraction)
+$ moftransformer download hmof
 ```
-
 2. Fine-tune the pretrained MOFTransformer.
 ```python
 import moftransformer
 from moftransformer.examples import example_path
 
 # data root and downstream from example
-root_dataset = example_path['root_dataset']
+data_root = example_path['data_root']
 downstream = example_path['downstream']
 log_dir = './logs/'
+# load_path = "pmtransformer" (default)
 
-# kwargs (optional)
-max_epochs = 10
-batch_size = 8
-
-moftransformer.run(root_dataset, downstream, log_dir=log_dir, 
+moftransformer.run(data_root, downstream, log_dir=log_dir, 
                    max_epochs=max_epochs, batch_size=batch_size,)
 ```
-which will run in about 35 seconds.
-
-
 3. Visualize analysis of feature importance for the fine-tuned model.
-
-download finetuned-bandgap model before visualize.
-```bash
-moftransformer download finetuned_model -o ./examples
-```
-
 ```python
 %matplotlib widget
-from moftransformer.visualize import PatchVisualizer
-from moftransformer.examples import visualize_example_path
+from visualize import PatchVisualizer
 
 model_path = "examples/finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt'
-data_path = visualize_example_path
+data_path = 'examples/visualize/dataset/'
 cifname = 'MIBQAR01_FSR'
 
 vis = PatchVisualizer.from_cifname(cifname, model_path, data_path)
 vis.draw_graph() # or vis.draw_grid()
 ```
 
 ## [Architecture](https://hspark1212.github.io/MOFTransformer/introduction.html)
-`MOFTransformer`is a multi-modal Transformer pre-trained with 1 million hypothetical MOFs so that it efficiently capture both local and global feeatures of MOFs.
+It is a multi-modal pre-training Transformer encoder which is designed to capture both local and global features of porous materials. 
 
-- `MOFformer` takes two different representations as input
+The pre-traning tasks are as follows:
+(1) Topology Prediction
+(2) Void Fraction Prediction
+(3) Building Block Classification
+ 
+It takes two different representations as input
   - Atom-based Graph Embedding : CGCNN w/o pooling layer -> local features
   - Energy-grid Embedding : 1D flatten patches of 3D energy grid -> global features
   
 <p align="center">
   <img src="https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig2.jpg" width="700")
 </p>
 
@@ -163,32 +125,38 @@
 vis.draw_graph()
 ```
 <p align="center">
 <img src="https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/getting_started/assets/1.gif" width="400">
 </p>
 
 ```python
+vis = PatchVisualizer.from_cifname(cifname, model_path, data_path)
 vis.draw_grid()
 ```
 <p align="center">
 <img src="https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/getting_started/assets/3.gif" width="400">
 </p>
 
 ## Universal Transfer Learning
-| Property                                 | MOFTransformer | Original Paper | Number of Data | Remarks          | Reference |
-|------------------------------------------|----------------|----------------|----------------|------------------|-----------|
-|N<sub>2</sub> uptake                     | R2: 0.78       | R2: 0.71       | 5,286          | CoRE MOF         | 1         |
-|O<sub>2</sub> uptake                     | R2: 0.83       | R2: 0.74       | 5,286          | CoRE MOF         | 1         |
-|N<sub>2</sub> diffusivity                | R2: 0.77       | R2: 0.76       | 5,286          | CoRE MOF         | 1         |
-|O<sub>2</sub> diffusivity                | R2: 0.78       | R2: 0.74       | 5,286          | CoRE MOF         | 1         |
-|CO<sub>2</sub> Henry coefficient         | MAE : 0.30     | MAE : 0.42     | 8,183          | CoRE MOF         | 2         |
-|Solvent removal stability classification | ACC : 0.76     | ACC : 0.76     | 2,148          | Text-mining data | 3         |
-|Thermal stability regression             | R2 : 0.44      | R2 : 0.46      | 3,098          | Text-mining data | 3         |
-### Reference
-1. [Prediction of O2/N2 Selectivity in Metal−Organic Frameworks via High-Throughput Computational Screening and Machine Learning](https://pubs.acs.org/doi/abs/10.1021/acsami.1c18521)
-2. [Understanding the diversity of the metal-organic framework ecosystem](https://www.nature.com/articles/s41467-020-17755-8)
-3. [Using Machine Learning and Data Mining to Leverage Community Knowledge for the Engineering of Stable Metal–Organic Frameworks](https://pubs.acs.org/doi/10.1021/jacs.1c07217)
 
-## Citation
-If you want to cite the MOFTransformer and the pre-training and fine-tuning dataset, please refer to the publication:
+Comparison of mean absolute error (MAE) values for various baseline models, scratch, MOFTransformer, and PMTransformer on different properties of MOFs, COFs, PPNs, and zeolites. The bold values indicate the lowest MAE value for each property. The details of information can be found in [PMTransformer paper]()
+
+| Material | Property | Number of Dataset | Energy histogram | Descriptor-based ML | CGCNN | Scratch | MOFTransformer | PMTransformer |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| MOF | H<sub>2</sub> Uptake (100 bar) | 20,000 | 9.183 | 9.456 | 32.864 | 7.018 | 6.377 | **5.963** |
+| MOF | H<sub>2</sub> diffusivity (dilute) | 20,000 | 0.644 | 0.398 | 0.6600 | 0.391 | 0.367 | 0.**366** |
+| MOF | Band-gap | 20.373 | 0.913 | 0.590 | 0.290 | 0.271 | 0.224 | **0.216** |
+| MOF | N<sub>2</sub> uptake (1 bar) | 5,286 | 0.178 | 0.115 | 0.108 | 0.102 | 0.071 | **0.069** |
+| MOF | O<sub>2</sub> uptake (1 bar) | 5,286 | 0.162 | 0.076 | 0.083 | 0.071 | **0.051** | 0.053 |
+| MOF | N<sub>2</sub> diffusivity (1 bar) | 5,286 | 7.82e-5 | 5.22e-5 | 7.19e-5 | 5.82e-05 | **4.52e-05** | 4.53e-05 |
+| MOF | O<sub>2</sub> diffusivity (1 bar) | 5,286 | 7.14e-5 | 4.59e-5 | 6.56e-5 | 5.00e-05 | 4.04e-05 | **3.99e-05** |
+| MOF | CO<sub>2</sub> Henry coefficient | 8,183 | 0.737 | 0.468 | 0.426 | 0.362 | 0.295 | **0.288** |
+| MOF | Thermal stability | 3,098 | 68.74 | 49.27 | 52.38 | 52.557 | 45.875 | **45.766** |
+| COF | CH<sub>4</sub> uptake (65bar) | 39,304 | 5.588 | 4.630 | 15.31 | 2.883 | 2.268 | **2.126** |
+| COF | CH<sub>4</sub> uptake (5.8bar) | 39,304 | 3.444 | 1.853 | 5.620 | 1.255 | **0.999** | 1.009 | 
+| COF | CO<sub>2</sub> heat of adsorption | 39,304 | 2.101 | 1.341 | 1.846 | 1.058 | 0.874 | **0.842** |
+| COF | CO<sub>2</sub> log KH | 39,304 | 0.242 | 0.169 | 0.238 | 0.134 | 0.108 | **0.103** |
+| PPN | CH<sub>4</sub> uptake (65bar) | 17,870 | 6.260 | 4.233 | 9.731 | 3.748 | 3.187 | **2.995** | 
+| PPN | CH<sub>4</sub> uptake (1bar) | 17,870  | 1.356	| 0.563	| 1.525	| 0.602	| 0.493	| **0.461** | 
+| Zeolite | CH<sub>4</sub>  KH (unitless) | 99,204	| 8.032	| 6.268	| 6.334	| 4.286	| 4.103	| **3.998** |
+| Zeolite | CH<sub>4</sub>  Heat of adsorption | 99,204	| 1.612	|1.033	| 1.603	| 0.670	| 0.647	|**0.639** |
 
-Y. Kang, H. Park, B. Smit, J. Kim. "A multi-modal pre-training transformer for universal transfer learning in metal–organic frameworks", *Nature Machine Intelligence*, **(2023)** DOI: [https://doi.org/10.1038/s42256-023-00628-2](https://doi.org/10.1038/s42256-023-00628-2)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1 Name: moftransformer Version: 1.1.3 Summary:
+Metadata-Version: 2.1 Name: moftransformer Version: 2.0.0 Summary:
 moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
 Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
 docs/source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
-# [MOFTransformer](https://hspark1212.github.io/MOFTransformer/index.html) This
-package provides universal transfer learing for metal-organic frameworks(MOFs)
-to construct structure-property relationships. `MOFTransformer` obtains state-
-of-the-art performance to predict accross various properties that include gas
-adsorption, diffusion, electronic properties regardless of gas types. Beyond
-its universal transfer learning capabilityies, it provides feature importance
-analysis from its attentions scores to capture chemical intution. ## [Install]
-(https://hspark1212.github.io/MOFTransformer/installation.html) ### OS and
-hardware requirements The package development version is tested on following
-systems: Linux : Ubuntu 20.04, 22.04 For optimal performance, we recommend
-running with GPUs ### Depedencies ``` python>=3.8 ``` Given that MOFTransformer
-is based on pytorch, please install pytorch (>= 1.10.0) according to your
-environments. ### Installation using PIP ``` $ pip install moftransformer ```
-which should install in about 50 seconds. ### Download the pretrained model
-(ckpt file) - you can download the pretrained model with 1 M hMOFs in
-[figshare](https://figshare.com/articles/dataset/MOFTransformer/21155506) or
+# [PMTransformer (MOFTransformer)](https://hspark1212.github.io/MOFTransformer/
+index.html) This package provides a universal transfer learning model,
+`PMTransformer` (Porous Materials Transformer), which obtains the state-of-the-
+art performance in predicting various properties of porous materials. The
+PMTRansformer was pre-trainied with 1.9 million hypothetical porous materials
+including Metal-Organic Frameworks (MOFs), Covalent-Organic Frameworks (COFs),
+Porous Polymer Networks (PPNs), and zeolites. By fine-tuning the pre-trained
+`PMTransformer`, you can easily obtain machine learning models to accurately
+predict various properties of porous materials . NOTE: From version 2.0.0, the
+default pre-training model has been changed from `MOFTransformer` to
+`PMTransformer`, which was pre-trained with a larger dataset, containing other
+porous materials as well as MOFs. The `PMTransformer` outperforms the
+`MOFTransformer` in predicting various properties of porous materials. ##
+[Install](https://hspark1212.github.io/MOFTransformer/installation.html) ###
+Depedencies ``` python>=3.8 ``` Given that MOFTransformer is based on pytorch,
+please install pytorch (>= 1.12.0) according to your environments. ###
+Installation using PIP ``` $ pip install moftransformer ``` ### Download the
+pretrained models (ckpt file) - you can download the pretrained models
+(`PMTransformer.ckpt` and `MOFTransformer.ckpt`) [figshare](https://
+figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2) or
 you can download with a command line: ``` $ moftransformer download
-pretrain_model ``` ### (Optional) Download dataset for CoREMOF, QMOF - we've
-provide the dataset of MOFTransformer (i.e., atom-based graph embeddings and
-energy-grid embeddings) for CoREMOF, QMOF ``` $ moftransformer download coremof
-$ moftransformer download qmof ``` ## [Getting Started](https://
-hspark1212.github.io/MOFTransformer/tutorial.html) 1. At first, you can run
-`prepare_data` with 10 cifs in `moftransformer/examples/raw` directory. In
-order to run `prepare_data`, you need to install `GRIDAY` to calculate energy
-grid. You can download GRIDAY using command-line. ```bash $ moftransformer
-install-griday ``` Example for running `prepare-data` ```python from
-moftransformer.examples import example_path from moftransformer.utils import
-prepare_data # Get example path root_cifs = example_path['root_cif']
-root_dataset = example_path['root_dataset'] downstream = example_path
-['downstream'] train_fraction = 0.7 test_fraction = 0.2 # Run prepare data
-prepare_data(root_cifs, root_dataset, downstream=downstream,
-train_fraciton=train_fraction, test_fraciton=test_fraction) ``` 2. Fine-tune
-the pretrained MOFTransformer. ```python import moftransformer from
-moftransformer.examples import example_path # data root and downstream from
-example root_dataset = example_path['root_dataset'] downstream = example_path
-['downstream'] log_dir = './logs/' # kwargs (optional) max_epochs = 10
-batch_size = 8 moftransformer.run(root_dataset, downstream, log_dir=log_dir,
-max_epochs=max_epochs, batch_size=batch_size,) ``` which will run in about 35
-seconds. 3. Visualize analysis of feature importance for the fine-tuned model.
-download finetuned-bandgap model before visualize. ```bash moftransformer
-download finetuned_model -o ./examples ``` ```python %matplotlib widget from
-moftransformer.visualize import PatchVisualizer from moftransformer.examples
-import visualize_example_path model_path = "examples/finetuned_bandgap.ckpt" #
-or 'examples/finetuned_h2_uptake.ckpt' data_path = visualize_example_path
-cifname = 'MIBQAR01_FSR' vis = PatchVisualizer.from_cifname(cifname,
-model_path, data_path) vis.draw_graph() # or vis.draw_grid() ``` ##
-[Architecture](https://hspark1212.github.io/MOFTransformer/introduction.html)
-`MOFTransformer`is a multi-modal Transformer pre-trained with 1 million
-hypothetical MOFs so that it efficiently capture both local and global
-feeatures of MOFs. - `MOFformer` takes two different representations as input -
-Atom-based Graph Embedding : CGCNN w/o pooling layer -> local features -
-Energy-grid Embedding : 1D flatten patches of 3D energy grid -> global features
+pretrain_model ``` ### (Optional) Download pre-embeddings for CoREMOF, QMOF -
+we've provide the pre-embeddings (i.e., atom-based graph embeddings and energy-
+grid embeddings), inputs of `PMTransformer`, for CoREMOF, QMOF database. ``` $
+moftransformer download coremof $ moftransformer download qmof ``` ## [Getting
+Started](https://hspark1212.github.io/MOFTransformer/tutorial.html) 1. At
+first, you download dataset of hMOFs (20,000 MOFs) as an example. ``` $
+moftransformer download hmof ``` 2. Fine-tune the pretrained MOFTransformer.
+```python import moftransformer from moftransformer.examples import
+example_path # data root and downstream from example data_root = example_path
+['data_root'] downstream = example_path['downstream'] log_dir = './logs/' #
+load_path = "pmtransformer" (default) moftransformer.run(data_root, downstream,
+log_dir=log_dir, max_epochs=max_epochs, batch_size=batch_size,) ``` 3.
+Visualize analysis of feature importance for the fine-tuned model. ```python
+%matplotlib widget from visualize import PatchVisualizer model_path =
+"examples/finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt'
+data_path = 'examples/visualize/dataset/' cifname = 'MIBQAR01_FSR' vis =
+PatchVisualizer.from_cifname(cifname, model_path, data_path) vis.draw_graph() #
+or vis.draw_grid() ``` ## [Architecture](https://hspark1212.github.io/
+MOFTransformer/introduction.html) It is a multi-modal pre-training Transformer
+encoder which is designed to capture both local and global features of porous
+materials. The pre-traning tasks are as follows: (1) Topology Prediction (2)
+Void Fraction Prediction (3) Building Block Classification It takes two
+different representations as input - Atom-based Graph Embedding : CGCNN w/
+o pooling layer -> local features - Energy-grid Embedding : 1D flatten patches
+of 3D energy grid -> global features
 ## [Feature Importance Anaylsis](https://hspark1212.github.io/MOFTransformer/
 getting_started/visualization.html) you can easily visualize feature importance
 analysis of atom-based graph embeddings and energy-grid embeddings. ```python
 %matplotlib widget from visualize import PatchVisualizer model_path =
 "examples/finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt'
 data_path = 'examples/visualize/dataset/' cifname = 'MIBQAR01_FSR' vis =
 PatchVisualizer.from_cifname(cifname, model_path, data_path) vis.draw_graph()
 ```
    [https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/
                      source/getting_started/assets/1.gif]
-```python vis.draw_grid() ```
+```python vis = PatchVisualizer.from_cifname(cifname, model_path, data_path)
+vis.draw_grid() ```
    [https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/
                      source/getting_started/assets/3.gif]
-## Universal Transfer Learning | Property | MOFTransformer | Original Paper |
-Number of Data | Remarks | Reference | |---------------------------------------
----|----------------|----------------|----------------|------------------|-----
-------| |N2 uptake | R2: 0.78 | R2: 0.71 | 5,286 | CoRE MOF | 1 | |O2 uptake |
-R2: 0.83 | R2: 0.74 | 5,286 | CoRE MOF | 1 | |N2 diffusivity | R2: 0.77 | R2:
-0.76 | 5,286 | CoRE MOF | 1 | |O2 diffusivity | R2: 0.78 | R2: 0.74 | 5,286 |
-CoRE MOF | 1 | |CO2 Henry coefficient | MAE : 0.30 | MAE : 0.42 | 8,183 | CoRE
-MOF | 2 | |Solvent removal stability classification | ACC : 0.76 | ACC : 0.76 |
-2,148 | Text-mining data | 3 | |Thermal stability regression | R2 : 0.44 | R2 :
-0.46 | 3,098 | Text-mining data | 3 | ### Reference 1. [Prediction of O2/N2
-Selectivity in MetalâOrganic Frameworks via High-Throughput Computational
-Screening and Machine Learning](https://pubs.acs.org/doi/abs/10.1021/
-acsami.1c18521) 2. [Understanding the diversity of the metal-organic framework
-ecosystem](https://www.nature.com/articles/s41467-020-17755-8) 3. [Using
-Machine Learning and Data Mining to Leverage Community Knowledge for the
-Engineering of Stable MetalâOrganic Frameworks](https://pubs.acs.org/doi/
-10.1021/jacs.1c07217) ## Citation If you want to cite the MOFTransformer and
-the pre-training and fine-tuning dataset, please refer to the publication: Y.
-Kang, H. Park, B. Smit, J. Kim. "A multi-modal pre-training transformer for
-universal transfer learning in metalâorganic frameworks", *Nature Machine
-Intelligence*, **(2023)** DOI: [https://doi.org/10.1038/s42256-023-00628-2]
-(https://doi.org/10.1038/s42256-023-00628-2)
+## Universal Transfer Learning Comparison of mean absolute error (MAE) values
+for various baseline models, scratch, MOFTransformer, and PMTransformer on
+different properties of MOFs, COFs, PPNs, and zeolites. The bold values
+indicate the lowest MAE value for each property. The details of information can
+be found in [PMTransformer paper]() | Material | Property | Number of Dataset |
+Energy histogram | Descriptor-based ML | CGCNN | Scratch | MOFTransformer |
+PMTransformer | | --- | --- | --- | --- | --- | --- | --- | --- | --- | | MOF |
+H2 Uptake (100 bar) | 20,000 | 9.183 | 9.456 | 32.864 | 7.018 | 6.377 |
+**5.963** | | MOF | H2 diffusivity (dilute) | 20,000 | 0.644 | 0.398 | 0.6600 |
+0.391 | 0.367 | 0.**366** | | MOF | Band-gap | 20.373 | 0.913 | 0.590 | 0.290 |
+0.271 | 0.224 | **0.216** | | MOF | N2 uptake (1 bar) | 5,286 | 0.178 | 0.115 |
+0.108 | 0.102 | 0.071 | **0.069** | | MOF | O2 uptake (1 bar) | 5,286 | 0.162 |
+0.076 | 0.083 | 0.071 | **0.051** | 0.053 | | MOF | N2 diffusivity (1 bar) |
+5,286 | 7.82e-5 | 5.22e-5 | 7.19e-5 | 5.82e-05 | **4.52e-05** | 4.53e-05 | |
+MOF | O2 diffusivity (1 bar) | 5,286 | 7.14e-5 | 4.59e-5 | 6.56e-5 | 5.00e-05 |
+4.04e-05 | **3.99e-05** | | MOF | CO2 Henry coefficient | 8,183 | 0.737 | 0.468
+| 0.426 | 0.362 | 0.295 | **0.288** | | MOF | Thermal stability | 3,098 | 68.74
+| 49.27 | 52.38 | 52.557 | 45.875 | **45.766** | | COF | CH4 uptake (65bar) |
+39,304 | 5.588 | 4.630 | 15.31 | 2.883 | 2.268 | **2.126** | | COF | CH4 uptake
+(5.8bar) | 39,304 | 3.444 | 1.853 | 5.620 | 1.255 | **0.999** | 1.009 | | COF |
+CO2 heat of adsorption | 39,304 | 2.101 | 1.341 | 1.846 | 1.058 | 0.874 |
+**0.842** | | COF | CO2 log KH | 39,304 | 0.242 | 0.169 | 0.238 | 0.134 | 0.108
+| **0.103** | | PPN | CH4 uptake (65bar) | 17,870 | 6.260 | 4.233 | 9.731 |
+3.748 | 3.187 | **2.995** | | PPN | CH4 uptake (1bar) | 17,870 | 1.356 | 0.563
+| 1.525 | 0.602 | 0.493 | **0.461** | | Zeolite | CH4 KH (unitless) | 99,204 |
+8.032 | 6.268 | 6.334 | 4.286 | 4.103 | **3.998** | | Zeolite | CH4 Heat of
+adsorption | 99,204 | 1.612 |1.033 | 1.603 | 0.670 | 0.647 |**0.639** |
```

### Comparing `moftransformer-1.1.3/moftransformer.egg-info/SOURCES.txt` & `moftransformer-2.0.0/moftransformer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 moftransformer/__init__.py
 moftransformer/config.py
 moftransformer/config_ex.py
 moftransformer/run.py
+moftransformer/run_cp.py
 moftransformer.egg-info/PKG-INFO
 moftransformer.egg-info/SOURCES.txt
 moftransformer.egg-info/dependency_links.txt
 moftransformer.egg-info/entry_points.txt
 moftransformer.egg-info/requires.txt
 moftransformer.egg-info/top_level.txt
 moftransformer/assets/__init__.py
```


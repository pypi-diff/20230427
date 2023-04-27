# Comparing `tmp/obsinfo-0.111.1.post4.tar.gz` & `tmp/obsinfo-0.111b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsinfo-0.111.1.post4.tar", last modified: Wed Apr 26 21:37:11 2023, max compression
+gzip compressed data, was "obsinfo-0.111b1.tar", last modified: Wed Apr 12 06:31:11 2023, max compression
```

## Comparing `obsinfo-0.111.1.post4.tar` & `obsinfo-0.111b1.tar`

### file list

```diff
@@ -1,101 +1,301 @@
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.888550 obsinfo-0.111.1.post4/
--rw-r--r--   0 crawford   (501) admin       (80)    35148 2021-10-18 08:41:35.000000 obsinfo-0.111.1.post4/LICENSE.txt
--rw-r--r--   0 crawford   (501) admin       (80)      140 2021-10-18 08:41:35.000000 obsinfo-0.111.1.post4/MANIFEST.in
--rw-r--r--   0 crawford   (501) admin       (80)     1925 2023-04-26 21:37:11.888741 obsinfo-0.111.1.post4/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)     1032 2021-10-18 08:41:35.000000 obsinfo-0.111.1.post4/README.rst
--rw-r--r--   0 crawford   (501) admin       (80)      104 2021-10-18 08:41:35.000000 obsinfo-0.111.1.post4/pyproject.toml
--rw-r--r--   0 crawford   (501) admin       (80)       63 2023-04-26 21:37:11.889747 obsinfo-0.111.1.post4/setup.cfg
--rw-r--r--   0 crawford   (501) admin       (80)     2224 2023-04-26 21:31:44.000000 obsinfo-0.111.1.post4/setup.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.849504 obsinfo-0.111.1.post4/src/
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.853905 obsinfo-0.111.1.post4/src/obsinfo/
--rw-r--r--   0 crawford   (501) admin       (80)       17 2023-04-26 18:08:49.000000 obsinfo-0.111.1.post4/src/obsinfo/__init__.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.859252 obsinfo-0.111.1.post4/src/obsinfo/addons/
--rw-r--r--   0 crawford   (501) admin       (80)    11113 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/addons/LC2SDS.py
--rw-r--r--   0 crawford   (501) admin       (80)    10887 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/addons/LCHEAPO.py
--rw-r--r--   0 crawford   (501) admin       (80)     9134 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/addons/OCA.py
--rw-r--r--   0 crawford   (501) admin       (80)    15899 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/addons/SDPCHAIN.py
--rw-r--r--   0 crawford   (501) admin       (80)       64 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/addons/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     2481 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/addons/infodump.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.862303 obsinfo-0.111.1.post4/src/obsinfo/console_scripts/
--rw-r--r--   0 crawford   (501) admin       (80)      104 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/console_scripts/__init__.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    62825 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post4/src/obsinfo/console_scripts/_test.py
--rw-r--r--   0 crawford   (501) admin       (80)     7112 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/console_scripts/makeStationXML.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     7821 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/console_scripts/print.py
--rw-r--r--   0 crawford   (501) admin       (80)      289 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/console_scripts/print_version.py
--rw-r--r--   0 crawford   (501) admin       (80)     8214 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/console_scripts/setup.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    13974 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post4/src/obsinfo/console_scripts/validate.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.862685 obsinfo-0.111.1.post4/src/obsinfo/datacite/
--rw-r--r--   0 crawford   (501) admin       (80)        0 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/datacite/__init__.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.868200 obsinfo-0.111.1.post4/src/obsinfo/helpers/
--rw-r--r--   0 crawford   (501) admin       (80)      871 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/helpers/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     3091 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/helpers/comments.py
--rw-r--r--   0 crawford   (501) admin       (80)     1552 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/helpers/external_references.py
--rw-r--r--   0 crawford   (501) admin       (80)     3089 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/helpers/float_with_uncert.py
--rw-r--r--   0 crawford   (501) admin       (80)     1690 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/helpers/functions.py
--rw-r--r--   0 crawford   (501) admin       (80)     1493 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/helpers/identifiers.py
--rw-r--r--   0 crawford   (501) admin       (80)     6455 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/helpers/location.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     3336 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/helpers/logger.py
--rw-r--r--   0 crawford   (501) admin       (80)     2675 2023-04-26 21:31:44.000000 obsinfo-0.111.1.post4/src/obsinfo/helpers/obsinfo_class_list.py
--rw-r--r--   0 crawford   (501) admin       (80)     3169 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/helpers/oi_date.py
--rw-r--r--   0 crawford   (501) admin       (80)     2621 2023-04-26 21:31:44.000000 obsinfo-0.111.1.post4/src/obsinfo/helpers/person.py
--rw-r--r--   0 crawford   (501) admin       (80)     7685 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/helpers/phone.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.872477 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/
--rw-r--r--   0 crawford   (501) admin       (80)      830 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    11540 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/channel.py
--rw-r--r--   0 crawford   (501) admin       (80)     4950 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/equipment.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.876809 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/
--rw-r--r--   0 crawford   (501) admin       (80)     1806 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/AD_conversion.py
--rw-r--r--   0 crawford   (501) admin       (80)     2843 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/FIR.py
--rw-r--r--   0 crawford   (501) admin       (80)      506 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     1511 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/analog.py
--rw-r--r--   0 crawford   (501) admin       (80)     2309 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/coefficients.py
--rw-r--r--   0 crawford   (501) admin       (80)     1212 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/digital.py
--rw-r--r--   0 crawford   (501) admin       (80)     3202 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/filter.py
--rw-r--r--   0 crawford   (501) admin       (80)     1612 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/filter_template.py
--rw-r--r--   0 crawford   (501) admin       (80)     4963 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/poles_zeros.py
--rw-r--r--   0 crawford   (501) admin       (80)     2398 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/polynomial.py
--rw-r--r--   0 crawford   (501) admin       (80)     1588 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/response_list.py
--rw-r--r--   0 crawford   (501) admin       (80)    12127 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/instrument.py
--rw-r--r--   0 crawford   (501) admin       (80)    10005 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/instrument_component.py
--rw-r--r--   0 crawford   (501) admin       (80)    10115 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/instrumentation.py
--rw-r--r--   0 crawford   (501) admin       (80)     5482 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/orientation.py
--rw-r--r--   0 crawford   (501) admin       (80)    17385 2023-04-26 21:31:44.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/stage.py
--rw-r--r--   0 crawford   (501) admin       (80)     2959 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/instrumentation/stages.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.879416 obsinfo-0.111.1.post4/src/obsinfo/misc/
--rw-r--r--   0 crawford   (501) admin       (80)        0 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/misc/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     2497 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/misc/configuration.py
--rw-r--r--   0 crawford   (501) admin       (80)      866 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/misc/const.py
--rw-r--r--   0 crawford   (501) admin       (80)     4660 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/misc/discoveryfiles.py
--rw-r--r--   0 crawford   (501) admin       (80)     3062 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/misc/printobs.py
--rw-r--r--   0 crawford   (501) admin       (80)     4026 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/misc/remoteGitLab.py
--rw-r--r--   0 crawford   (501) admin       (80)    28035 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/misc/yamlref.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.880391 obsinfo-0.111.1.post4/src/obsinfo/obsmetadata/
--rw-r--r--   0 crawford   (501) admin       (80)       36 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/obsmetadata/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    25468 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post4/src/obsinfo/obsmetadata/obsmetadata.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.883558 obsinfo-0.111.1.post4/src/obsinfo/subnetwork/
--rw-r--r--   0 crawford   (501) admin       (80)      438 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/subnetwork/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     3090 2023-04-26 21:31:44.000000 obsinfo-0.111.1.post4/src/obsinfo/subnetwork/network.py
--rw-r--r--   0 crawford   (501) admin       (80)     2147 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/subnetwork/operator.py
--rw-r--r--   0 crawford   (501) admin       (80)     2094 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/subnetwork/processing.py
--rw-r--r--   0 crawford   (501) admin       (80)      654 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/subnetwork/site.py
--rw-r--r--   0 crawford   (501) admin       (80)    10459 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post4/src/obsinfo/subnetwork/station.py
--rw-r--r--   0 crawford   (501) admin       (80)     4727 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/subnetwork/subnetwork.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.886997 obsinfo-0.111.1.post4/src/obsinfo/tests/
--rw-r--r--   0 crawford   (501) admin       (80)     2880 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/tests/CompareXMLTree.py
--rw-r--r--   0 crawford   (501) admin       (80)       17 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/tests/__init__.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.888054 obsinfo-0.111.1.post4/src/obsinfo/tests/_old/
--rw-r--r--   0 crawford   (501) admin       (80)     5743 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/tests/_old/testlog.py
--rw-r--r--   0 crawford   (501) admin       (80)     4295 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/tests/_old/testmain.py
--rw-r--r--   0 crawford   (501) admin       (80)     1159 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/tests/remoteGithub.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    73575 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post4/src/obsinfo/tests/run_test_script.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    35088 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/tests/test_datapath.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    53975 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/tests/test_infofile.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     2148 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post4/src/obsinfo/tests/test_main.py
--rw-r--r--   0 crawford   (501) admin       (80)       30 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post4/src/obsinfo/version.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-26 21:37:11.856524 obsinfo-0.111.1.post4/src/obsinfo.egg-info/
--rw-r--r--   0 crawford   (501) admin       (80)     1925 2023-04-26 21:37:11.000000 obsinfo-0.111.1.post4/src/obsinfo.egg-info/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)     2981 2023-04-26 21:37:11.000000 obsinfo-0.111.1.post4/src/obsinfo.egg-info/SOURCES.txt
--rw-r--r--   0 crawford   (501) admin       (80)        1 2023-04-26 21:37:11.000000 obsinfo-0.111.1.post4/src/obsinfo.egg-info/dependency_links.txt
--rw-r--r--   0 crawford   (501) admin       (80)      586 2023-04-26 21:37:11.000000 obsinfo-0.111.1.post4/src/obsinfo.egg-info/entry_points.txt
--rw-r--r--   0 crawford   (501) admin       (80)       85 2023-04-26 21:37:11.000000 obsinfo-0.111.1.post4/src/obsinfo.egg-info/requires.txt
--rw-r--r--   0 crawford   (501) admin       (80)        8 2023-04-26 21:37:11.000000 obsinfo-0.111.1.post4/src/obsinfo.egg-info/top_level.txt
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.575257 obsinfo-0.111b1/
+-rw-r--r--   0 crawford   (501) admin       (80)    35148 2021-10-18 08:41:35.000000 obsinfo-0.111b1/LICENSE.txt
+-rw-r--r--   0 crawford   (501) admin       (80)      140 2021-10-18 08:41:35.000000 obsinfo-0.111b1/MANIFEST.in
+-rw-r--r--   0 crawford   (501) admin       (80)     1919 2023-04-12 06:31:11.575447 obsinfo-0.111b1/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)     1032 2021-10-18 08:41:35.000000 obsinfo-0.111b1/README.rst
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.481113 obsinfo-0.111b1/obsinfo/
+-rw-r--r--   0 crawford   (501) admin       (80)       17 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/__init__.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.483686 obsinfo-0.111b1/obsinfo/_examples/
+-rw-r--r--   0 crawford   (501) admin       (80)    10244 2023-02-06 14:21:22.000000 obsinfo-0.111b1/obsinfo/_examples/.DS_Store
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.484720 obsinfo-0.111b1/obsinfo/_examples/Information_Files/
+-rw-r--r--   0 crawford   (501) admin       (80)    12292 2023-04-10 11:11:33.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      828 2023-02-06 14:15:15.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/README.rst
+-rw-r--r--   0 crawford   (501) admin       (80)       90 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/README.txt
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.485116 obsinfo-0.111b1/obsinfo/_examples/Information_Files/campaigns/
+-rw-r--r--   0 crawford   (501) admin       (80)     2053 2023-04-10 16:23:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/campaigns/SPOBS.campaign.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.485576 obsinfo-0.111b1/obsinfo/_examples/Information_Files/datacites/
+-rw-r--r--   0 crawford   (501) admin       (80)     1731 2023-04-10 16:23:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/datacites/EMSO-MOMAR_OBS.datacite.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.486341 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/
+-rw-r--r--   0 crawford   (501) admin       (80)     1763 2023-03-22 08:38:06.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/ADS1281.datalogger_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     5880 2023-03-22 08:38:32.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/LC2000.datalogger_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.490625 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 18:40:52.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      729 2023-04-11 18:33:44.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5321_FIR1.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      618 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      605 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.with-delay.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      556 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR3.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      592 2023-02-28 16:43:08.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_100sps-SINC.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      596 2023-02-28 16:43:14.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_200sps-SINC.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      436 2023-02-28 16:43:36.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR1.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      435 2023-02-28 16:43:35.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR2.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      443 2023-02-28 16:43:29.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR3_LINEAR.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      443 2023-02-28 16:43:33.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR4_LINEAR.stage_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.492895 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)      480 2023-02-28 16:44:38.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR2.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2412 2023-02-28 16:44:43.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR3.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      283 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR1.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      268 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR2.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      578 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR3-linear.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1118 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR4-linear.filter.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.493597 obsinfo-0.111b1/obsinfo/_examples/Information_Files/experiments/
+-rw-r--r--   0 crawford   (501) admin       (80)    16208 2023-03-01 16:50:51.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/experiments/MAYOBS.experiment.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)    19366 2023-04-10 16:23:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/experiments/MOMAR.experiment.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.497398 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:33:43.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)     3594 2023-04-12 06:20:50.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_2012+.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2189 2023-04-11 21:33:49.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_pre2012.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     4527 2023-03-22 08:38:31.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/GURALP_CP.instrumentation_base.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1084 2023-03-07 15:14:40.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/HYDROCT1.instrumentation_base.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1265 2023-03-07 15:14:50.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS1.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1451 2023-03-07 15:15:08.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS2.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1732 2023-03-07 15:20:23.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS3-for-channel-mod-testing.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1554 2023-03-07 15:20:21.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/WBOBS1.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1885 2023-03-07 15:14:30.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/empty.instrumentation_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.498130 obsinfo-0.111b1/obsinfo/_examples/Information_Files/location_bases/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 16:53:33.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/location_bases/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)     1356 2023-02-27 22:12:01.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/location_bases/INSU-IPGP.location_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.499002 obsinfo-0.111b1/obsinfo/_examples/Information_Files/networks/
+-rw-r--r--   0 crawford   (501) admin       (80)      329 2023-04-11 08:09:43.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/networks/EMSO-AZORES.network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      413 2023-04-11 08:09:59.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/networks/RHUM-RUM.network.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.499765 obsinfo-0.111b1/obsinfo/_examples/Information_Files/operators/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-11-30 17:19:05.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/operators/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      345 2023-02-28 16:41:26.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/operators/INSU-IPGP.operator.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.501222 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/
+-rw-r--r--   0 crawford   (501) admin       (80)      159 2023-02-28 16:46:55.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/Kevin_Canjamale.person.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)       98 2023-02-28 16:47:13.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/Romuald_Daniel.person.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      100 2023-02-28 16:47:05.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/Simon_Besancon.person.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      166 2023-02-28 16:46:47.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/Wayne_Crawford.person.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.503298 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/
+-rw-r--r--   0 crawford   (501) admin       (80)      643 2023-02-27 22:11:57.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_BBOBS.preamplifier_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      448 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_DPG.preamplifier_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      811 2023-02-27 22:11:40.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_GEOPHONE.preamplifier_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      797 2023-02-27 22:11:34.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO-no_redundancy.preamplifier_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      797 2023-02-27 22:11:25.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.504754 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/
+-rw-r--r--   0 crawford   (501) admin       (80)      451 2023-02-27 22:11:22.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_BBOBS_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      662 2023-02-27 22:11:20.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_geophone_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      698 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/SIO-LDEO_DPG-Card_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      821 2023-02-27 22:11:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/Scripps_SPOBS_HydroL22_theoretical.stage_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.508004 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/
+-rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-02-06 14:13:53.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      661 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/HITECH_HTI04-PLC-ULF.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      752 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/HITECH_HTI90U.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2341 2023-04-11 21:38:03.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240__theoretical.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1425 2023-02-27 22:11:14.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240_plusDates.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      835 2023-04-11 14:10:42.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_TCOMPACT_theoretical.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      652 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SERCEL_L22.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      698 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SERCEL_L28.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2009 2023-02-27 22:11:07.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SIO_DPG.sensor_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.512065 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/
+-rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-02-06 14:13:53.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      430 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1341 2023-01-09 11:31:34.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-90U_SIO-preamp_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      536 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5004_calibrated.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      527 2023-04-11 13:55:08.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5018_calibrated.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      382 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_generic_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      485 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L22D_LCHEAPO_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      537 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L28LB_LCHEAPO_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1233 2023-02-27 22:11:02.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Trillium_T240__theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      586 2023-02-27 22:11:00.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Trillium_TCompact__theoretical.stage_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.516249 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2023-01-09 11:32:20.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      280 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      310 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5004_2007.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      306 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5017_2007.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      364 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      383 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L22D_C510-S2000_generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      236 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L28LB-obs_C395-S2490_generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      728 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN1-399_generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      873 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN400-_generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      547 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_TCompact__generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      854 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/test---attributes-poleszeros.filter.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.521703 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2023-04-11 10:41:26.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)        5 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/.obsinfo
+-rw-r--r--   0 crawford   (501) admin       (80)     3690 2023-04-11 08:10:25.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP.subnetwork.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3429 2023-04-11 21:13:12.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP_with_gain_mods.subnetwork.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2798 2023-04-11 10:40:05.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EMPTY-INSTRUMENTATION.INSU-IPGP.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2835 2023-04-12 06:00:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2211 2023-04-11 08:10:30.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential_noRefs.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1890 2023-04-11 21:46:11.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/LEAP_SECOND.INSU-IPGP.subnetwork.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3197 2023-04-11 18:07:50.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/ORIENTED.INSU-IPGP.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3092 2023-04-11 18:07:24.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/SPOBS.INSU-IPGP.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2699 2023-04-11 18:07:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/SPOBS_noAnchors.INSU-IPGP.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2017 2023-04-11 18:44:22.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/TEST.subnetwork.yaml_error.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.522621 obsinfo-0.111b1/obsinfo/_examples/Information_Files/timing_bases/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 16:53:33.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/timing_bases/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      252 2023-01-17 15:49:59.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/timing_bases/Seascan_GNSS.timing_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.473509 obsinfo-0.111b1/obsinfo/_examples/Training/
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.525281 obsinfo-0.111b1/obsinfo/_examples/Training/templates/
+-rw-r--r--   0 crawford   (501) admin       (80)     1308 2023-04-11 08:12:26.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS-train.network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3185 2023-04-11 08:12:46.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS.INSU-IPGP.network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1501 2023-01-17 18:01:07.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS1.instrumentation.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1625 2023-01-17 18:00:12.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS1_2012+.instrumentation.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      573 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/CS5322.stage.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1047 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/T240.stage.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.526768 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/
+-rw-r--r--   0 crawford   (501) admin       (80)     3049 2023-03-22 08:38:30.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/LC2000-1.datalogger.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3053 2023-03-22 08:38:26.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/LC2000.datalogger.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      907 2023-03-21 09:43:56.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/preamplifier.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1257 2023-03-21 09:44:03.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/sensor.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.530043 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)      263 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/AD_Conversion.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      673 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/CirrusLogic_FIR.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      607 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/ExampleFIR.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      409 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/HiTechPZ.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      416 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/HiTech_PolesZeros.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      191 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/analog.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      390 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/coefficients.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      310 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/digital.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      379 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/response_list.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2175 2023-04-11 08:12:58.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/network.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.531754 obsinfo-0.111b1/obsinfo/_examples/scripts/
+-rw-r--r--   0 crawford   (501) admin       (80)      292 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/README.rst
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.532400 obsinfo-0.111b1/obsinfo/_examples/scripts/add_ons/
+-rw-r--r--   0 crawford   (501) admin       (80)      331 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/add_ons/README.rst
+-rw-r--r--   0 crawford   (501) admin       (80)      952 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/add_ons/make_data_process_scripts.sh
+-rwxr-xr-x   0 crawford   (501) admin       (80)      376 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/make_stationXML.sh
+-rwxr-xr-x   0 crawford   (501) admin       (80)      420 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/print_info_files.sh
+-rwxr-xr-x   0 crawford   (501) admin       (80)     1646 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/validate_all.sh
+-rwxr-xr-x   0 crawford   (501) admin       (80)      315 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/validate_files.sh
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.534403 obsinfo-0.111b1/obsinfo/addons/
+-rw-r--r--   0 crawford   (501) admin       (80)     9904 2023-01-05 14:22:59.000000 obsinfo-0.111b1/obsinfo/addons/LC2SDS.py
+-rw-r--r--   0 crawford   (501) admin       (80)    10899 2023-01-05 14:26:17.000000 obsinfo-0.111b1/obsinfo/addons/LCHEAPO.py
+-rw-r--r--   0 crawford   (501) admin       (80)     9134 2023-04-11 08:13:40.000000 obsinfo-0.111b1/obsinfo/addons/OCA.py
+-rw-r--r--   0 crawford   (501) admin       (80)    15899 2023-04-11 08:13:46.000000 obsinfo-0.111b1/obsinfo/addons/SDPCHAIN.py
+-rw-r--r--   0 crawford   (501) admin       (80)       64 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/addons/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2481 2023-01-05 14:20:29.000000 obsinfo-0.111b1/obsinfo/addons/infodump.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.537195 obsinfo-0.111b1/obsinfo/console_scripts/
+-rw-r--r--   0 crawford   (501) admin       (80)      104 2023-04-11 12:05:29.000000 obsinfo-0.111b1/obsinfo/console_scripts/__init__.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    63491 2023-03-22 08:38:16.000000 obsinfo-0.111b1/obsinfo/console_scripts/_test.py
+-rw-r--r--   0 crawford   (501) admin       (80)     7941 2023-04-12 05:49:55.000000 obsinfo-0.111b1/obsinfo/console_scripts/makeStationXML.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     8399 2023-04-12 05:27:13.000000 obsinfo-0.111b1/obsinfo/console_scripts/print.py
+-rw-r--r--   0 crawford   (501) admin       (80)      289 2022-06-20 07:21:38.000000 obsinfo-0.111b1/obsinfo/console_scripts/print_version.py
+-rw-r--r--   0 crawford   (501) admin       (80)     8160 2023-04-12 05:54:26.000000 obsinfo-0.111b1/obsinfo/console_scripts/setup.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    17057 2023-04-12 05:58:43.000000 obsinfo-0.111b1/obsinfo/console_scripts/validate.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.475272 obsinfo-0.111b1/obsinfo/data/
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.544142 obsinfo-0.111b1/obsinfo/data/schemas/
+-rw-r--r--   0 crawford   (501) admin       (80)     8861 2023-03-03 09:25:57.000000 obsinfo-0.111b1/obsinfo/data/schemas/datacite.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     5514 2023-03-25 15:00:10.000000 obsinfo-0.111b1/obsinfo/data/schemas/datalogger_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)    10023 2023-04-11 15:24:46.000000 obsinfo-0.111b1/obsinfo/data/schemas/definitions.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-04-11 08:14:23.000000 obsinfo-0.111b1/obsinfo/data/schemas/experiment.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)    13582 2023-04-06 17:48:52.000000 obsinfo-0.111b1/obsinfo/data/schemas/filter.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     8241 2023-04-11 10:28:57.000000 obsinfo-0.111b1/obsinfo/data/schemas/instrumentation_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     1378 2022-11-30 17:16:16.000000 obsinfo-0.111b1/obsinfo/data/schemas/iris_units.json
+-rw-r--r--   0 crawford   (501) admin       (80)     6575 2023-04-11 15:31:38.000000 obsinfo-0.111b1/obsinfo/data/schemas/location_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     1922 2023-04-11 08:14:35.000000 obsinfo-0.111b1/obsinfo/data/schemas/network.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     1407 2023-04-06 14:54:32.000000 obsinfo-0.111b1/obsinfo/data/schemas/operator.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     1735 2023-02-28 08:30:05.000000 obsinfo-0.111b1/obsinfo/data/schemas/person.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     4650 2023-03-25 15:00:19.000000 obsinfo-0.111b1/obsinfo/data/schemas/preamplifier_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     6472 2023-03-25 15:00:00.000000 obsinfo-0.111b1/obsinfo/data/schemas/sensor_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     8193 2023-04-06 17:50:39.000000 obsinfo-0.111b1/obsinfo/data/schemas/stage_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     2051 2023-03-21 13:52:11.000000 obsinfo-0.111b1/obsinfo/data/schemas/stages.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     7216 2023-04-11 10:58:00.000000 obsinfo-0.111b1/obsinfo/data/schemas/subnetwork.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     3997 2023-02-28 16:48:56.000000 obsinfo-0.111b1/obsinfo/data/schemas/timing_base.schema.json
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.544468 obsinfo-0.111b1/obsinfo/datacite/
+-rw-r--r--   0 crawford   (501) admin       (80)        0 2023-01-19 09:54:12.000000 obsinfo-0.111b1/obsinfo/datacite/__init__.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.548405 obsinfo-0.111b1/obsinfo/helpers/
+-rw-r--r--   0 crawford   (501) admin       (80)      729 2023-04-11 09:20:15.000000 obsinfo-0.111b1/obsinfo/helpers/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3091 2023-04-06 13:54:33.000000 obsinfo-0.111b1/obsinfo/helpers/comments.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1565 2023-04-06 13:06:26.000000 obsinfo-0.111b1/obsinfo/helpers/external_references.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3089 2023-04-12 05:45:13.000000 obsinfo-0.111b1/obsinfo/helpers/float_with_uncert.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1518 2023-04-11 16:29:35.000000 obsinfo-0.111b1/obsinfo/helpers/functions.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1506 2023-04-11 09:14:43.000000 obsinfo-0.111b1/obsinfo/helpers/identifiers.py
+-rw-r--r--   0 crawford   (501) admin       (80)     6469 2023-04-05 13:41:46.000000 obsinfo-0.111b1/obsinfo/helpers/location.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3401 2023-04-11 14:33:07.000000 obsinfo-0.111b1/obsinfo/helpers/obsinfo_class_list.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3622 2023-04-02 23:37:37.000000 obsinfo-0.111b1/obsinfo/helpers/oi_date.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2621 2023-04-11 14:26:19.000000 obsinfo-0.111b1/obsinfo/helpers/person.py
+-rw-r--r--   0 crawford   (501) admin       (80)     7685 2023-04-06 07:43:07.000000 obsinfo-0.111b1/obsinfo/helpers/phone.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.551585 obsinfo-0.111b1/obsinfo/instrumentation/
+-rw-r--r--   0 crawford   (501) admin       (80)      830 2023-04-11 10:13:55.000000 obsinfo-0.111b1/obsinfo/instrumentation/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    11457 2023-04-12 05:43:58.000000 obsinfo-0.111b1/obsinfo/instrumentation/channel.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4969 2023-04-11 15:24:42.000000 obsinfo-0.111b1/obsinfo/instrumentation/equipment.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.555415 obsinfo-0.111b1/obsinfo/instrumentation/filter/
+-rw-r--r--   0 crawford   (501) admin       (80)     1850 2023-04-03 16:39:05.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/AD_conversion.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2814 2023-04-12 06:16:41.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/FIR.py
+-rw-r--r--   0 crawford   (501) admin       (80)      506 2023-01-30 15:51:03.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1555 2023-04-11 16:22:34.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/analog.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2353 2023-04-03 16:39:20.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/coefficients.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1256 2023-04-03 16:40:13.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/digital.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3106 2023-03-10 16:10:10.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/filter.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1656 2023-04-06 17:54:00.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/filter_template.py
+-rw-r--r--   0 crawford   (501) admin       (80)     5290 2023-04-11 16:27:01.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/poles_zeros.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2442 2023-04-03 16:39:41.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/polynomial.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1854 2023-04-03 16:39:53.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/response_list.py
+-rw-r--r--   0 crawford   (501) admin       (80)    12143 2023-04-11 22:07:58.000000 obsinfo-0.111b1/obsinfo/instrumentation/instrument.py
+-rw-r--r--   0 crawford   (501) admin       (80)     9710 2023-04-11 18:45:31.000000 obsinfo-0.111b1/obsinfo/instrumentation/instrument_component.py
+-rw-r--r--   0 crawford   (501) admin       (80)    10284 2023-04-11 18:01:13.000000 obsinfo-0.111b1/obsinfo/instrumentation/instrumentation.py
+-rw-r--r--   0 crawford   (501) admin       (80)     5442 2023-03-27 23:26:01.000000 obsinfo-0.111b1/obsinfo/instrumentation/orientation.py
+-rw-r--r--   0 crawford   (501) admin       (80)    17057 2023-04-06 17:59:14.000000 obsinfo-0.111b1/obsinfo/instrumentation/stage.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2771 2023-04-03 14:12:36.000000 obsinfo-0.111b1/obsinfo/instrumentation/stages.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.557913 obsinfo-0.111b1/obsinfo/misc/
+-rw-r--r--   0 crawford   (501) admin       (80)        0 2022-06-24 14:31:17.000000 obsinfo-0.111b1/obsinfo/misc/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2497 2022-06-24 14:30:50.000000 obsinfo-0.111b1/obsinfo/misc/configuration.py
+-rw-r--r--   0 crawford   (501) admin       (80)      866 2022-06-24 14:29:23.000000 obsinfo-0.111b1/obsinfo/misc/const.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4660 2022-06-24 14:27:52.000000 obsinfo-0.111b1/obsinfo/misc/discoveryfiles.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3062 2023-03-21 09:50:57.000000 obsinfo-0.111b1/obsinfo/misc/printobs.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4026 2022-06-24 14:17:30.000000 obsinfo-0.111b1/obsinfo/misc/remoteGitLab.py
+-rw-r--r--   0 crawford   (501) admin       (80)    28034 2023-04-06 17:16:02.000000 obsinfo-0.111b1/obsinfo/misc/yamlref.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.558622 obsinfo-0.111b1/obsinfo/obsMetadata/
+-rw-r--r--   0 crawford   (501) admin       (80)       37 2023-02-15 09:27:51.000000 obsinfo-0.111b1/obsinfo/obsMetadata/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    25122 2023-04-11 21:42:28.000000 obsinfo-0.111b1/obsinfo/obsMetadata/obsmetadata.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.560673 obsinfo-0.111b1/obsinfo/subnetwork/
+-rw-r--r--   0 crawford   (501) admin       (80)      376 2023-04-06 14:04:52.000000 obsinfo-0.111b1/obsinfo/subnetwork/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2138 2023-04-11 10:19:15.000000 obsinfo-0.111b1/obsinfo/subnetwork/operator.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2094 2023-04-11 18:04:18.000000 obsinfo-0.111b1/obsinfo/subnetwork/processing.py
+-rw-r--r--   0 crawford   (501) admin       (80)      654 2023-04-06 13:55:11.000000 obsinfo-0.111b1/obsinfo/subnetwork/site.py
+-rw-r--r--   0 crawford   (501) admin       (80)    10316 2023-04-11 18:15:51.000000 obsinfo-0.111b1/obsinfo/subnetwork/station.py
+-rw-r--r--   0 crawford   (501) admin       (80)     6326 2023-04-11 10:58:08.000000 obsinfo-0.111b1/obsinfo/subnetwork/subnetwork.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.562051 obsinfo-0.111b1/obsinfo/template_specifications/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:14:05.000000 obsinfo-0.111b1/obsinfo/template_specifications/.DS_Store
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.563040 obsinfo-0.111b1/obsinfo/template_specifications/components/
+-rw-r--r--   0 crawford   (501) admin       (80)     1439 2023-03-22 08:38:14.000000 obsinfo-0.111b1/obsinfo/template_specifications/components/datalogger.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1076 2023-03-21 09:51:15.000000 obsinfo-0.111b1/obsinfo/template_specifications/components/preamplifier.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1438 2023-03-21 09:51:26.000000 obsinfo-0.111b1/obsinfo/template_specifications/components/sensor.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.565577 obsinfo-0.111b1/obsinfo/template_specifications/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)      276 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/AD_Conversion.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      449 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/FIR.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      603 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/PolesZeros.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      194 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/analog.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      410 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/coefficients.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      320 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/digital.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      401 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/response_list.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1419 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/instrumentation.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2483 2023-04-11 08:15:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1113 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/stage.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.567437 obsinfo-0.111b1/obsinfo/templates/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:14:05.000000 obsinfo-0.111b1/obsinfo/templates/.DS_Store
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.568612 obsinfo-0.111b1/obsinfo/templates/components/
+-rw-r--r--   0 crawford   (501) admin       (80)     1265 2023-03-22 08:38:17.000000 obsinfo-0.111b1/obsinfo/templates/components/datalogger.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      907 2023-03-21 09:51:36.000000 obsinfo-0.111b1/obsinfo/templates/components/preamplifier.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1257 2023-03-21 09:51:42.000000 obsinfo-0.111b1/obsinfo/templates/components/sensor.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.571652 obsinfo-0.111b1/obsinfo/templates/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)      263 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/AD_Conversion.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      435 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/FIR.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      561 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/PolesZeros.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      191 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/analog.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      390 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/coefficients.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      310 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/digital.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      379 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/response_list.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1327 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/instrumentation.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2176 2023-04-11 08:15:41.000000 obsinfo-0.111b1/obsinfo/templates/network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1055 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/stage.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.574845 obsinfo-0.111b1/obsinfo/tests/
+-rw-r--r--   0 crawford   (501) admin       (80)     2880 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/tests/CompareXMLTree.py
+-rw-r--r--   0 crawford   (501) admin       (80)       17 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/tests/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1159 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/tests/remoteGithub.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    74280 2023-03-25 15:32:18.000000 obsinfo-0.111b1/obsinfo/tests/run_test_script.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    35142 2023-03-25 15:32:14.000000 obsinfo-0.111b1/obsinfo/tests/test_datapath.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    54029 2023-03-25 15:30:33.000000 obsinfo-0.111b1/obsinfo/tests/test_infofile.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     2148 2023-02-15 16:43:20.000000 obsinfo-0.111b1/obsinfo/tests/test_main.py
+-rw-r--r--   0 crawford   (501) admin       (80)       24 2023-04-12 06:30:25.000000 obsinfo-0.111b1/obsinfo/version.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.483199 obsinfo-0.111b1/obsinfo.egg-info/
+-rw-r--r--   0 crawford   (501) admin       (80)     1919 2023-04-12 06:31:10.000000 obsinfo-0.111b1/obsinfo.egg-info/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)    14855 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        1 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 crawford   (501) admin       (80)      586 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/entry_points.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       85 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/requires.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        8 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/top_level.txt
+-rw-r--r--   0 crawford   (501) admin       (80)      104 2021-10-18 08:41:35.000000 obsinfo-0.111b1/pyproject.toml
+-rw-r--r--   0 crawford   (501) admin       (80)       63 2023-04-12 06:31:11.576223 obsinfo-0.111b1/setup.cfg
+-rw-r--r--   0 crawford   (501) admin       (80)     2261 2023-04-12 05:54:29.000000 obsinfo-0.111b1/setup.py
```

### Comparing `obsinfo-0.111.1.post4/LICENSE.txt` & `obsinfo-0.111b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/PKG-INFO` & `obsinfo-0.111b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsinfo
-Version: 0.111.1.post4
+Version: 0.111b1
 Summary: Tools for documenting ocean bottom seismometer experiments and creating metadata
 Home-page: https://gitlab.com/resif/obsinfo
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: seismology OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `obsinfo-0.111.1.post4/README.rst` & `obsinfo-0.111b1/README.rst`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/setup.py` & `obsinfo-0.111b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
     print(long_description)
     
 version={}
-with open("src/obsinfo/version.py") as fp:
+with open("obsinfo/version.py") as fp:
     exec(fp.read(),version)
 
 setuptools.setup(
     name="obsinfo",
     version=version['__version__'],
     author="Wayne Crawford",
     author_email="crawford@ipgp.fr",
     description="Tools for documenting ocean bottom seismometer experiments and creating metadata",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://gitlab.com/resif/obsinfo",
+    packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=[
           'numpy>=1',
           'obspy>=1.1',
           'pyyaml>=3.0',
           'jsonschema>=3.2,<4',
           'python-gitlab>=2.9.0',
@@ -38,22 +39,22 @@
             'obsinfo-makescripts_LCHEAPO=obsinfo.addons.LCHEAPO:_console_script',
             'obsinfo-makescripts_LC2SDS=obsinfo.addons.LC2SDS:_console_script'
         ]
     },
     python_requires='>=3.9',
     setup_requires=["pytest-runner"],
     tests_require=["pytest"],
-    classifiers=[
+    classifiers=(
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Physics"
-    ],
+    ),
     keywords='seismology OBS'
 )
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/addons/LC2SDS.py` & `obsinfo-0.111b1/obsinfo/addons/LC2SDS.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 """
 Write a script to convert LCHEAPO data to SDS* using the lcheapo** python package
 
 Includes clock drift and leap-second correction
 Script is a BASH shell script
 *SDS = SeisComp Data Structure
-**THIS PROGRAM DOES NOT CREATE DATA-CENTER QUALITY DATA:
+**THE LCHEAPO PACKAGE DOES NOT CREATE DATA-CENTER QUALITY DATA:
     - drift correction is calculated for each day, not each record
     - does not set drift correction record header flags
     - does not fill in record header time_correction field
 """
 import os.path
 from pathlib import Path
 import warnings
 
 # import obsinfo
 from obsinfo.subnetwork import Subnetwork
 from ..misc.discoveryfiles import (Datapath)
-from ..obsmetadata import (ObsMetadata)
+from ..obsMetadata.obsmetadata import (ObsMetadata)
 from .LCHEAPO import _get_ref_code
 
 SEPARATOR_LINE = "\n# " + 60 * "=" + "\n"
 
 
 def process_script(network_code, stations, station_data_path, input_dir=".",
-                   output_dir="../", include_header=True, no_drift_correct=False):
+                   output_dir="../", include_header=True):
     """
     Writes script to transform raw OBS data to SeisComp Data Structure
 
     Arguments:
         network_code (str): FDSN network_code
         stations (list of :class:`.Station`): the stations to process
         station_data_path (str): the base directory beneath the station data dirs
         input_dir (str): directory beneath station_dir for LCHEAPO data
         output_dir (str): directory beneath station_dir for SDS directory
         include_header (bool): include the header that sets up paths
                                (should be done once)
-        no_drift_correct (bool): Do NOT drift correct
     """
     fixed_dir = "lcheapo_fixed"
     s = _header(station_data_path)
     s += _run_station_function(network_code, fixed_dir, output_dir)
     for station in stations:
         # station_dir = os.path.join(station_data_path, station.label)
-        s += _run_station_call(station, no_drift_correct)
+        s += _run_station_call(station)
     return s
 
 
 def _header(station_data_path):
     s = "#!/bin/bash\n\n"
     s += f'DATA_DIR={station_data_path}\n\n'
     return s
@@ -55,15 +54,15 @@
 def _run_station_function(network_code, fixed_dir='lcheapo_fixed', output_dir="../"):
     s = ('run_station () {\n'
          '    # Run lcfix and lc2SDS_weak for one station\n'
          '    # $1: station name\n'
          '    # $2: obs type\n'
          '    # $3: reference start sync time\n'
          '    # $4: instrument start sync time [if empty, uses $3]\n'
-         '    # $5: reference end sync time [if empty, do not shift times]\n'
+         '    # $5: reference end sync time\n'
          '    # $6: obs clock end sync time\n'
          '    # $7: leap-second times [empty if none]\n'
          '    # $8: leap-second types [empty if none]\n'
          '    echo "Working on station $1"\n'
          '    STATION_DIR=$DATA_DIR/$1\n'
          '    echo "------------------------------------------------------------"\n'
          '    echo "Running LCFIX"\n'
@@ -77,29 +76,23 @@
          '    echo "Running LC2SDS_weak"\n'
          f'    mkdir -p $STATION_DIR/{output_dir}\n'
          f'    command cd $STATION_DIR/{fixed_dir}\n'
          '    lchfiles=$(command ls *.fix.lch)\n'
          '    command cd -\n'
          '    echo "lchfiles:" $lchfiles\n'
          '    if [ -z "$7" ]\n'
-         '    then  # NO LEAP-SECOND INFORMATION\n'
-         '        if [ -z "$5" ]\n'
-         '        then  # NO END SYNC, DO NOT SHIFT TIMES\n'
-         f'            cmd="lc2SDS_weak $lchfiles -d \\"$STATION_DIR\\" -i \\"{fixed_dir}\\" -o \\"{output_dir}\\" --network \\"{network_code}\\" --station \\"$1\\" --obs_type \\"$2\\""\n'
-         '        elif [ -z "$4" ]\n'
-         '        then  # NO INSTRUMENT START SYNC, ASSUME SAME AS REFERENCE\n'
+         '    then\n'
+         '        if [ -z "$4" ]\n'
+         '        then\n'
          f'            cmd="lc2SDS_weak $lchfiles -d \\"$STATION_DIR\\" -i \\"{fixed_dir}\\" -o \\"{output_dir}\\" --network \\"{network_code}\\" --station \\"$1\\" --obs_type \\"$2\\" --start_times \\"$3\\" --end_times \\"$5\\" \\"$6\\""\n'
-         '        else  # INSTRUMENT START SYNC SUPPLIED\n'
+         '        else\n'
          f'            cmd="lc2SDS_weak $lchfiles -d \\"$STATION_DIR\\" -i \\"{fixed_dir}\\" -o \\"{output_dir}\\" --network \\"{network_code}\\" --station \\"$1\\" --obs_type \\"$2\\" --start_times \\"$3\\" \\"$4\\" --end_times \\"$5\\" \\"$6\\""\n'
          '        fi\n'
-         '    else  # THERE IS LEAP-SECOND INFORMATION\n'
-         '        if [ -z "$5" ]\n'
-         '        then\n'
-         f'            cmd="lc2SDS_weak $lchfiles -d \\"$STATION_DIR\\" -i \\"{fixed_dir}\\" -o \\"{output_dir}\\" --network \\"{network_code}\\" --station \\"$1\\" --obs_type \\"$2\\" --leapsecond_times \\"$7\\" --leapsecond_types \\"$8\\""\n'
-         '        elif [ -z "$4" ]\n'
+         '    else\n'
+         '        if [ -z "$4" ]\n'
          '        then\n'
          f'            cmd="lc2SDS_weak $lchfiles -d \\"$STATION_DIR\\" -i \\"{fixed_dir}\\" -o \\"{output_dir}\\" --network \\"{network_code}\\" --station \\"$1\\" --obs_type \\"$2\\" --start_times \\"$3\\" --end_times \\"$5\\" \\"$6\\" --leapsecond_times \\"$7\\" --leapsecond_types \\"$8\\""\n'
          '        else\n'
          f'            cmd="lc2SDS_weak $lchfiles -d \\"$STATION_DIR\\" -i \\"{fixed_dir}\\" -o \\"{output_dir}\\" --network \\"{network_code}\\" --station \\"$1\\" --obs_type \\"$2\\" --start_times \\"$3\\" \\"$4\\" --end_times \\"$5\\" \\"$6\\" --leapsecond_times \\"$7\\" --leapsecond_types \\"$8\\""\n'
          '        fi\n'
          '    fi\n'
          '    echo "Running: $cmd"\n'
@@ -107,22 +100,21 @@
          '    echo "------------------------------------------------------------"\n'
          '    echo "Removing intermediate files"\n'
          f'    command rm -r $STATION_DIR/{fixed_dir}\n'
          '}\n\n')
     return s
 
 
-def _run_station_call(station, no_drift_correct):
+def _run_station_call(station):
 
     """
     Write a call to the run_station() function
 
     Args:
         station (:class:`.Station`): station information
-        no_drift_correct (bool): do NOT drift correct
     Returns:
         s (str): single-line call
     """
     station_code = station.label
     obs_type = _get_ref_code(station.instrumentation)
     leaptimes, leaptypes = [], []
     ccld = None
@@ -146,18 +138,15 @@
         end_sync_ref = ccld["end_sync_reference"]
         end_sync_inst = ccld["end_sync_instrument"]
     if leaptimes:
         raise ValueError("the network file provides leapseconds: run_station can't (yet) handle that")
         leaptimes_str = " ".join(leaptimes)
         leaptypes_str = " ".join(leaptypes)
     s = f'run_station "{station_code}" "{obs_type}" '
-    if no_drift_correct is True:
-        s += '"" "" "" "" '
-    else:
-        s += f'"{start_sync_ref}" "{start_sync_inst}" "{end_sync_ref}" "{end_sync_inst}" '
+    s += f'"{start_sync_ref}" "{start_sync_inst}" "{end_sync_ref}" "{end_sync_inst}" '
     s += f'"{leaptimes_str}" "{leaptypes_str}"\n'
 
     return s
 
 
 def _console_script(argv=None):
     """
@@ -184,16 +173,14 @@
                              "(default: %(default)s)")
     # parser.add_argument("--append", action="store_true",
     #                     help="append to existing script file")
     parser.add_argument("-v", "--verbose", action="store_true",
                         help="increase output verbosity")
     parser.add_argument("--no_header", action="store_true",
                         help="do not include a script header")
-    parser.add_argument("--no_drift_correct", action="store_true",
-                        help="do not correct for instrument drift")
     parser.add_argument("-q", "--quiet", action="store_true",
                         help="run silently")
     args = parser.parse_args()
 
     if not args.quiet:
         print("Creating LC2SDS_weak process script, ", end="", flush=True)
 
@@ -217,16 +204,15 @@
 
     # scripts = []
     # first_time = True
     script = process_script(subnetwork.fdsn_code,
                             subnetwork.stations,
                             args.station_data_path,
                             input_dir=args.input_dir,
-                            output_dir=args.output_dir,
-                            no_drift_correct=args.no_drift_correct)
+                            output_dir=args.output_dir)
     if not args.quiet:
         print(', '.join([s.label for s in subnetwork.stations]))
     fname = "process" + args.suffix + ".sh"
     if args.verbose:
         print(f" ... writing file {fname}", flush=True)
     with open(fname, 'w') as f:
         f.write(script)
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/addons/LCHEAPO.py` & `obsinfo-0.111b1/obsinfo/addons/LCHEAPO.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Write extraction script for LCHEAPO instruments (proprietary to miniseed)
 """
 # import obsinfo
 from obsinfo.subnetwork import Subnetwork
 from ..misc.discoveryfiles import (Datapath)
-from ..obsmetadata import (ObsMetadata)
+from ..obsMetadata.obsmetadata import (ObsMetadata)
 from pathlib import Path
 import os.path
 
 SEPARATOR_LINE = "\n# " + 60 * "=" + "\n"
 
 
 def process_script(network_code,
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/addons/OCA.py` & `obsinfo-0.111b1/obsinfo/addons/OCA.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/addons/SDPCHAIN.py` & `obsinfo-0.111b1/obsinfo/addons/SDPCHAIN.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/addons/infodump.py` & `obsinfo-0.111b1/obsinfo/addons/infodump.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/console_scripts/_test.py` & `obsinfo-0.111b1/obsinfo/console_scripts/_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,33 +62,31 @@
 from logging.handlers import RotatingFileHandler
 
 # Third party  imports
 from obspy.core.utcdatetime import UTCDateTime
 from obspy.core.inventory.util import Site
 
 # obsinfo modules
-from ..obsmetadata import (ObsMetadata)
-from ..instrumentation import (Instrumentation, InstrumentComponent,
-                               Stages, Stage, Location)
-from ..network import (Station, Subnetwork)
-from ..instrumentation.filter import (Filter, PolesZeros, FIR,
-                                      Coefficients, ResponseList)
-from ..misc.printobs import PrintObs
-from ..misc.discoveryfiles import Datapath
+from obsinfo.obsMetadata.obsmetadata import (ObsMetadata)
+from obsinfo.instrumentation import (Instrumentation, InstrumentComponent,
+                                     Stages, Stage, Location)
+from obsinfo.network import (Station, Subnetwork)
+from obsinfo.instrumentation.filter import (Filter, PolesZeros, FIR,
+                                            Coefficients, ResponseList)
+from obsinfo.misc.printobs import PrintObs
+from obsinfo.misc.discoveryfiles import Datapath
 # import obsinfo
-from ..misc.const import (EXIT_SUCCESS, EXIT_FAILURE, EXIT_NOINPUT,
-                          EXIT_SOFTWARE, EXIT_DATAERR, EXIT_UNAVAILABLE)
-from ..helpers import init_logging
+from obsinfo.misc.const import (EXIT_SUCCESS, EXIT_FAILURE, EXIT_NOINPUT,
+                                EXIT_SOFTWARE, EXIT_DATAERR, EXIT_UNAVAILABLE)
+# from obsinfo.misc.configuration import Singleton
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 verbose = False
 
-logger = init_logging("test")
-
 
 class JsonRefTest(unittest.TestCase):
     """
     Class of test methods for information file format
 
     Attributes:
         testing_path (str): path to datafiles to be tested aside from the examples
@@ -1316,14 +1314,15 @@
 
     """
 
     args = retrieve_arguments()
     tst = TestObsinfo()
     tst.setUp(test=False, print_output=True, level=args.level)
     # dp = Datapath()
+    logger = init_logging()
 
     try:
 
         type = ObsMetadata.get_information_file_type(args.input_filename)
 
         print(f'Printing {type} file: {args.input_filename}')
 
@@ -1339,16 +1338,14 @@
             tst._test_sensor(tst.infofiles_path.build_datapath(args.input_filename))
         elif type == "instrumentation":
             tst._test_instrumentation(tst.infofiles_path.build_datapath(args.input_filename))
         elif type == "station":
             tst._test_station(tst.infofiles_path.build_datapath(args.input_filename))
         elif type == "network":
             tst._test_network(tst.infofiles_path.build_datapath(args.input_filename))
-        else:
-            logger.warning(f'Could not find type of {args.input_filename}')
 
     except TypeError:
         print("Illegal format: fields may be missing or with wrong format in input file, or there is a programming error")
         logger.error("TypeError: Illegal format: fields may be missing or with wrong format in input file, or there is a programming error")
         if args.debug:
             raise
         sys.exit(EXIT_DATAERR)
@@ -1424,7 +1421,28 @@
 
     args = parser_args.parse_args()
 
     if not Path(args.input_filename[0]).is_absolute():
         args.input_filename = str(Path(os.getcwd()).joinpath(args.input_filename[0]).resolve())
 
     return args
+
+
+def init_logging():
+    """
+    Create or open a rotating logging file and add it to ObsinfoConfiguration
+
+    :returns: object of Logger class
+    """
+    logfile = Path.home().joinpath('.obsinfo', 'obsinfolog-validate')
+
+    logger = logging.getLogger("obsinfo")
+
+    logger.setLevel(logging.DEBUG)
+    # add a rotating handler with 200K (approx) files and just two files
+    handler = RotatingFileHandler(logfile, maxBytes=200000,
+                                  backupCount=2)
+    frmt = logging.Formatter(fmt='%(asctime)s %(levelname)-8s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+    handler.setFormatter(frmt)
+    logger.addHandler(handler)
+
+    return logger
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/console_scripts/makeStationXML.py` & `obsinfo-0.111b1/obsinfo/console_scripts/makeStationXML.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,34 +8,37 @@
 # General library imports
 import sys
 import os
 # import re
 import warnings
 
 from pathlib import Path  # , PurePath
+# from json.decoder import JSONDecodeError
+import logging
+from logging.handlers import RotatingFileHandler
 
 from argparse import ArgumentParser
 
 # Third party imports
 # import obspy
 from obspy.core.inventory import Inventory  # , Station, Channel, Site
 from obspy.core.inventory import Network
 # from obspy.clients.nrl import NRL
 
 # obsinfo imports
 from ..subnetwork import (Subnetwork)
-from ..obsmetadata import (ObsMetadata)
+from ..obsMetadata.obsmetadata import (ObsMetadata)
 from ..misc.discoveryfiles import (Datapath)
 from .print_version import main as print_version
+import obsinfo
 from ..misc.const import EXIT_USAGE, EXIT_SUCCESS
-from ..helpers import init_logging
+# from ..misc.configuration import ObsinfoConfiguration
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
-logger = init_logging("makeStationXML")
 
 
 def main(argv=None, dp=None):
     """
     Entry point for obsinfo-makeStationXML.
 
      1) Setups status variables from command line arguments.
@@ -53,14 +56,15 @@
             If None, will use values specified in .obsinforc
     """
 
     # create list of directories to search for files
     if dp is None:
         dp = Datapath()
     args = retrieve_arguments(argv, dp)
+    logger = init_logging()
 
     if args.verbose:
         print(f'Using OBSINFO_DATAPATH: {dp.datapath_list}')
 
     logger.info(f'Using OBSINFO_DATAPATH: {dp.datapath_list}')
 
     _make_StationXML(logger, args, dp)
@@ -175,24 +179,46 @@
         args = parser_args.parse_args()
 
     if args.version:
         print_version()
         sys.exit(EXIT_SUCCESS)
 
     # schemas must always be installed under obsinfo/data/schemas
-    args.schemapath = Path(__file__).parent.joinpath('data', 'schemas')
+    args.schemapath = Path(obsinfo.__file__).parent.joinpath('data', 'schemas')
 
     if not args.input_filename:
         print("No input filename specified")
         sys.exit(EXIT_USAGE)
 
     input_filename = args.input_filename[0]
 
     args.input_filename = str(datapath.build_datapath(input_filename)
                               if args.remote
                               else Path(os.getcwd()).joinpath(input_filename))
 
     return args
 
 
+def init_logging():
+    """
+    Create or open a rotating logging file and add it to ObsinfoConfiguration
+
+    :returns: object of Logger class
+    """
+
+    logfile = Path.home().joinpath('.obsinfo', 'obsinfolog-makeStationXML')
+
+    logger = logging.getLogger("obsinfo")
+
+    logger.setLevel(logging.DEBUG)
+    # add a rotating handler with 200K (approx) files and just two files
+    handler = RotatingFileHandler(logfile, maxBytes=200000,
+                                  backupCount=2)
+    frmt = logging.Formatter(fmt='%(asctime)s %(levelname)-8s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+    handler.setFormatter(frmt)
+    logger.addHandler(handler)
+
+    return logger
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/console_scripts/print.py` & `obsinfo-0.111b1/obsinfo/console_scripts/print.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 Application to print obsinfo information files.
 """
 import os
 import warnings
 from pathlib import Path
 from argparse import ArgumentParser
 
+import logging
+from logging.handlers import RotatingFileHandler
+
 # obsinfo modules
-from ..obsmetadata import ObsMetadata
-from ..instrumentation import (Instrumentation, Stage, Filter,
+import obsinfo
+from obsinfo.obsMetadata.obsmetadata import ObsMetadata
+from obsinfo.instrumentation import (Instrumentation, Stage, Filter,
                                      Preamplifier, Sensor, Datalogger)
-from ..helpers import Location, Locations, Person, init_logging
-from ..subnetwork import (Subnetwork, Network, Operator)
-from ..misc.discoveryfiles import Datapath
+from obsinfo.helpers import Location, Locations, Person
+from obsinfo.subnetwork import (Subnetwork, Operator)
+from obsinfo.misc.discoveryfiles import Datapath
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 verbose = False
 
-logger = init_logging("print", console_level='WARNING')
-
 
 def print_single_file(info_file, n_sublevels=0, configs=False, verbose=True):
     """
     Print a single obsinfo file.
 
     Args:
         info_file (str): info file to validate.
@@ -40,16 +42,14 @@
         print(str(e))
         return False
     if configs is not True:
         print(f'{Path(info_file).name}: ', end='', flush=True)
         no_class_msg = f"Can't print {filetype} files (no associated class)"
         if filetype == 'subnetwork':
             obj = Subnetwork(attributes_dict[filetype])
-        elif filetype == 'network':
-            obj = Network(attributes_dict[filetype])
         elif filetype == 'instrumentation_base':
             location_code='00'
             locations = Locations(
                 [Location({'position': {'lat': 0, 'lon': 0, 'elev': 0},
                            'base': {'uncertainties.m': {'lat': 0, 'lon': 0, 'elev':0},
                                     'depth.m': 0,
                                     'geology': 'seafloor',
@@ -62,33 +62,31 @@
         elif filetype == 'datalogger_base':
             obj = Datalogger({'base': attributes_dict[filetype]})
         elif filetype == 'sensor_base':
             obj = Sensor({'base': attributes_dict[filetype]})
         elif filetype == 'preamplifier_base':
             obj = Preamplifier({'base': attributes_dict[filetype]})
         elif filetype == 'location_base':
-            obj = Location({'base': attributes_dict[filetype],
-                             'position': {'lat': 0, 'lon': 0, 'elev': 0}})
+            obj = Location({'base': attributes_dict[filetype]})
         elif filetype == 'stage_base':
             obj = Stage({'base': attributes_dict[filetype]})
         elif filetype == 'network':
             print(no_class_msg)
             return
         elif filetype == 'operator':
             obj = Operator(attributes_dict[filetype])
         elif filetype == 'filter':
-            obj = Filter.construct(attributes_dict[filetype], 1, 'print')
+            obj = Filter.construct(attributes_dict[filetype])
         elif filetype == 'person':
             obj = Person(attributes_dict[filetype])
         elif filetype == 'timing_base':
             print(no_class_msg)
             return
         else:
             print(f"Unknown information file type: '{filetype}")
-            return
         print("\n    " + obj.__str__(indent=4, n_subclasses=n_sublevels))
     else:
         if filetype in ('instrumentation_base', 'datalogger_base',
                         'sensor_base' 'preamplifier_base',
                         'location_base', 'stage_base', 'timing_base'):
             configs = attributes_dict[filetype].get('configurations', {})
             keys = list(configs.keys())
@@ -98,15 +96,15 @@
         else:
             if verbose:
                 print(f'{Path(info_file).name}: ', end='', flush=True)
                 print(f"file type: '{filetype}' has no configurations")
             return
 
 
-def print_directory(info_dir, n_sublevels=1, configs=False,
+def print_directory(info_dir, n_sublevels=False, configs=False,
                     drilldown=False, verbose=False):
     """
     Validate all information files in a directory.
 
     Args:
         info_dir (:class:`Path`): directory where files reside
         drilldown (bool): drill down through subdirectories
@@ -186,17 +184,40 @@
                              "--n_sublevels=0)")
 
     args = parser.parse_args()
 
     if args.input == 'DATAPATH':
         args.input = Datapath().datapath_list[0]
         args.drilldown = True
+        args.n_levels = 0
         print('Validating first DATAPATH dir')
     args.input = Path(args.input)
     if not args.input.is_absolute():
         args.input = Path(os.getcwd()).joinpath(args.input).resolve()
 
     return args
 
 
+def init_logging():
+    """
+    Create or open a rotating logging file and add it to ObsinfoConfiguration
+
+    :returns: object of Logger class
+    """
+    logfile = Path.home().joinpath('.obsinfo', 'obsinfolog-validate')
+
+    logger = logging.getLogger("obsinfo")
+
+    logger.setLevel(logging.DEBUG)
+    # add a rotating handler with 200K (approx) files and just two files
+    handler = RotatingFileHandler(logfile, maxBytes=200000,
+                                  backupCount=2)
+    frmt = logging.Formatter(fmt='%(asctime)s %(levelname)-8s %(message)s',
+                             datefmt='%Y-%m-%d %H:%M:%S')
+    handler.setFormatter(frmt)
+    logger.addHandler(handler)
+
+    return logger
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/console_scripts/setup.py` & `obsinfo-0.111b1/obsinfo/console_scripts/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,34 +6,33 @@
 # import sys
 import re
 # import site
 import shutil
 import datetime
 import platform
 from pathlib import Path
+# import logging
 import warnings
 
 from argparse import ArgumentParser
 
+import obsinfo
 from ..misc.const import EXIT_IOERR
-from ..version import __version__
-from ..helpers import init_logging
-
-logger = init_logging("setup")
+from obsinfo.version import __version__
 
 
 def main():
     """
     Entry point to configure variables in file .obsinforc
 
     and to copy examples and templates out of the distribution directories
     """
     # initialize variables
     version = platform.python_version()
-    path_to_package = Path(__file__).parent.parent
+    path_to_package = Path(obsinfo.__file__).parent
     examples_dir = path_to_package.joinpath("_examples/Information_Files")
     templates_dir = path_to_package.joinpath("templates")
     home = Path.home()
     configuration_file = home.joinpath('.obsinforc')
 
     args = retrieve_arguments()
 
@@ -54,17 +53,16 @@
                 os.rename(dest, new_dest)
 
             shutil.copytree(examples_dir, dest.joinpath("Information_Files"))
             shutil.copytree(templates_dir, dest.joinpath("templates"))
         except NotADirectoryError:
             print("Directory not found")
             exit(EXIT_IOERR)
-        except OSError as e:
+        except OSError:
             print("Operating system error")
-            print(e)
             exit(EXIT_IOERR)
     # create configuration file
     output = []
 
     output.append("gitlab_repository: " + args.gitlab + "\n")
     output.append("gitlab_project: " + args.project + "\n")
     output.append("gitlab_path: " + args.remote_path + "\n")
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/console_scripts/validate.py` & `obsinfo-0.111b1/obsinfo/console_scripts/validate.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 """
 import os
 from pathlib import Path
 import glob
 import re
 import sys
 from argparse import ArgumentParser
+import logging
+from logging.handlers import RotatingFileHandler
 
-from ..misc.discoveryfiles import Datapath
-from ..obsmetadata import ObsMetadata
-from ..misc.const import EXIT_SUCCESS
-from ..helpers import init_logging
+from obsinfo.misc.discoveryfiles import Datapath
+import obsinfo
+from obsinfo.obsMetadata.obsmetadata import ObsMetadata
+from obsinfo.misc.const import EXIT_SUCCESS
 
-logger = init_logging("validate")
 
 class ValidateObsinfo():
     """
     Methods to validate each level of information files.
 
     Attributes:
         datapath (:class:`/.Datapath`): Store datapath list(s)
@@ -44,15 +45,15 @@
             debug (bool): Print more detailed messages and enable traceback
                 of exceptions
         Returns: self
         """
         dp = Datapath()
         self.datapath = dp
         self.datapath.infofiles_path = dp.datapath_list
-        self.datapath.validate_path = Path(__file__).parent.parent.joinpath('data', 'schemas')
+        self.datapath.validate_path = Path(obsinfo.__file__).parent.joinpath('data', 'schemas')
 
         self.verbose = verbose
         self.remote = remote
         self.debug = debug
 
         return self
 
@@ -67,15 +68,15 @@
             filetype (str): the information file type
             file_format (str): the information file format ('json' or 'yaml')
             check_schema (bool): validate schema file as well
         Returns:
             (bool): True if validated, False if not
         """
         if file_format not in ('json', 'yaml'):
-            logger.error('file_format ("{file_format}") not in ("json", "yaml")')
+            logging.error('file_format ("{file_format}") not in ("json", "yaml")')
             raise ValueError('file_format ("{file_format}") not in ("json", "yaml")')
         try:
             ret = ObsMetadata().validate(info_file,
                                          self.datapath.validate_path,
                                          self.remote,
                                          file_format,
                                          filetype,
@@ -100,15 +101,15 @@
             forced_filetype (str): file type.  If None, determine it.
             drilldown (bool): drill down through directories beneath the specified one
             continue_on_fail (bool): continue testing if a validation fails
             check_schema (bool): check schema on first use
         Returns:
             false if any file failed
         """
-        suffixes = ['.yaml', '.json']
+        suffixes = ['.yaml', '.yml']
         checked_schemas = []
         if not dir.is_dir():
             raise ValueError(f'"{dir}" is not a directory!')
         if drilldown is True:
             print(f'Validating files in and below directory {dir}')
             if forced_filetype is not None:
                 raise ValueError('Cannot specify filetype when drilling down '
@@ -126,16 +127,17 @@
         results = {'passed': 0, 'failed': 0, 'skipped': 0}
         for file in files:
             if file.suffix.lower() not in suffixes:
                 print(f'Skipping {str(file.relative_to(dir))}')
                 results['skipped'] += 1
                 continue
             if forced_filetype==None:
-                filetype = ObsMetadata.get_information_file_type(str(file))
-                if filetype is None:
+                try:
+                    filetype = ObsMetadata.get_information_file_type(str(file))
+                except Exception:
                     print(f"Could not find a schema for {str(file.relative_to(dir))}, skipping...")
                     results['skipped'] += 1
                     continue
             print(f"Validating {str(file.relative_to(dir))} against "
                   f"{filetype}.schema.json ... ", end='', flush=True)
             if check_schema is True:
                 if filetype in checked_schemas: 
@@ -269,14 +271,15 @@
     Entry point for obsinfo-validate.
 
      1) Sets up status variables from command line arguments.
      2) Validates file according to file type contained in name
      3) Manages all uncaught exceptions
     """
     args = retrieve_arguments()
+    # logger = init_logging()
 
     val = ValidateObsinfo()
     val.setUp(verbose=args.verbose, remote=args.remote, debug=args.debug)
 
     filetype = None
     if args.schema:
         if ObsMetadata.is_valid_type(args.schema):
@@ -294,14 +297,72 @@
     elif args.input.is_dir():
         if args.schema and args.drilldown:
             raise ValueError("Cannot specify schema for a drill-down "
                              "directory validation")
         val.validate_directory(args.input, filetype, args.drilldown,
                                args.continue_on_fail, check_schema=args.check_schema)
 
+#     try:
+#         val.validate_single_file(input_filename, filetype)
+#     except TypeError as e:
+#         print("TypeError:" + str(e))
+#         logger.error("TypeError: Illegal format: fields may be missing or "
+#                      "with wrong format in input file, or there is a "
+#                      "programming error")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_DATAERR)
+#     except (KeyError, IndexError) as e:
+#         print("Illegal value in dictionary key or list index:" + str(e))
+#         logger.error("KeyError, IndexError: Illegal value in dictionary key "
+#                      "or list index")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_SOFTWARE)
+#     except ValueError as e:
+#         print("ValueError:" + str(e))
+#         logger.error("ValueError: An illegal value was detected")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_DATAERR)
+#     except FileNotFoundError as e:
+#         if args.debug:
+#             raise
+#         print("File not found:" + str(e))
+#         logger.error(f"FileNotFoundError: {str(e)}")
+#         sys.exit(EXIT_NOINPUT)
+#     except JSONDecodeError as e:
+#         print("JSONDecodeError:" + str(e))
+#         logger.error("JSONDecodeError: File and/or subfiles have an illegal "
+#                      "format. Probably indentation or missing "
+#                      "quotes/parentheses/brackets")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_DATAERR)
+#     except (IOError, OSError, LookupError) as e:
+#         print("File could not be opened or read:" + str(e))
+#         logger.error("IOError, OSError, LookupError: File could not be "
+#                      "opened or read")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_UNAVAILABLE)
+#     except AttributeError as e:
+#         print("Attribute error: " + str(e))
+#         logger.debug("AttributeError: Programming error: an object in code "
+#                      "had a wrong attribute")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_SOFTWARE)
+#     except:
+#         print("General exception")
+#         logger.debug("General exception:")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_FAILURE)
+#
     sys.exit(EXIT_SUCCESS)
 
 
 def retrieve_arguments():
     """
     Retrieve command line arguments.
 
@@ -357,9 +418,31 @@
     args.input = Path(args.input)
     if not args.input.is_absolute():
         args.input = Path(os.getcwd()).joinpath(args.input).resolve()
 
     return args
 
 
+def init_logging():
+    """
+    Create or open a rotating logging file and add it to ObsinfoConfiguration
+
+    :returns: object of Logger class
+    """
+    logfile = Path.home().joinpath('.obsinfo', 'obsinfolog-validate')
+
+    logger = logging.getLogger("obsinfo")
+
+    logger.setLevel(logging.DEBUG)
+    # add a rotating handler with 200K (approx) files and just two files
+    handler = RotatingFileHandler(logfile, maxBytes=200000,
+                                  backupCount=2)
+    frmt = logging.Formatter(fmt='%(asctime)s %(levelname)-8s %(message)s',
+                             datefmt='%Y-%m-%d %H:%M:%S')
+    handler.setFormatter(frmt)
+    logger.addHandler(handler)
+
+    return logger
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/helpers/__init__.py` & `obsinfo-0.111b1/obsinfo/helpers/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 Helper classes, used by other classes
 """
-# noqa: F401 disables flake8 warning that imported modules are unused
 from .float_with_uncert import FloatWithUncert        # noqa: F401
 from .location import Location, Locations             # noqa: F401
-from .oi_date import OIDate, OIDates                  # noqa: F401
+from .oi_date import OIDate                           # noqa: F401
 from .comments import Comments                        # noqa: F401
 from .obsinfo_class_list import ObsinfoClassList      # noqa: F401
-from .functions import (str_indent, str_list_str, verify_dict_is_empty) # noqa: F401
+from .functions import (str_indent, str_list_str, verify_dict_is_empty)        # noqa: F401
 from .person import Person, Persons                   # noqa: F401
 from .phone import Phone, Phones                      # noqa: F401
 from .external_references import ExternalReferences   # noqa: F401
-from .identifiers import Identifiers                  # noqa: F401
-from .logger import init_logging                      # noqa: F401
+from .identifiers import Identifiers      # noqa: F401
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/helpers/comments.py` & `obsinfo-0.111b1/obsinfo/helpers/comments.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/helpers/external_references.py` & `obsinfo-0.111b1/obsinfo/helpers/external_references.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             Args:
                 attributes_list: (list of dict or str): list
                     of external references read from YAML/JSON file
         """
         if attributes_list is None:
             super().__init__([], ExternalReference)
         else:
-            super().__init__(attributes_list, ExternalReference)
+            super().__init__([ExternalReference(x) for x in attributes_list])
 
 
 class ExternalReference(object):
     def __init__(self, attributes_dict):
         self.uri = attributes_dict.pop('uri')
         self.description = attributes_dict.pop('description')
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/helpers/float_with_uncert.py` & `obsinfo-0.111b1/obsinfo/helpers/float_with_uncert.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/helpers/functions.py` & `obsinfo-0.111b1/obsinfo/helpers/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from textwrap import indent
 import inspect
-import logging
-
-logger = logging.getLogger("obsinfo")
 
 def str_indent(s, nchars: int):
     """
     Indents all lines of a string by a given # of spaces
 
     Normally indents all but the first line, if nchars is negative then indents
     all lines including the first, by -nchars
@@ -32,28 +29,25 @@
         indent (int):  # of characters to indent by
         n_subclasses (int): if < 0, return a one-line string
     """
     if slist is None:
         return 'None'
 
     if n_subclasses < 0:
-        if len(slist) == 0:
-            return '[]'
-        elif len(slist) == 1:
-            return f'["{slist[0]}"]'
-        return f'List of {len(slist)} strings'
+        return f'{len(slist)} strings'
+    
     s = 'List of strings:'
     for x in slist:
         s += f'\n- {x}'
     return str_indent(s, indent)
 
 
 def verify_dict_is_empty(attributes_dict):
     if len(attributes_dict) == 0:
         return
     stack = inspect.stack()
     the_class = stack[1][0].f_locals["self"].__class__.__name__
     the_method = stack[1][0].f_code.co_name
-    logger.error(f'attributes dict in {the_class}.{the_method} has '
+    raise ValueError(f'attributes dict in {the_class}.{the_method} has '
                      f'leftover keys: {list(attributes_dict.keys())}')
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/helpers/identifiers.py` & `obsinfo-0.111b1/obsinfo/helpers/identifiers.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             Args:
                 attributes_list: (list of dict or str): list
                     of external references read from YAML/JSON file
         """
         if attributes_list is None:
             super().__init__([], Identifier)
         else:
-            super().__init__(attributes_list, Identifier)
+            super().__init__([Identifier(x) for x in attributes_list])
 
 
 class Identifier(object):
     """
     A type to document persistent identifiers. Must provide a scheme (prefix)
     """
     def __init__(self, uri):
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/helpers/location.py` & `obsinfo-0.111b1/obsinfo/helpers/location.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 # Standard library modules
 import warnings
 import numpy as np
 import logging
 
 from .float_with_uncert import FloatWithUncert
-from ..obsmetadata import ObsMetadata
+from ..obsMetadata import ObsMetadata
 from .functions import str_indent
 from .obsinfo_class_list import ObsinfoClassList
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
@@ -66,22 +66,22 @@
         if code is not None:
             if 'code' in attributes_dict:
                 raise ValueError('provided location code as argument AND dict key')
             else:
                 attributes_dict['code'] = code
 
         position = attributes_dict.pop('position', None)
-        if position is None:
+        if not position:
             msg = 'No position in location'
             warnings.warn(msg)
             logger.error(msg)
             raise TypeError(msg)
-        self._lat = position.pop('lat')
-        self._lon = position.pop('lon')
-        self._elev = position.pop('elev')
+        self._lat = position.get('lat', None)
+        self._lon = position.get('lon', None)
+        self._elev = position.get('elev', None)
         self._position = position  # for __repr__()
         self.code = attributes_dict.pop('code', None)
 
         # Get base-config elements
         base_dict = attributes_dict.get_configured_modified_base()
         self.geology = base_dict.get('geology', None)
         self.vault = base_dict.get('vault', None)
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/helpers/obsinfo_class_list.py` & `obsinfo-0.111b1/obsinfo/helpers/obsinfo_class_list.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,57 +13,70 @@
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class ObsinfoClassList(list):
-    def __init__(self, seq, element_class):
+    def __init__(self, seq, element_class=None):
         """
         Args:
             seq (list or None): sequence of dicts or of :class:element_class.
                 If dicts, converts to element_class type using element_class()
                 If None, return empty instance
             element_class (:class:): the class that every element should be
                 (or become)
         """
         if seq is not None and not isinstance(seq, list):
             raise TypeError(f'seq ({type(seq)}) is neither a list nor None')
         # Validate element_class
-        if not inspect.isclass(element_class):
-            raise TypeError('element_class is not a class')
-        self.element_class = element_class
-        
+        if element_class is None:
+            if seq is None:
+                raise ValueError('You did not provide an element_class to '
+                                 'instantiate the empty input seq')            
+            elif len(seq) == 0:
+                raise ValueError('You did not provide an element_class to '
+                                 'instantiate the empty input seq')            
+            elif isinstance(seq[0], dict):        
+                raise ValueError('You did not provide an element_class to '
+                                 'translate the dicts in the input sequence')
+        else:
+            if not inspect.isclass(element_class):
+                raise TypeError('element_class is not a class')
+
         if seq is None:
             super().__init__([])
+            self.element_class = element_class
             return
         elif len(seq) == 0:
             super().__init__([])
+            self.element_class = element_class
             return
         
         # Verify all elements are of same type
         for x in seq:
             if not isinstance(x, type(seq[0])):
                 raise TypeError(f'seq elements are not all of same type '
                                 f'({type(x)} != {type(seq[0])})')
 
-        if not isinstance (seq[0], element_class):
+        if isinstance (seq[0], dict):
             seq = [element_class(x) for x in seq]
 
         super().__init__(x for x in seq)
-
+        self.element_class = self[0].__class__
+        
     def append(self, item):
         if not isinstance(item, self.element_class):
             item = element_class(item)
         super().append(item)
 
     def __str__(self, indent=0, n_subclasses=0):
         s = f'{self.__class__.__name__}:'
         if len(self) == 0:
-            return s + ' []'
+            return s + ' Empty'
         elif len(self) == 1:
             return s + f' [{self[0].__str__(4, n_subclasses-1)}]'
         if n_subclasses < 0:
             return s + f' {len(self)} {self.element_class}s'
         for x in self:
             s += f'\n    - {x.__str__(indent=8, n_subclasses=n_subclasses-1)}'
         return str_indent(s, indent)
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/helpers/person.py` & `obsinfo-0.111b1/obsinfo/helpers/person.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/helpers/phone.py` & `obsinfo-0.111b1/obsinfo/helpers/phone.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/__init__.py` & `obsinfo-0.111b1/obsinfo/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/channel.py` & `obsinfo-0.111b1/obsinfo/instrumentation/channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 
 # Non-standard modules
 from obspy.core.inventory.channel import Channel as obspy_Channel
 from obspy.core.inventory.util import Comment
 
 # obsinfo modules
-from ..obsmetadata import ObsMetadata
+from ..obsMetadata import ObsMetadata
 from ..helpers import (Location, OIDate, str_indent, verify_dict_is_empty,
                        Comments, ExternalReferences, Identifiers, ObsinfoClassList)
 from .orientation import Orientation
 from .instrument import Instrument
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
@@ -63,16 +63,16 @@
             ic_modifs (dict or :class:`ObsMetadata`): modifications to pass
                 through to InstrumentComponents
             location (:class:`Location`): channel location
             equipment (:class:`Equipment`): channel equipment
         """
         # For __repr__
         self.input = {
-                      'attributes_dict':   {} if not attributes_dict else '<ObsMetaData>',
-                      'ic_modifs':   {} if not ic_modifs else '<ObsMetaData>',
+                      'attributes_dict':   {} if not attributes_dict else '<obsinfo.ObsMetaData>',
+                      'ic_modifs':   {} if not ic_modifs else '<obsinfo.ObsMetaData>',
                       'location': location,
                       'equipment': '<obsinfo.Equipment>'
                      }
 
         orientation = attributes_dict.pop('orientation', None)
         o_code = self._get_orientation_code(orientation)
         self.equipment = equipment
@@ -110,23 +110,21 @@
     def __str__(self, indent=0, n_subclasses=0):
         """
         Args:
             indent (int): number of extra characters to indent lines by
             n_subclasses (int): number of levels of subclass to print out
         """
         if n_subclasses < 0:
-            if self.location is not None:
-                return f'{self.__class__.__name__} {self.location.code}.{self.seed_code}'
-            else:
-                return f'{self.__class__.__name__} {self.seed_code}'
+            return self.__class__.__name__
 
         kwargs = {'indent': 4, 'n_subclasses': n_subclasses-1}
-        s = f'{self.__class__.__name__} {self.seed_code}:\n'
-        if self.location is not None:
-            s += f'    location: {self.location.__str__(**kwargs)}\n'
+        s = f'Channel {self.seed_code}:\n'
+        s += f'    location code: {self.location.code}\n'
+        # Force print of at least location.__str__() and orientation.__str__()
+        s += f'    location: {self.location.__str__(**kwargs)}\n'
         s += f'    orientation: {self.orientation.__str__(**kwargs)}\n'
         s += f'    start_date: {self.start_date}\n'
         s += f'    end_date: {self.end_date}\n'
         s += f'    equipment: {self.equipment.__str__(**kwargs)}\n'
         s += f'    comments: {self.comments}\n'
         s += f'    equipment: {self.instrument.__str__(**kwargs)}\n'
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/equipment.py` & `obsinfo-0.111b1/obsinfo/instrumentation/equipment.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import logging
 
 # Non-standard modules
 from obspy.core.inventory.util import Equipment as obspy_Equipment
 from obspy.core.utcdatetime import UTCDateTime
 
 # obsinfo
-from ..obsmetadata import ObsMetadata
-from ..helpers import OIDate, OIDates, str_indent, str_list_str
+from ..obsMetadata import ObsMetadata
+from ..helpers import OIDate, str_indent
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Equipment(obspy_Equipment):
@@ -55,17 +55,19 @@
         self.model = attributes_dict.get('model', None)
         self.manufacturer = attributes_dict.get('manufacturer', None)
         self.vendor = attributes_dict.get('vendor', None)
         self.serial_number = attributes_dict.get('serial_number', None)
         self.resource_id = attributes_dict.get('resource_id', None)
         self.installation_date = OIDate(attributes_dict.get('installation_date', None))
         self.removal_date = OIDate(attributes_dict.get('removal_date', None))
-        self.calibration_dates = OIDates(attributes_dict.get('calibration_dates', None))
-        # equip = self.to_obspy()
-        # self.obspy_equipment = equip[0] if isinstance(equip, tuple) else equip
+        calibration_dates = attributes_dict.get('calibration_dates', [])
+        self.calibration_dates = [OIDate(x) for x in calibration_dates]
+
+        equip = self.to_obspy()
+        self.obspy_equipment = equip[0] if isinstance(equip, tuple) else equip
 
     def __repr__(self):
         args = []
         if self.type:
             args.append(f"'type': '{self.type}'")
         if self.description:
             args.append(f"'description': '{self.description}'")
@@ -101,29 +103,31 @@
         if self.resource_id is not None:
             s += f"\n    resource_id: {self.resource_id}"
         if self.installation_date.date is not None:
             s += f"\n    installation_date: {self.installation_date}"
         if self.removal_date.date is not None:
             s += f"\n    removal_date: {self.removal_date}"
         if self.calibration_dates:
-            s += f"\n    calibration_dates: {self.calibration_dates.__str__(indent=4, n_subclasses=n_subclasses-1)}"
+            s += f"\n    calibration_dates: {self.calibration_dates}"
         return str_indent(s, indent)
 
     def to_obspy(self):
         """
         Convert an equipment (including the equipment description in
         components) to its obspy object
 
         Returns:
             (:class:`obspy.core.invertory.util.Equipment`)
         """
-        return obspy_Equipment(
+        equip = obspy_Equipment(
             type=self.type,
             description=self.description,
             manufacturer=self.manufacturer,
             vendor=self.vendor,
             model=self.model,
             serial_number=self.serial_number,
             installation_date=self.installation_date.to_obspy(),
             removal_date=self.removal_date.to_obspy(),
-            calibration_dates=self.calibration_dates.to_obspy(),
+            calibration_dates=[x.to_obspy() for x in self.calibration_dates],
             resource_id=self.resource_id)
+
+        return equip
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/AD_conversion.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/AD_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 Filter class and subclasses
 """
 # Standard library modules
+import warnings
 import logging
 
 from .coefficients import Coefficients
 from ...helpers import str_indent
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class ADConversion(Coefficients):
     """
     ADConversion Filter (Flat Coefficients filter)
 
@@ -25,15 +28,14 @@
         """
         Constructor
 
         Args:
             attributes_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         attributes_dict["transfer_function_type"] = 'DIGITAL'
         attributes_dict["numerator_coefficients"] = [1.0]
         attributes_dict["denominator_coefficients"] = []
         # Have to pop these before super, or it will give an error.
         input_full_scale = attributes_dict.pop('input_full_scale', None)
         output_full_scale = attributes_dict.pop('output_full_scale', None)
         super().__init__(attributes_dict, stage_id)
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/FIR.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/FIR.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 """
 Finite Impulse Response Filter
 """
 # Standard library modules
+import warnings
 import logging
 
 from .filter_template import FilterTemplate
 from ...helpers import str_indent
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class FIR(FilterTemplate):
     """
     FIR Filter
 
     Attributes:
         symmetry (str): filter symmetry, one of "EVEN", "ODD", "NONE"
         coefficients (list of floats)
         coefficient_divisor (float)
         delay_samples (float)
     """
-    def __init__(self, attributes_dict, stage_description):
+    def __init__(self, attributes_dict, stage_id=-1):
 
         """
         Constructor
 
         Args:
             attributes_dict (dict): information file
                 dictionaries for stages
-            stage_description (str): id + name of corresponding stage,
-                used for reporting only
+            stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         super().__init__(attributes_dict)
         self.symmetry = attributes_dict.pop('symmetry', None)
         self.coefficients = attributes_dict.pop('coefficients', [])
         self.coefficient_divisor = attributes_dict.pop('coefficient_divisor', 1)
         self._validate_empty_attributes_dict(attributes_dict)
-        self._validate_values(stage_description)
 
-    def _validate_values(self, stage_description):
         # Validate values
         if not self.delay_samples:
             msg = 'No delay.samples in FIR filter'
             logger.error(msg)
             raise TypeError(msg)
 
         if self.symmetry not in ['ODD', 'EVEN', 'NONE']:
             msg = f'Illegal FIR symmetry: "{self.symmetry} in stage #{stage_id}"'
             logger.error(msg)
-            raise TypeError(msg)
+            raise TypeError()
 
         sum_coeff = 0
         coeff_cnt = 0
         if len(self.coefficients) > 0:
             for coeff in self.coefficients:
                 sum_coeff += coeff
                 coeff_cnt += 1
@@ -62,17 +61,19 @@
                 coeff_cnt *= 2
             if self.symmetry == 'ODD':
                 sum_coeff += sum_coeff - self.coefficients[-1]
                 coeff_cnt += coeff_cnt - 1
             norm_coeff = sum_coeff / self.coefficient_divisor
             norm_coeff = round(norm_coeff, 2)  # check up to two decimal places
             # last conditional verifies that there is at least one coeff
-            if norm_coeff != 1:
-                logger.warning(f'Sum of {coeff_cnt} coefficients in stage '
-                               f'{stage_description} is {norm_coeff}, not 1 ')
+            if norm_coeff != 1 and norm_coeff != 0:
+                msg = (f'Sum of {coeff_cnt} coefficients in stage "{stage_id}" is '
+                       f'{norm_coeff}, not 1 ')
+                warnings.warn(msg)
+                logger.warning(msg)
 
     def __str__(self, indent=0, n_subclasses=0):
         if n_subclasses < 0:
             return f'{type(self)}'
         s = super().__str__() + '\n'
         s += f"    symmetry: {self.symmetry}\n"
         s += f"    coefficient_divisor: {self.coefficient_divisor}\n"
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/analog.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/analog.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 Analog Filter (subclass of PolesZeros)
 """
 # Standard library modules
+import warnings
 import logging
 
 from .poles_zeros import PolesZeros
 from ...helpers import str_indent
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Analog(PolesZeros):
     """
     Analog Filter (Flat PolesZeros filter)
     """
@@ -18,15 +21,14 @@
         """
         Constructor
 
         Args:
             attributes_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         attributes_dict["transfer_function_type"] = "LAPLACE (RADIANS/SECOND)"
         attributes_dict["poles"] = []
         attributes_dict["zeros"] = []
         if not "normalization_factor" in attributes_dict:
             attributes_dict["normalization_factor"] = 1.0
         # if not "normalization_frequency" in attributes_dict:
         #     attributes_dict["normalization_frequency"] = 1.
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/coefficients.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/coefficients.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Coefficients Filter
 """
+import warnings
 import logging
 
 from .filter_template import FilterTemplate
 from ...helpers import str_indent
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Coefficients(FilterTemplate):
     """
     Coefficients Filter Class
 
@@ -23,15 +26,14 @@
         """
         Constructor
 
         Args:
             attr_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         super().__init__(attr_dict, stage_id)
         self.transfer_function_type = attr_dict.pop('transfer_function_type',
                                                     'DIGITAL')
         self.numerator_coefficients = attr_dict.pop('numerator_coefficients',
                                                     [1.])
         self.denominator_coefficients = attr_dict.pop('denominator_coefficients', [])
         self._validate_empty_attributes_dict(attr_dict)
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/digital.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/digital.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 Digital filter (subclass of Coefficents, which is subclass of Filter)
 """
 # Standard library modules
+import warnings
 import logging
 
 from .coefficients import Coefficients
 from ...helpers import str_indent
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Digital(Coefficients):
     """
     Digital Filter (Flat Coefficients filter)
     """
@@ -18,15 +21,14 @@
         """
         Constructor
 
         Args:
             attributes_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         attributes_dict["transfer_function_type"] = 'DIGITAL'
         attributes_dict["numerator_coefficients"] = [1.0]
         attributes_dict["denominator_coefficients"] = []
         super().__init__(attributes_dict, stage_id)
         self._validate_empty_attributes_dict(attributes_dict)
 
     def __repr__(self):
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/filter.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/filter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,85 +1,81 @@
 """
 Filter class and subclasses
 """
 # Standard library modules
+import warnings
 import logging
 
 from .poles_zeros import PolesZeros
 from .analog import Analog
 from .digital import Digital
 from .AD_conversion import ADConversion
 from .FIR import FIR
 from .response_list import ResponseList
 from .coefficients import Coefficients
 from .polynomial import Polynomial
-from ...obsmetadata import ObsMetadata
+from ...obsMetadata import ObsMetadata
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Filter(object):
     """
     Filter is a gateway to the other filter classes
     """
     @staticmethod
-    def construct(attributes_dict, stage_sequence_number, stage_name,
+    def construct(attributes_dict, stage_id="-1",
                   sensitivity_gain_frequency=1.):
         """
         Constructs an appropriate Filter subclass from an attributes_dict
 
         Args:
             attributes_dict (dict or list of dicts): information file
                 dict for stages
-            stage_sequence_number (int): sequence_number of corresponding stage.
-            stage_name (str): name of corresponding stage. Used for reporting only
+            stage_id (int): id of corresponding stage. Used for reporting only
             sensitivity_gain_frequency (float): frequency at which gain was
                 specified.
                 Used for PoleZeros Normalization factor/frequency
         Returns:
             (:class:`.Filter`): object of the adequate filter subclass
         Raises:
             (TypeError): if filter type is not valid
         """
-        logger.debug('in Filter.construct()')
         if attributes_dict is None:
             msg = "No attributes in filter"
             logger.error(msg)
             raise TypeError(msg)
         if not isinstance(attributes_dict, ObsMetadata):
             attributes_dict = ObsMetadata(attributes_dict)
 
-        stage_description = f'#{stage_sequence_number}'
-        if stage_name is not None:
-                stage_description += f' ("{stage_name}")'
-
         if "type" not in attributes_dict:
-            msg = f'No "type" specified for filter in stage {stage_description}'
+            msg = f'No "type" specified for filter in stage #{stage_id}'
             logger.error(msg)
             raise TypeError(msg)
         else:
-            args = (attributes_dict, stage_description)
             filter_type = attributes_dict.get('type', None)
             if filter_type == 'PolesZeros':
                 attributes_dict['sensitivity_gain_frequency'] = sensitivity_gain_frequency
-                obj = PolesZeros(*args)
+                obj = PolesZeros(attributes_dict, stage_id)
             elif filter_type == 'FIR':
-                obj = FIR(*args)
+                obj = FIR(attributes_dict, stage_id)
             elif filter_type == 'Coefficients':
-                obj = Coefficients(*args)
+                obj = Coefficients(attributes_dict, stage_id)
             elif filter_type == 'ResponseList':
-                obj = ResponseList(*args)
+                obj = ResponseList(attributes_dict, stage_id)
             elif filter_type == 'ADCONVERSION':
-                obj = ADConversion(*args)
+                obj = ADConversion(attributes_dict, stage_id)
             elif filter_type == 'ANALOG':
                 attributes_dict['sensitivity_gain_frequency'] = sensitivity_gain_frequency
-                obj = Analog(*args)
+                obj = Analog(attributes_dict, stage_id)
             elif filter_type == 'DIGITAL':
-                obj = Digital(*args)
+                obj = Digital(attributes_dict, stage_id)
             elif filter_type == 'Polynomial':
-                obj = Polynomial(*args)
+                obj = Polynomial(attributes_dict, stage_id)
             else:
                 msg = (f'Unknown Filter type: "{filter_type}" in '
                        'stage #{stage_id}')
                 logger.error(msg)
                 raise TypeError(msg)
         return obj
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/filter_template.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/filter_template.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
 FilterTemplate class, used by all other filter classes
 """
 # Standard library modules
+import warnings
 import logging
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class FilterTemplate(object):
     """
     FilterTemplate is superclass of all filter classes
 
@@ -21,15 +24,14 @@
         """
         Constructor
 
         Args:
             attributes_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         self.delay_samples = attributes_dict.pop('delay.samples', None)
         self.delay_seconds = attributes_dict.pop('delay.seconds', None)
         self.resource_id = attributes_dict.pop('resource_id', None)
         self.stage_id = stage_id
         self.type = attributes_dict.pop('type', None)
 
     def _validate_empty_attributes_dict(self, attributes_dict):
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/poles_zeros.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/poles_zeros.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 """
 Filter class and subclasses
 """
 # Standard library modules
 import math as m
+import warnings
 import logging
 
 # Non-standard modules
+# import obspy.core.inventory.response as obspy_response
+# from scipy._lib.doccer import extend_notes_in_docstring
 from .filter_template import FilterTemplate
 from ...helpers import str_indent
 
+# from ..misc.configuration import ObsinfoConfiguration
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class PolesZeros(FilterTemplate):
     """
     PolesZeros filter
 
@@ -29,15 +35,14 @@
         """
         Constructor
 
         Args:
             attr_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         super().__init__(attr_dict, stage_id)
         self.transfer_function_type = attr_dict.pop(
             'transfer_function_type', 'LAPLACE (RADIANS/SECOND)')
         self.poles = [complex(x.replace(" ", ""))
                       for x in attr_dict.pop('poles', [])]
         self.zeros = [complex(x.replace(" ", ""))
                       for x in attr_dict.pop('zeros', [])]
@@ -71,16 +76,16 @@
             n_subclasses (int): number of levels of subclass to print out
         """
         if n_subclasses < 0:
             return f'{type(self)}'
         s = super().__str__() + '\n'
         s += f'    {len(self.poles)} poles, {len(self.zeros)} zeros\n'
         s += f'    transfer_function_type: {self.transfer_function_type}\n'
-        s += f'    normalization_frequency: {self.normalization_frequency:g}\n'
-        s += f'    normalization_factor: {self.normalization_factor:g}'
+        s += f'    normalization_frequency: {self.normalization_frequency:g}'
+        s += f'\n  normalization_factor: {self.normalization_factor:g}'
         return str_indent(s, indent)
 
     def calc_normalization_factor(self, stage_id=-1, debug=False):
         """
         Calculate the normalization factor for a given set of poles-zeros
 
         The norm factor A0 is calculated such that
@@ -105,20 +110,25 @@
 
         A0 = 1.0 + (1j * 0.0)
         if self.transfer_function_type == "LAPLACE (HERTZ)":
             s = 1j * self.normalization_frequency
         elif self.transfer_function_type == "LAPLACE (RADIANS/SECOND)":
             s = 1j * 2 * m.pi * self.normalization_frequency
         else:
-            logger.warning("Don't know how to calculate normalization factor"
-                           "for z-transform poles and zeros!")
+            msg = ("Don't know how to calculate normalization factor"
+                   "for z-transform poles and zeros!")
+            warnings.warn(msg)
+            logger.warning(msg)
             return None
 
         for p in self.poles:
             A0 *= (s - p)
         for z in self.zeros:
             A0 /= (s - z)
 
-        logger.debug(f"poles={self.poles}, zeros={self.zeros}, s={s}, A0={A0}")
+        if debug:
+            msg = f"poles={self.poles}, zeros={self.zeros}, s={s}, A0={A0}"
+            print(msg)
+            logger.debug(msg)
 
         A0 = abs(A0)
         return A0
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/polynomial.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/polynomial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Polynomial Filter
 """
+import warnings
 import logging
 
 from .filter_template import FilterTemplate
 from ...helpers import str_indent
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Polynomial(FilterTemplate):
     """
     Polynomial Filter Class (never tested)
     """
@@ -18,15 +21,14 @@
         """
         Constructor
 
         Args:
             attr_dict (dict or :class`ObsMetadata`): filter attributes
            stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         super().__init__(attr_dict, stage_id)
         self.frequency_lower_bound = attr_dict.pop('frequency_lower_bound', 0.)
         self.frequency_upper_bound = attr_dict.pop('frequency_upper_bound', 0.)
         self.approximation_lower_bound = attr_dict.pop('approximation_lower_bound', None)
         self.approximation_upper_bound = attr_dict.pop('approximation_upper_bound', None)
         self.maximum_error = attr_dict.pop('maximum_error', None)
         self.coefficients = attr_dict.pop('coefficients', [])
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/filter/response_list.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/response_list.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 """
 Filter class and subclasses
 """
+# Standard library modules
+import warnings
 import logging
 
+# Non-standard modules
+# import obspy.core.inventory.response as obspy_response
+# from scipy._lib.doccer import extend_notes_in_docstring
+
 from .filter_template import FilterTemplate
 from ...helpers import str_indent
 
+# from ..misc.configuration import ObsinfoConfiguration
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class ResponseList(FilterTemplate):
     """
     ResponseList Filter
 
@@ -22,15 +31,14 @@
         """
         Constructor
 
         Args:
             attributes_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         super().__init__(attributes_dict, stage_id)
         self.elements = attributes_dict.pop('elements', [])
         self._validate_empty_attributes_dict(attributes_dict)
 
         # Validate attributes
         for element in self.elements:
             if not len(element) == 3:
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/instrument.py` & `obsinfo-0.111b1/obsinfo/instrumentation/instrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         Args:
             attributes_dict (dict or :class:`.ObsMetadata`): instrument attributes_dict
             modifs (dict or :class:`ObsMetadata`): modifications passed
                 down from the Instrumentation level (including channel selection)
         """
         # For __repr__()
         if modifs:
-            self.inputs = {'modifs': "<ObsMetadata>"}
+            self.inputs = {'modifs': "<obsinfo.ObsMetadata>"}
         else:
             self.inputs = {'modifs': {}}
         
         self.correction = None
         self.delay = None
 
         if not attributes_dict:
@@ -78,15 +78,15 @@
         # # if self.stages is not None:
         # #     self.obspy_stages = [x.to_obspy() for x in self.stages]
         # # else:
         # #     self.obspy_stages = None
         # self.obspy_response = self.to_obspy()
 
     def __repr__(self):
-        s =   'Instrument(attributes_dict = <ObsMetadata>\n',
+        s =   'Instrument(attributes_dict = <obsinfo.ObsMetadata>\n',
         s += f'           modifs={self.inputs["modifs"]}'
         return s
 
     def __str__(self, indent=0, n_subclasses=0):
         if n_subclasses < 0:
             return self.__class__.__name__
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/instrument_component.py` & `obsinfo-0.111b1/obsinfo/instrumentation/instrument_component.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 InstrumentComponent class and subclasses Sensor, Preamplifier, Datalogger.
 Equipment class
 """
 # Standard library modules
+import warnings
 import logging
 
 # Non-standard modules
 
 # obsinfo
 from .stages import Stages
 from .equipment import Equipment
-from ..obsmetadata import (ObsMetadata)
-from ..helpers import str_indent, str_list_str, verify_dict_is_empty
+from obsinfo.obsMetadata.obsmetadata import (ObsMetadata)
+from ..helpers import str_indent, verify_dict_is_empty
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class InstrumentComponent(object):
     """
     InstrumentComponent class. Superclass of all component classes.
     No obspy/StationXML equivalent, because they only specify the whole
@@ -44,17 +47,17 @@
             msg = 'No attributes_dict'
             logger.error(msg)
             raise TypeError(msg)
         if not isinstance(attributes_dict, ObsMetadata):
             attributes_dict = ObsMetadata(attributes_dict)
 
         # Remove elements to be processed in Stages()
-        higher_stage_modifications = ObsMetadata(attributes_dict.pop('stage_modifications', {}))
+        response_modifs = ObsMetadata(attributes_dict.pop('stage_modifications', {}))
         if 'stage_modifications' in higher_modifs:
-            higher_stage_modifications.safe_update(higher_modifs.pop('stage_modifications'))
+            response_modifs.safe_update(higher_modifs.pop('stage_modifications'))
 
         # Put shortcuts in the right place:
         if 'serial_number' in attributes_dict:
             attributes_dict.safe_update(
                 {'modifications':
                     {'equipment':
                         {'serial_number': attributes_dict.pop('serial_number')}
@@ -73,20 +76,16 @@
         
         if 'notes' in base_dict:
             del base_dict['notes']
 
         self.equipment = Equipment(base_dict.pop('equipment', None))
         self.configuration = base_dict.pop('configuration', None)
         self.configuration_description = base_dict.pop('configuration_description', self.configuration)
-        stage_modifications = ObsMetadata(base_dict.pop('stage_modifications', {}))
-        stage_modifications.safe_update(higher_stage_modifications, warn_crush=True)
-        self.stages = Stages(base_dict.pop('stages', []), {'stage_modifications': stage_modifications},
+        self.stages = Stages(base_dict.pop('stages', []), response_modifs,
                              base_dict.get('correction', None))
-        self.equipment.calibration_dates += self.stages.calibration_dates
-        logger.info('Instrument_Component has {len(self.stages)} stages')
         self._error_check(self.stages)
         if self.configuration_description is not None:
             self.equipment.description += ' [config: {}]'.format(
                 self.configuration_description)
         # self.obspy_equipment = self.equipment.to_obspy()
         self.base_dict = base_dict  # leftovers for specific components
 
@@ -111,21 +110,24 @@
             s += f'\n    stages: {self.stages.__str__(**kwargs)}'
         return s
 
     def _error_check(self, stages):
         """Some of these checks seem redundant"""
         if stages is None:
             msg = f'stages is None {type(self)}'
+            warnings.warn(msg)
             logger.warning(msg)
         elif not stages:
             msg = f'No response stages in {type(self)}'
+            warnings.warn(msg)
             logger.error(msg)
             raise TypeError(msg)
         elif len(stages) == 0:
             msg = f'len(stages) == 0 in {type(self)}'
+            warnings.warn(msg)
             logger.error(msg)
             raise TypeError(msg)
 
 
 class Sensor(InstrumentComponent):
     """
     Sensor Instrument Component. No obspy equivalent
@@ -149,15 +151,14 @@
 
         Args:
             attributes_dict (dict or :class:`ObsMetadata`): InstrumentComponent
                 attributes
             higher_modifs (dict or :class:`ObsMetadata`): modifications
                 inherited from instrumentation
         """
-        logger.info('Creating Sensor()')
         super().__init__(attributes_dict, higher_modifs)
         seed_dict = self.base_dict.pop('seed_codes', {})
         self.seed_band_base_code = seed_dict.get('band_base', None)
         self.seed_instrument_code = seed_dict.get('instrument', None)
         verify_dict_is_empty(self.base_dict)
         del self.base_dict
 
@@ -195,15 +196,14 @@
             attributes_dict (dict or :class:`ObsMetadata`): InstrumentComponent
                 attributes
             higher_modifs (dict or :class:`ObsMetadata`): modifications
                 inherited from instrumentation
         Returns:
             (:class:`Datalogger`)
         """
-        logger.info('Creating Datalogger()')
         super().__init__(attributes_dict, higher_modifs)
         self.sample_rate = self.base_dict.pop('sample_rate', None)
         self.correction = self.base_dict.pop('correction', 0)
         verify_dict_is_empty(self.base_dict)
         del self.base_dict
 
     def __str__(self, indent=0, n_subclasses=0):
@@ -230,15 +230,14 @@
         """
         Args:
             attributes_dict (dict or :class:`ObsMetadata`): InstrumentComponent
                 attributes
             higher_modifs (dict or :class:`ObsMetadata`): modifications
                 inherited from instrumentation
         """
-        logger.info('Creating Preamplifier()')
         if not attributes_dict:
             return None   # It is acceptable to have no preamplifier
         super().__init__(attributes_dict, higher_modifs)
         verify_dict_is_empty(self.base_dict)
         del self.base_dict
 
     def __str__(self, indent=0, n_subclasses=0):
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/instrumentation.py` & `obsinfo-0.111b1/obsinfo/instrumentation/instrumentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 # Standard library modules
 import warnings
 import logging
 
 # Non-standard modules
 
 # obsinfo modules
-from ..obsmetadata import ObsMetadata
+from obsinfo.obsMetadata.obsmetadata import ObsMetadata
 from .instrument_component import Equipment
 from .channel import Channel, Channels
 from ..helpers import str_indent, verify_dict_is_empty, Location, ObsinfoClassList
+# from .operator_class import Operator
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Instrumentations(ObsinfoClassList):
@@ -74,15 +75,15 @@
             # No base instrument defined, should act like a None
             self.channels = Channels()
             self.equipment = Equipment({'description': attributes_dict['base']})
             return
         
         ic_names = ('datalogger', 'sensor', 'preamplifier')
 
-        self.input = {'attributes_dict': {} if not attributes_dict else '<ObsMetaData>',
+        self.input = {'attributes_dict': {} if not attributes_dict else '<obsinfo.ObsMetaData>',
                       'station_locations': station_locations,
                       'station_start_date': station_start_date,
                       'station_end_date': station_end_date,
                       'station_location_code': station_location_code}
         
         # Syntax checking - Check whether
         if not attributes_dict:
@@ -96,37 +97,41 @@
         else:
             # Easy mistake of including a dash in the yaml file
             msg = 'Instrumentation is not a dict'
             logger.error(msg)
             raise TypeError(msg)
 
         # Remove elements not to be processed here
-        channel_modifs = attributes_dict.pop('channel_modifications', ObsMetadata({}))
+        channel_modifs = attributes_dict.pop('channel_modifications', {})
 
         # Extract instrument_component modifications
         mods = attributes_dict.get('modifications', None)
         if mods is not None:
             # Extract InstrumentComponent modifications
             ic_modifs = ObsMetadata({ic: mods.pop(ic)
                                     for ic in ic_names if ic in mods})
             # Put remaining modifications back
             attributes_dict['modifications'] = mods
         else:
             ic_modifs = ObsMetadata({})
 
         # Put shortcuts in the right place:
         if 'serial_number' in attributes_dict:
-            x = attributes_dict.pop('serial_number')
             attributes_dict.safe_update(
-                {'modifications': {'equipment': {'serial_number': x}}},
+                {'modifications':
+                    {'equipment':
+                        {'serial_number':
+                         attributes_dict.pop('serial_number')}}},
                 warn_crush=True)
         if 'datalogger_configuration' in attributes_dict:
-            x = attributes_dict.pop('datalogger_configuration')
-            channel_modifs.safe_update(
-                {'*-*': {'datalogger': {'configuration': x}}},
+            attributes_dict.safe_update(
+                {'modifications':
+                    {'datalogger':
+                        {'configuration':
+                         attributes_dict.pop(datalogger_configuration)}}},
                 warn_crush=True)
 
         # Get main elements
         base_dict = attributes_dict.get_configured_modified_base()
         base_location_code = base_dict.pop('location_code', station_location_code)
         ### 'configuration' is solely informational
         base_configuration = base_dict.pop('configuration', None)
@@ -202,15 +207,15 @@
                 Must have 'orientation' and 'location_code' keys
             channel_modifs (dict): channel_modifications, keys are
                 id_codes, in order of priority:
                     "<ORT>-<LOC>": orientation_code <ORT> & location_code <LOC>
                     "<ORT>": orientation_code <ORT>
                     "*-<LOC>": location_code <LOC>, all orientation_codes
                     "<ORT>-*": orientation_code <ORT>, all location_codes
-                    "*-*": All ``id_codes``
+                   "*" or "*-*": All ``id_codes``
             location_code (str): The location
 
         Returns:
             (:class:`ObsMetadata``): the selected channel modifications
         """
         for k in ('orientation', 'location_code'):
             if k not in chan_dict:
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/orientation.py` & `obsinfo-0.111b1/obsinfo/instrumentation/orientation.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import warnings
 import logging
 
 # Non-standard modules
 import obspy.core.util.obspy_types as obspy_types
 
 # obsinfo modules
-from ..obsmetadata import (ObsMetadata)
+from obsinfo.obsMetadata.obsmetadata import (ObsMetadata)
 from ..helpers import FloatWithUncert, str_indent
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
@@ -76,21 +76,19 @@
         self.code = key
         value = ObsMetadata(attributes_dict.pop(key, None))
         azimuth = value.get('azimuth.deg', None)
         dip = value.get('dip.deg', None)
         if azimuth is None and dip is None:
             raise ValueError(f'orientation {key}: neither azimuth nor dip specified')
         if azimuth is not None:
-            azimuth.safe_update({'unit': 'degrees'})
-            self.azimuth = FloatWithUncert(azimuth)
+            self.azimuth = FloatWithUncert(azimuth | {'unit': 'degrees'})
         else:
             self.azimuth = FloatWithUncert({'value': 0, 'unit': 'degrees'})
         if dip is not None:
-            dip.safe_update({'unit': 'degrees'})
-            self.dip = FloatWithUncert(dip)
+            self.dip = FloatWithUncert(dip | {'unit': 'degrees'})
         else:
             self.dip = FloatWithUncert({'value': 0, 'unit': 'degrees'})
             
         # Test required values
         if key in 'XYEN':
             if self.azimuth.uncertainty is None:
                 logger.warning("orientation XYEN should have azimuth uncertainty, doesn't")
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/stage.py` & `obsinfo-0.111b1/obsinfo/instrumentation/stage.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from obspy.core.inventory.response import (
     PolesZerosResponseStage, FIRResponseStage,
     CoefficientsTypeResponseStage, ResponseListResponseStage,
     PolynomialResponseStage)
 import obspy.core.util.obspy_types as obspy_types
 
 # Local modules
-from ..obsmetadata import ObsMetadata
+from ..obsMetadata import ObsMetadata
 from .filter import (Filter, PolesZeros, FIR, Coefficients, ResponseList,
                      Analog, Digital, ADConversion, Polynomial)
-from ..helpers import str_indent, OIDates
+from ..helpers import str_indent
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Stage(object):
@@ -43,14 +43,15 @@
         input_sample_rate (float): input sample rate in sps
         delay (float): delay in seconds of stage. If not present, will be
             calculated from delay from digital stages
         decimation_factor (float): decimation factor of stage
         correction (float) : delay correction. Calculated from instrument
             delay correction
         polarity (str, either "+" or "-"): whether stage changes polarity
+        calibration_date (str in date format): calibration date of stage
         resource_id (str)
         instrument_sensitivity (float): Not used, set to None. Sensitivity
             is calculated for the whole response.
 
     """
     def __init__(self, attributes_dict, higher_modifs=ObsMetadata({}),
                  correction=None, sequence_number=-1,
@@ -70,49 +71,46 @@
            ext_config_name (str): higher-level configuration definition (overrides
                 whatever is in self)
         """
         if attributes_dict is None:
             return None
         
         # input parameters, for __repr__
-        self.inputs = {'attributes_dict': '<ObsMetadata>',
-                       'higher_modifs': '<ObsMetadata>',
+        self.inputs = {'higher_modifs': ':class:`ObsMetadata`',
                        'correction': correction,
                        'sequence_number': sequence_number,
                        'ext_config_name': ext_config_name}
         if not higher_modifs:
                     self.inputs['higher_modifs'] = '{}'
 
         if not isinstance(attributes_dict, ObsMetadata):
             attributes_dict = ObsMetadata(attributes_dict)
         if not isinstance(higher_modifs, ObsMetadata):
             higher_modifs = ObsMetadata(higher_modifs)
 
-        # put appropriate "stage_modifications" in "modifications"
+        # replace "stage_modifications" by "modifications" before sending off
+        # to ObsMetadata.get_configured_modified_base()
         m = self._get_stage_modifications(
             attributes_dict.pop('stage_modifications', {}), sequence_number)
+        hm = self._get_stage_modifications(
+            higher_modifs.pop('stage_modifications', {}), sequence_number)
         if "modifications" in attributes_dict:
             attributes_dict['modifications'].safe_update(m)
         elif not m == {}:
             attributes_dict['modifications'] = m
 
-        hm = self._get_stage_modifications(
-            higher_modifs.pop('stage_modifications', {}), sequence_number)
         if "modifications" in higher_modifs:
             higher_modifs['modifications'].safe_update(hm)
         elif not hm == {}:
             higher_modifs['modifications'] = hm
 
         base_dict = attributes_dict.get_configured_modified_base(higher_modifs)
 
         self.name = base_dict.pop('name', None)  
-        self.configuration = base_dict.pop('configuration', None)
-        # CalibrationDates belongs in equipment, but is more logical to state
-        # in stage, rely on equipment to look for it.    
-        self.calibration_dates = OIDates(base_dict.pop('calibration_dates', []) )     
+        self.configuration = base_dict.pop('configuration', None)      
         self.configuration_description = base_dict.pop('configuration_description',
                                                        self.configuration)      
         self.description = base_dict.pop('description', '')
         if self.configuration_description is not None:
             if self.name is None:
                 self.name = f'[config: {self.configuration_description}]'
             else:
@@ -121,26 +119,24 @@
         gd = base_dict.pop('gain', None)
         if gd is None:
             msg = f'No gain specified in stage {self.name}'
             logger.error(msg)
             raise TypeError(msg)
         self.gain = gd.get('value', 1.0)
         self.gain_frequency = gd.get('frequency', 0.0)
-        self.stage_sequence_number = sequence_number
 
-
-        self.filter = Filter.construct(base_dict.pop('filter'),
-                                       self.stage_sequence_number,
-                                       self.name,
+        self.filter = Filter.construct(base_dict.pop('filter'), self.name,
                                        self.gain_frequency)
         if not self.filter:
             msg = f'No filter in stage {self.name}'
             logger.error(msg)
             raise TypeError(msg)
 
+        self.stage_sequence_number = sequence_number
+
         x = base_dict.pop('input_units', None)
         if x:
             self.input_units = x.get('name', None)
             self.input_units_description = x.get('description', None)
 
         x = base_dict.pop('output_units', None)
         if x:
@@ -155,14 +151,15 @@
         self._delay = base_dict.pop('delay', None)
         self.decimation_factor = base_dict.pop('decimation_factor', 1)
         self.correction = correction
 
         # default polarity is positive
         self.polarity = base_dict.pop('polarity', 1)
         self.resource_id = base_dict.pop('resource_id', None)
+        self.calibration_date = base_dict.pop('calibration_date', None)
         self.instrument_sensitivity = None
         # Instrument sensitivity will be calculated using obspy and stored in
         # first stage
         if len(base_dict) > 0:
             raise ValueError('base_dict has remaing fields: {}'
                              .format([x for x in base_dict.keys()]))
 
@@ -194,15 +191,15 @@
         # Calculate delay based on filter
         if self.filter.delay_seconds is not None:
             filter_delay = self.filter.delay_seconds
         elif self.filter.delay_samples is not None:
             if not self.input_sample_rate:
                 # Delay is already none, leave it like that
                 msg = ('Cannot calculate delay from delay_samples '
-                       f'because stage {self.name} has no input_sample_rate')
+                       f'because stage {self.name}has no input_sample_rate')
                 logger.warning(msg)
                 warnings.warn(msg)
             else:
                 filter_delay = self.filter.delay_samples / self.input_sample_rate
 
         if self._delay is None:
             return filter_delay 
@@ -213,47 +210,44 @@
                    f" ({self._delay} != {filter_delay}): ignoring filter "
                    "delay")
             warning.warn(msg)
             logger.warning(msg)
         return self._delay
         
     def __repr__(self):
-        return (f"Stage({self.inputs['attributes_dict']}, "
-                f"{self.inputs['higher_modifs']}, "
-                f"{self.inputs['correction']}, "
-                f"{self.inputs['sequence_number']}, "
-                f"{self.inputs['ext_config_name']})")
+        return (f"Stage(:class:`ObsMetadata`, {self.inputs['higher_modifs']},"
+                f" {self.inputs['correction']}, {self.inputs['sequence_number']},"
+                f" {self.inputs['ext_config_name']})")
 
     def __str__(self, indent=0, n_subclasses=0):
         if n_subclasses < 0:
             return f'{type(self)}'
-        kwargs = {'indent': 4, 'n_subclasses': n_subclasses-1}
         s = f'Stage:\n'
         s += f'    name: {self.name}\n'
         s += f'    description: {self.description}\n'
         s += f'    input_units: {self.input_units}\n'
         s += f'    output_units: {self.output_units}\n'
         s += f'    gain: {self.gain}\n'
         s += f'    gain_frequency: {self.gain_frequency:g}\n'
-        s += f'    filter: {self.filter.__str__(**kwargs)}\n'
+        s += f'    filter: {self.filter.__str__(4, n_subclasses-1)}\n'
         if not self.stage_sequence_number == -1:
             s += f'    stage_sequence_number: {self.stage_sequence_number}\n'
-        if self.calibration_dates is not None:
-            s += f'    calibration_dates: {self.calibration_dates.__str__(**kwargs)}\n'
         if self.input_units_description:
             s += f'    input_units_description: {self.input_units_description}\n'
         if self.output_units_description:
             s += f'    output_units_description: {self.output_units_description}\n'
         if self.input_sample_rate:
             s += f'    input_sample_rate: {self.input_sample_rate}\n'
 
         s += f'    decimation_factor: {self.decimation_factor}\n'
         s += f'    delay: {self.delay}\n'
         s += f'    correction: {self.correction}'
 
+        if self.calibration_date:
+            s += f'\n    calibration_dates={self.calibration_date}'
         return str_indent(s, indent)
 
     def to_obspy(self):
         """
         Return equivalent *obspy.core.inventory.response* classes stages:
 
         Possible stage classes:
@@ -352,17 +346,16 @@
             msg = 'Unhandled response stage type in stage '\
                   f'#{self.stage_sequence_number}: "{filt.type}"'
             warnings.warn(msg)
             logger.error(msg)
             raise TypeError(msg)
 
         return obspy_stage
-    
-    @staticmethod
-    def _get_stage_modifications(resp_modifs, sequence_number):
+
+    def _get_stage_modifications(self, resp_modifs, sequence_number):
         """
         Select which channel modifications specified at station level apply
         to a given stage,  with the stage number (WITHIN an instrument
         component) as key code
 
         Args:
             resp_modifs (dict or :class:`.ObsMetadata`): response modifications:
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/instrumentation/stages.py` & `obsinfo-0.111b1/obsinfo/instrumentation/stages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Stages and Stage classes
 """
 # Standard library modules
 import warnings
 import logging
 
-from ..obsmetadata import ObsMetadata
+from ..obsMetadata import ObsMetadata
 from .stage import Stage
-from ..helpers import ObsinfoClassList, OIDates
+from ..helpers import ObsinfoClassList
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Stages(ObsinfoClassList):
@@ -20,68 +20,61 @@
     
     Has a custom constructor using a list of attribute_dicts, and custom
     input_units(), output_units and to_obspy() methods
 
     Attributes:
         stages (list of objects of :class:`Stage`)
     """
-    def __init__(self, attribute_list=None, higher_modifications={},
-                 correction=None):
+    def __init__(self, attribute_list=None, modifs={},
+                 correction=None):  # , ext_config_name=None):
         """
         Constructor
 
         Args:
             attribute_list (list of dicts): information file
                 dictionaries for each stage
-            higher_modifications (dict or :class:`.ObsMetadata`): modifications to
-                pass down to Stage
+            modifs (dict or :class:`.ObsMetadata`):
+                modifications to pass down to Stage
             correction (float): used only for datalogger: the delay
                 correction for the entire instrument
+            # ext_config_name (str): external configuration name applied to
+            #     every stage.
         """
         if attribute_list is None:
             msg = 'No stages in information file'
             warnings.warn(msg)
             logger.warning(msg)
-            super().__init__([], Stage)
+            super().__init__([])
+            # self.stages = None
         else:
             stages = []
-            logger.debug(f'{higher_modifications=}')
             for s, i in zip(attribute_list, range(0, len(attribute_list))):
                 # Assign correction value
                 if correction is None:
                     correction = None
                 elif i == len(attribute_list)-1:
                     correction = correction
                 else:
                     correction = 0
-                stages.append(Stage(ObsMetadata(s),
-                                    higher_modifications,
-                                    correction, i+1))
+                stages.append(
+                    Stage(ObsMetadata(s), modifs, correction, i+1)) # , ext_config_name))
                 if i > 0:
                     # Check that input units match prior output units
                     s = stages
                     if not s[i].input_units == s[i-1].output_units:
                         raise ValueError(f'stage {i:d} input units do not '
                                          f'match stage {i-1:d} output units '
                                          '("{}"~="{}")'.format(
                                             s[i].input_units,
                                             s[i-1].output_units))
-            super().__init__(stages, Stage)
+            super().__init__(stages)
 
 
     @property
     def input_units(self):
         return self[0].input_units
         # return self.stages[0].input_units
 
     @property
     def output_units(self):
         return self[-1].output_units
         # return self.stages[-1].output_units
-
-    @property
-    def calibration_dates(self):
-        caldates = OIDates([])
-        for x in self:
-            if x is not None:
-                caldates.extend(x.calibration_dates)
-        return caldates
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/misc/configuration.py` & `obsinfo-0.111b1/obsinfo/misc/configuration.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/misc/const.py` & `obsinfo-0.111b1/obsinfo/misc/const.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/misc/discoveryfiles.py` & `obsinfo-0.111b1/obsinfo/misc/discoveryfiles.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/misc/printobs.py` & `obsinfo-0.111b1/obsinfo/misc/printobs.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/misc/remoteGitLab.py` & `obsinfo-0.111b1/obsinfo/misc/remoteGitLab.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/misc/yamlref.py` & `obsinfo-0.111b1/obsinfo/misc/yamlref.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,15 +446,15 @@
         :returns: dictionary of parsed YAML or JSON formats
         :raises: FileNotFoundError, IOError, OSError
 
         """
         scheme = urlparse.urlsplit(uri).scheme
         path = urlparse.urlsplit(uri).path
 
-        logger.debug(f"Opening file: {path}")
+        logger.info(f"Opening file: {path}")
         # Open locally or remotely according to scheme
         if scheme == 'file':
             try:
                 with open(path, "rt") as fp:
                     strm = fp.read()
             except FileNotFoundError:
                 msg = f'File not found: {path}'
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/obsmetadata/obsmetadata.py` & `obsinfo-0.111b1/obsinfo/obsMetadata/obsmetadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 obsinfo information file routines, contained in superclass ObsMetadata for
 generality
 """
 # Standard library modules
 import json
 from pathlib import Path, PurePath
+import warnings
 from urllib.parse import urlparse
 from urllib.parse import unquote
 import logging
 import time
 
 # Non-standard modules
 import jsonschema
@@ -16,17 +17,18 @@
 
 # Local modules
 from ..misc import yamlref
 from ..misc.yamlref import JsonLoader
 from ..misc.remoteGitLab import gitLabFile
 from ..misc.discoveryfiles import Datapath
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
-overwrite_symbol = '^'      # Used by safe_update
 root_symbol = "#"
 VALID_FORMATS = ["JSON", "YAML"]
 DEFAULT_SCHEMA_PATH = Path(__file__).parent.parent.joinpath('data', 'schemas')
 VALID_TYPES = [Path(f.stem).stem
                for f in DEFAULT_SCHEMA_PATH.glob('*.schema.json')]
 
 
@@ -89,16 +91,14 @@
         if quiet:
             verbose = False
 
         # Get schema filename
         if not schema_filename:
             if not file_type:
                 file_type = ObsMetadata.get_information_file_type(info_filename)
-            if file_type is None:
-                logger.error(f'Could not determine file type for {info_filename}')
             schema_filename = file_type + '.schema.json'
 
         # Get infofile instance and schema
         if dp is None:
             dp = Datapath()
         instance = self.read_info_file(info_filename, dp, remote, False,
                                        file_format, verbose)
@@ -196,16 +196,16 @@
         """
         stem = PurePath(filename).stem
         suffix = PurePath(stem).suffix
         type = suffix[1:]
         if type in VALID_TYPES:
             return type
         msg = f"File '{filename}' is of unknown type: {type}"
-        logger.warning(msg)
-        return None
+        logger.error(msg)
+        raise ValueError(msg)
 
     def read_json_yaml(filename, file_format=None):
         """
         Reads a JSON or YAML file. Does NOT use jsonReference  DEPRECATED.
 
         DEPRECATED. Not being used by any obsinfo method or function. Kept
         for compatibility
@@ -349,16 +349,14 @@
         Returns:
             (:class:`ObsMetadata`): JSON or YAML parsed info files
         """
         if quiet is True:
             verbose = False
         if validate:
             file_type = ObsMetadata.get_information_file_type(filename)
-            if file_type is None:
-                logger.error(f'Could not determine type of file {filename}')
             msg = f'Validating {file_type} file: {filename}'
             logger.info(msg)
             if verbose:
                 print(msg)
             ObsMetadata().validate(str(filename), DEFAULT_SCHEMA_PATH,
                                    remote=remote, verbose=verbose, quiet=quiet)
         else:
@@ -432,16 +430,16 @@
             raise ValueError('higher_level base-configuration-modification '
                              f'dict had leftover elements: {b}')
 
         # Configure, then modify
         configs = base_dict.pop("configurations", None)
         if configuration is not None:
             if configs is None:
-                raise ValueError(f"'{configuration}' configuration was requested"
-                                 ', but no configurations were specified')
+                raise ValueError(f"Configuration requested ('{configuration}')"
+                                 ', but no configurations specified')
             if configuration not in configs:
                 raise ValueError(
                     f"Requested configuration ('{configuration}') doesn't "
                     f"match specified configurations: {list(configs.keys())}")
             base_dict.safe_update(configs[configuration])
             base_dict['configuration'] = configuration
         base_dict.safe_update(modifs)
@@ -449,16 +447,15 @@
         return base_dict
         
     def safe_update(self, update_dict, allow_overwrite=True, warn_crush=False):
         """
         Update that only changes explicitly specfied fields
 
         Drills recursively through dicts inside the dict, only changing fields
-        which are specified in update_dict.  Lists are completely replaced, 
-        however, to avoid ambiguity.
+        which are specified in update_dict
 
         Args:
             update_dict (dict or :class:`ObsMetadata`): dictionary containing
                 fields to update
             allow_overwrite (bool): allow a field that was originally a dict
                 to be overwritten by a field that is not a dict.  Same for lists.
             warn_crush (bool): write out a warning when a value is replaced
@@ -468,78 +465,73 @@
             raise TypeError('update_dict is not a dict')
         if not isinstance(update_dict, self.__class__):
             update_dict = self.__class__(update_dict)
         for key, value in update_dict.items():
             # Change any dict into ObsMetadata
             if isinstance(value, dict) and not isinstance(value, self.__class__):
                 value = self.__class__(value)
-            if key[0] == overwrite_symbol:
-                key=key[1:]
-                if key in self:
-                    logger.info('Overwrite ordered for key {key}')
-                self[key] = value
-                continue  # Go to next loop iteration
             if key not in self:  # Add new key and its value
                 self[key] = value
-                continue  # Go to next loop iteration
-            # Key exists in self and not forced overwrite
-            if isinstance(self[key], dict):  # If original item is a dict
-                # if value is also a dictionary, update it
-                if isinstance(value,  dict):
-                    # if replacement value is a dictionary, recurse
-                    self[key].safe_update(value,
-                                          allow_overwrite=allow_overwrite,
-                                          warn_crush=warn_crush)
-                else:
-                    # if replacement value is not a dictionary
-                    if allow_overwrite:  # replace & warn
-                        self[key] = value
-                        logger.warning(f'dict field "{key}" '
-                                       'was replaced by a non-dict')
-                    else:  # reject & warn
-                        logger.warning(
-                            f'replacement field "{key}" was not inserted '
-                            'into original because original was a dict '
-                            'but replacement was not')
-            elif isinstance(self[key], list):  # If original item is a list
-                if isinstance(value,  list):   # If replacement is also a list
-                    # Replace the list
-                    self[key] = value
-                    logger.debug(f'"{key}": {len(self[key])}-element list replaced by {len(value)}-element list')
-                    # Recurse on contents
-                    # replacer = []
-                    # for item, holder in zip(value, self[key]):
-                    #     if isinstance(item, (dict, ObsMetadata)):
-                    #         holder = ObsMetadata(holder)  # SHOULDN'T BE NECESSARY!
-                    #         holder.safe_update(self.__class__(item),
-                    #                            allow_overwrite=allow_overwrite,
-                    #                            warn_crush=warn_crush)
-                    #     elif isinstance(item, list):
-                    #         raise ValueError('does not handle lists in lists')
-                    #     else:
-                    #         holder = item
-                    #     replacer.append(holder)
-                    # self[key] = replacer
+            else:  # Key exists in self:
+                if isinstance(self[key], dict):  # If original item is a dict
+                    # if value is also a dictionary, update it
+                    if isinstance(value,  dict):
+                        # if replacement value is a dictionary, recurse
+                        self[key].safe_update(value,
+                                              allow_overwrite=allow_overwrite,
+                                              warn_crush=warn_crush)
+                    else:
+                        # if replacement value is not a dictionary
+                        if allow_overwrite:  # replace & warn
+                            self[key] = value
+                            msg = f'field "{key}" was a dict, replaced by a non-dict'
+                            warnings.warn(msg)
+                            logger.warning(msg)
+                        else:  # reject & warn
+                            msg = (f'replacement field "{key}" not inserted '
+                                   'into original because original was a dict '
+                                   'but replacement was not')
+                            warnings.warn(msg)
+                            logger.warning(msg)
+                elif isinstance(self[key], list):  # If original item is a list
+                    if isinstance(value,  list):   # If replacement is also a list
+                        # Recurse on contents
+                        replacer = []
+                        for item, holder in zip(value, self[key]):
+                            if isinstance(item, (dict, ObsMetadata)):
+                                holder = ObsMetadata(holder)  # SHOULDN'T BE NECESSARY!
+                                holder.safe_update(self.__class__(item),
+                                                   allow_overwrite=allow_overwrite,
+                                                   warn_crush=warn_crush)
+                            elif isinstance(item, list):
+                                raise ValueError('does not handle lists in lists')
+                            else:
+                                holder = item
+                            replacer.append(holder)
+                        self[key] = replacer
+                    else:
+                        # if replacement value is not a list
+                        if allow_overwrite:  # replace & warn
+                            self[key] = value
+                            msg = f'field "{key}" was a list, replaced by a non-list'
+                            warnings.warn(msg)
+                            logger.warning(msg)
+                        else:  # reject & warn
+                            msg = (f'replacement field "{key}" not inserted '
+                                   'into original because original was a list '
+                                   'but replacement was not')
+                            warnings.warn(msg)
+                            logger.warning(msg)
                 else:
-                    # if replacement value is not a list
-                    if allow_overwrite:  # replace & warn
-                        self[key] = value
-                        msg = f'field "{key}" was a list, replaced by a non-list'
+                    # Replace existing others
+                    if key in self and warn_crush is True:
+                        msg = f'replacing self["{key}"]: was {self[key]}, now {value}'
+                        warnings.warn(msg)
                         logger.warning(msg)
-                    else:  # reject & warn
-                        msg = (f'replacement field "{key}" not inserted '
-                               'into original because original was a list '
-                               'but replacement was not')
-                        logger.warning(msg)
-            else:
-                # Replace existing others
-                if key in self and warn_crush is True:
-                    msg = f'replacing self["{key}"]: was {self[key]}, now {value}'
-                    logger.warning(msg)
-                self[key] = value
+                    self[key] = value
 
     def copy(self):
         return ObsMetadata(super().copy())
 
     def _convert_to_obsmetadata(self):
         """
         Make all contained dictionaries objects of :class: `.ObsMetadata`
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/subnetwork/operator.py` & `obsinfo-0.111b1/obsinfo/subnetwork/operator.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
         self.agency = attributes_dict['agency']     # required
         self.contacts = Persons(attributes_dict.get('contacts', None))
         self.website = attributes_dict.get('website', None)
 
     def __str__(self, indent=0, n_subclasses=0):
         if n_subclasses < 1:
-            return f'agency: {self.agency}'
+            return f'{type(self)}'
         kwargs = dict(indent=4, n_subclasses=n_subclasses-1)
         s = f'{self.__class__.__name__}:\n'
         s += f'    agency: {self.agency}\n'
         s += f'    contacts: {self.contacts.__str__(**kwargs)}\n'
         s += f'    website: {self.website}'
         return str_indent(s, indent)
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/subnetwork/processing.py` & `obsinfo-0.111b1/obsinfo/subnetwork/processing.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/subnetwork/site.py` & `obsinfo-0.111b1/obsinfo/subnetwork/site.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/subnetwork/station.py` & `obsinfo-0.111b1/obsinfo/subnetwork/station.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Station Class
 """
 # Standard library modules
+import warnings
 import logging
 
 # Non-standard modules
 from obspy.core.inventory.station import Station as obspy_Station
 
 from obspy.core.inventory.util import (Comment)
 from obspy.core.utcdatetime import UTCDateTime
@@ -14,40 +15,41 @@
 # obsinfo modules
 from .processing import Processing
 from ..instrumentation import Instrumentation, Instrumentations
 from ..helpers import (Location, Locations, OIDate,
                        str_list_str, str_indent, verify_dict_is_empty,
                        ObsinfoClassList, Comments, ExternalReferences, Identifiers)
 from .operator import Operators
-from ..obsmetadata import ObsMetadata
+from ..obsMetadata import ObsMetadata
 from .site import Site
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Stations(ObsinfoClassList):
     """
     A list of Station objects
     """
-    def __init__(self, stations_dict, station_only, operators, comments):
+    def __init__(self, stations_dict, station_only, stations_operators):
         """
-        Args:
-            stations_dict: (dict or :class:`.ObsMetadata`): dictionary
-                from station or network info file with YAML or JSON
-                attributes
-            station_only (boolean): Creates object with no instrumentation
-            operators (:class:`.Operators`): default station
-                operators
-            comments: (:class:`.Comments`): default station comments
+            Args:
+                stations_dict: (dict or :class:`.ObsMetadata`): dictionary
+                    from station or network info file with YAML or JSON
+                    attributes
+                station_only (boolean): Creates object with no instrumentation
+                stations_operators (:class:`.Operators`): default station
+                    operators
         """
         if stations_dict is None:
             super().__init__([])
         else:
-            super().__init__([Station(k, v, station_only, operators, comments)
-                             for k, v in (stations_dict.items())], Station)
+            super().__init__([Station(k, v, station_only, stations_operators)
+                             for k, v in (stations_dict.items())])
 
 
 class Station(object):
     """
     Station. Equivalent to obspy/StationXML Station
 
     Methods convert info files to an instance of this class and convert the
@@ -75,34 +77,33 @@
             a dict with keys ['uri', 'description']
         water_level (number): elevation (m) of water surface (useful for lakes)
         obspy_station (:class:`obspy.core.inventory.station.Station`):
             Equivalent obspy object
     """
 
     def __init__(self, code, attributes_dict, station_only=False,
-                 stations_operators=None, stations_comments=None):
+                 stations_operators=None):
         """
         Constructor
 
         Args:
             attributes_dict: (dict or :class:`.ObsMetadata`): dictionary
                 from station or network info file with YAML or JSON attributes
             station_only (boolean): Creates object with no instrumentation
             stations_operators (:class:`.Operators`): default station
                 operator(s)
-            stations_comments: (:class:`.Comments`): default station comments
         Raises:
             TypeError
         """
         if not attributes_dict:
             msg = 'No station attributes'
+            warnings.warn(msg)
             logger.error(msg)
             raise TypeError(msg)
 
-        logger.info(f'Creating Station "{code}"')
         self.code = code
         self.site = Site(attributes_dict.pop("site", None))
         self.start_date = OIDate(attributes_dict.pop("start_date"))
         self.end_date = OIDate(attributes_dict.pop("end_date"))
         self.location_code = attributes_dict.pop("location_code")
         self.restricted_status = attributes_dict.pop("restricted_status", None)
         self.operators = Operators(attributes_dict.pop("operators", None))
@@ -124,16 +125,14 @@
             else:
                 self.instrumentations = Instrumentations([Instrumentation(
                     instr_dict, self.locations, self.location_code,
                     self.start_date.date, self.end_date.date)])
 
         self.processing = Processing(attributes_dict.pop('processing', None))
         self.comments = Comments(attributes_dict.pop("comments", []))
-        if stations_comments is not None:
-            self.comments += stations_comments
         self.source_id = attributes_dict.pop('source_id', None)
         self.identifiers = Identifiers(attributes_dict.pop('identifiers', None))
         self.extras = attributes_dict.pop('extras', None)
         self.external_references = ExternalReferences(attributes_dict.pop('external_references', None))
         self.comments += Comments.from_extras(attributes_dict.pop('extras', None))
         self.comments += self.processing.to_comments()
         if 'notes' in attributes_dict:
@@ -148,15 +147,15 @@
         if self.processing:
             s += f'processing-steps: {self.processing.processing_list}'
         s += ')'
         return s
 
     def __str__(self, indent=0, n_subclasses=0):
         if n_subclasses < 0:
-            return f'{self.__class__.__name__} {self.code}'
+            return f'{self.__class__.__name__}: {self.code}'
         kwargs = dict(indent=4, n_subclasses=n_subclasses-1)
         s = f'{self.__class__.__name__}:\n'
         s += f'    code: {self.code}\n'
         s += f'    site: {self.site}\n'
         s += f'    start_date: {self.start_date}\n'
         s += f'    end_date: {self.end_date}\n'
         s += f'    location_code: {self.location_code}\n'
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/tests/CompareXMLTree.py` & `obsinfo-0.111b1/obsinfo/tests/CompareXMLTree.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/tests/remoteGithub.py` & `obsinfo-0.111b1/obsinfo/tests/remoteGithub.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/tests/run_test_script.py` & `obsinfo-0.111b1/obsinfo/tests/run_test_script.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,35 +62,38 @@
 import inspect
 import difflib
 import re
 import glob
 from json.decoder import JSONDecodeError
 from argparse import ArgumentParser
 
+import logging
+from logging.handlers import RotatingFileHandler
+
+
 #Third party  imports
 from obspy.core.utcdatetime import UTCDateTime
 from obspy.core.inventory.util import  (Latitude, Longitude, Site, Comment)
 
 # obsinfo modules
-from ..obsmetadata import (ObsMetadata)
-from ..instrumentation import (Instrumentation, InstrumentComponent,
+from obsinfo.obsMetadata.obsmetadata import (ObsMetadata)
+from obsinfo.instrumentation import (Instrumentation, InstrumentComponent,
                                      Datalogger, Preamplifier, Sensor,
                                      Stages, Stage, Filter)
-from ..helpers import Location, init_logging
-from ..network import (Station, Subnetwork)
-from ..instrumentation.filter import (Filter, PolesZeros, FIR, Coefficients, ResponseList,
+from obsinfo.helpers import Location
+from obsinfo.network import (Station, Subnetwork)
+from obsinfo.instrumentation.filter import (Filter, PolesZeros, FIR, Coefficients, ResponseList,
                      Analog, Digital, AD_Conversion)
-from ..misc.printobs import  (PrintObs)
-from ..misc.discoveryfiles import Datapath
+from obsinfo.misc.printobs import  (PrintObs)
+from obsinfo.misc.discoveryfiles import Datapath
 import obsinfo
-from ..misc.const import *
-from ..misc.configuration import Singleton
+from obsinfo.misc.const import *
+from obsinfo.misc.configuration import Singleton
 
 verbose = False
-logger = init_logging("run_test_script")
 
 class JsonRefTest(unittest.TestCase):
     """
     Class of test methods for information file format
     
     Attributes:
         testing_path (str): path to datafiles to be tested aside from the examples
@@ -1477,14 +1480,15 @@
     
     """
 
     args = retrieve_arguments()
     tst = TestObsinfo()
     tst.setUp(test=False, print_output=True, level=args.level) 
     dp = Datapath()
+    logger = init_logging()
         
     try:               
         
         type = ObsMetadata.get_information_file_type(args.input_filename)
          
         print(f'Printing {type} file: {args.input_filename}')
             
@@ -1500,16 +1504,14 @@
             tst._test_sensor(tst.infofiles_path.build_datapath(args.input_filename))
         elif type == "instrumentation":
             tst._test_instrumentation(tst.infofiles_path.build_datapath(args.input_filename))
         elif type == "station":
             tst._test_station(tst.infofiles_path.build_datapath(args.input_filename))
         elif type == "subnetwork":
             tst._test_subnetwork(tst.infofiles_path.build_datapath(args.input_filename))
-        else:
-            logger.error(f'Unknown file type "{type}" for file {args.input_filename}')
     
     except TypeError:
         print("Illegal format: fields may be missing or with wrong format in input file, or there is a programming error")
         logger.error("TypeError: Illegal format: fields may be missing or with wrong format in input file, or there is a programming error")
         if args.debug:
             raise
         
@@ -1594,10 +1596,33 @@
      
     if not Path(args.input_filename[0]).is_absolute():
         args.input_filename = str(Path(os.getcwd()).joinpath(args.input_filename[0]).resolve())
              
     return args  
 
 
+def init_logging():
+    """
+    Create or open a rotating logging file and add it to ObsinfoConfiguration
+    
+    :returns: object of Logger class 
+    """
+    
+    logfile = Path.home().joinpath('.obsinfo', 'obsinfolog-validate')
+    
+    
+    logger = logging.getLogger("obsinfo")
+    
+    logger.setLevel(logging.DEBUG)
+    # add a rotating handler with 200K (approx) files and just two files
+    handler = RotatingFileHandler(logfile, maxBytes=200000,
+                                  backupCount=2)
+    frmt = logging.Formatter(fmt='%(asctime)s %(levelname)-8s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+    handler.setFormatter(frmt)
+    logger.addHandler(handler)  
+    
+    return logger 
+
+
 if __name__ == '__main__':
     run_suite_yaml()
     run_suite_info_files(["--all"])
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/tests/test_datapath.py` & `obsinfo-0.111b1/obsinfo/tests/test_datapath.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,23 +66,23 @@
 import logging
 
 # Third party imports
 from obspy.core.utcdatetime import UTCDateTime
 from obspy.core.inventory.util import Site
 
 # obsinfo modules
-from ..obsmetadata import (ObsMetadata)
-from ..instrumentation import (Instrumentation, InstrumentComponent,
+from obsinfo.obsMetadata.obsmetadata import (ObsMetadata)
+from obsinfo.instrumentation import (Instrumentation, InstrumentComponent,
                                      Stage, Filter)
-from ..helpers import Location
-from ..subnetwork import (Station, Subnetwork)
-from ..instrumentation.filter import (PolesZeros, FIR, Coefficients,
+from obsinfo.helpers import Location
+from obsinfo.subnetwork import (Station, Subnetwork)
+from obsinfo.instrumentation.filter import (PolesZeros, FIR, Coefficients,
                                             ResponseList)
-from ..misc.printobs import (PrintObs)
-from ..misc.discoveryfiles import Datapath
+from obsinfo.misc.printobs import (PrintObs)
+from obsinfo.misc.discoveryfiles import Datapath
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 verbose = True
 
 
 class TestDatapath(unittest.TestCase):
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/tests/test_infofile.py` & `obsinfo-0.111b1/obsinfo/tests/test_infofile.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,22 +79,22 @@
 # from logging.handlers import RotatingFileHandler
 
 # Third party imports
 from obspy.core.utcdatetime import UTCDateTime
 from obspy.core.inventory.util import Site
 
 # obsinfo modules
-from ..obsmetadata import (ObsMetadata)
-from ..instrumentation import (Instrumentation, InstrumentComponent,
+from obsinfo.obsMetadata.obsmetadata import (ObsMetadata)
+from obsinfo.instrumentation import (Instrumentation, InstrumentComponent,
                                      Stages, Stage, Filter)
-from ..helpers import Location
-from ..subnetwork import (Station, Subnetwork)
-from ..instrumentation.filter import (PolesZeros, FIR, Coefficients, ResponseList)
-from ..misc.printobs import (PrintObs)
-from ..misc.discoveryfiles import Datapath
+from obsinfo.helpers import Location
+from obsinfo.subnetwork import (Station, Subnetwork)
+from obsinfo.instrumentation.filter import (PolesZeros, FIR, Coefficients, ResponseList)
+from obsinfo.misc.printobs import (PrintObs)
+from obsinfo.misc.discoveryfiles import Datapath
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 verbose = False
 
 
 class TestObsinfo(unittest.TestCase):
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo/tests/test_main.py` & `obsinfo-0.111b1/obsinfo/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post4/src/obsinfo.egg-info/PKG-INFO` & `obsinfo-0.111b1/obsinfo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsinfo
-Version: 0.111.1.post4
+Version: 0.111b1
 Summary: Tools for documenting ocean bottom seismometer experiments and creating metadata
 Home-page: https://gitlab.com/resif/obsinfo
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: seismology OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `obsinfo-0.111.1.post4/src/obsinfo.egg-info/entry_points.txt` & `obsinfo-0.111b1/obsinfo.egg-info/entry_points.txt`

 * *Files identical despite different names*


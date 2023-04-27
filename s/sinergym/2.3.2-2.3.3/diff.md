# Comparing `tmp/sinergym-2.3.2.tar.gz` & `tmp/sinergym-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinergym-2.3.2.tar", last modified: Tue Apr 18 10:20:59 2023, max compression
+gzip compressed data, was "sinergym-2.3.3.tar", last modified: Thu Apr 27 10:29:21 2023, max compression
```

## Comparing `sinergym-2.3.2.tar` & `sinergym-2.3.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:20:59.865363 sinergym-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 10:20:57.000000 sinergym-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-18 10:20:57.000000 sinergym-2.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-04-18 10:20:59.865363 sinergym-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16138 2023-04-18 10:20:57.000000 sinergym-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-18 10:20:59.000000 sinergym-2.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-18 10:20:59.865363 sinergym-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-18 10:20:59.000000 sinergym-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:20:59.837362 sinergym-2.3.2/sinergym/
--rw-r--r--   0 runner    (1001) docker     (123)    94684 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:20:59.837362 sinergym-2.3.2/sinergym/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:20:59.841362 sinergym-2.3.2/sinergym/data/buildings/
--rw-r--r--   0 runner    (1001) docker     (123)   168677 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf
--rw-r--r--   0 runner    (1001) docker     (123)   140099 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/buildings/5ZoneAutoDXVAV.idf
--rw-r--r--   0 runner    (1001) docker     (123)   586238 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf
--rw-r--r--   0 runner    (1001) docker     (123)   373188 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf
--rw-r--r--   0 runner    (1001) docker     (123)   475269 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/buildings/OfficeGridStorageSmoothing.idf
--rw-r--r--   0 runner    (1001) docker     (123)   265862 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/buildings/ShopWithVandBattery.idf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:20:59.841362 sinergym-2.3.2/sinergym/data/variables/
--rw-r--r--   0 runner    (1001) docker     (123)    35474 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    32612 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/variables/5ZoneAutoDXVAV.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    39868 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    42336 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/variables/OfficeGridStorageSmoothing.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/variables/ShopWithVandBattery.rdd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:20:59.861362 sinergym-2.3.2/sinergym/data/weather/
--rw-r--r--   0 runner    (1001) docker     (123)    28629 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1565086 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28503 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1550279 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28704 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1621761 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1553382 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28801 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1558629 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1558423 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1601571 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1637298 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1629153 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1639985 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29614 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1613784 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1624547 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1625209 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:20:59.861362 sinergym-2.3.2/sinergym/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/envs/eplus_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:20:59.865363 sinergym-2.3.2/sinergym/simulators/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/simulators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/simulators/eplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/simulators/eplus_alpha.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:20:59.865363 sinergym-2.3.2/sinergym/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    32883 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    39674 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/utils/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/utils/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/utils/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/utils/rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/utils/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:20:59.837362 sinergym-2.3.2/sinergym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 10:20:59.000000 sinergym-2.3.2/sinergym.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.579013 sinergym-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 10:29:18.000000 sinergym-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-27 10:29:18.000000 sinergym-2.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-04-27 10:29:21.579013 sinergym-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-04-27 10:29:18.000000 sinergym-2.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-27 10:29:20.000000 sinergym-2.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-27 10:29:21.579013 sinergym-2.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-27 10:29:20.000000 sinergym-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.551013 sinergym-2.3.3/sinergym/
+-rw-r--r--   0 runner    (1001) docker     (123)    94684 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.551013 sinergym-2.3.3/sinergym/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.555013 sinergym-2.3.3/sinergym/data/buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)   168677 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   140099 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/buildings/5ZoneAutoDXVAV.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   586238 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   373188 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   475269 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/buildings/OfficeGridStorageSmoothing.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   265862 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/buildings/ShopWithVandBattery.idf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.555013 sinergym-2.3.3/sinergym/data/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)    35474 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    32612 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/variables/5ZoneAutoDXVAV.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    39868 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    42336 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/variables/OfficeGridStorageSmoothing.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/variables/ShopWithVandBattery.rdd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.575013 sinergym-2.3.3/sinergym/data/weather/
+-rw-r--r--   0 runner    (1001) docker     (123)    28629 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1565086 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28503 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1550279 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28704 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1621761 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1553382 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28801 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1558629 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1558423 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1601571 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1637298 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1629153 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1639985 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29614 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1613784 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1624547 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1625209 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.575013 sinergym-2.3.3/sinergym/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/envs/eplus_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.575013 sinergym-2.3.3/sinergym/simulators/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/simulators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/simulators/eplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/simulators/eplus_alpha.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.579013 sinergym-2.3.3/sinergym/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32883 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39674 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.551013 sinergym-2.3.3/sinergym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-04-27 10:29:21.000000 sinergym-2.3.3/sinergym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-27 10:29:21.000000 sinergym-2.3.3/sinergym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:29:21.000000 sinergym-2.3.3/sinergym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-27 10:29:21.000000 sinergym-2.3.3/sinergym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 10:29:21.000000 sinergym-2.3.3/sinergym.egg-info/top_level.txt
```

### Comparing `sinergym-2.3.2/LICENSE` & `sinergym-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/PKG-INFO` & `sinergym-2.3.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 2.3.2
+Version: 2.3.3
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
@@ -19,16 +19,14 @@
 Provides-Extra: gcloud
 Provides-Extra: test
 Provides-Extra: visualization
 License-File: LICENSE
 
 # Sinergym
 
-> :warning: Stable Baselines 3 are working in order to have [gymnasium support](https://github.com/DLR-RM/stable-baselines3/pull/780). It is possible that SB3 algorithms don't work correctly with Sinergym environments temporally.
-
 <div align="center">
   <img src="images/logo.png" width=40%><br><br>
 </div>
 
 </p>
   <p align="center">
     <a href="https://github.com/ugr-sail/sinergym/releases">
@@ -72,19 +70,18 @@
 
 <div align="center">
   <img src="images/general_blueprint.png" width=80%><br><br>
 </div>
 
 The goal of this project is to create an environment following [Gymnasium interface](https://gymnasium.farama.org/), for wrapping simulation engines for building control using **deep reinforcement learning**.
 
-Please, help us to improve by **reporting your questions and issues** [here](https://github.com/ugr-sail/sinergym/issues). It is easy, just 2 clicks using our issue templates (questions, bugs, improvements, etc.). More detailed info on how to report issues [here](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue). 
+Please, help us to improve by **reporting your questions and issues** [here](https://github.com/ugr-sail/sinergym/issues). It is easy, just 2 clicks using our issue templates (questions, bugs, improvements, etc.). More detailed info on how to report issues [here](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue). Don't forget to take a look at [CONTRIBUTING.md](https://github.com/ugr-sail/sinergym/blob/main/CONTRIBUTING.md) if you're thinking about contributing to Sinergym.
 
 The main functionalities of *Sinergym* are the following :
 
-
 -  **Include different simulation engines**. Communication between
    Python and [EnergyPlus](https://energyplus.net/) is established
    using [BCVTB](https://simulationresearch.lbl.gov/bcvtb/FrontPage) middleware.
    Since this tool allows for interacting with several simulation
    engines, more of them (e.g.
    [OpenModelica](https://openmodelica.org/)) could be included in
    the backend while maintaining the Gymnasium API.
@@ -127,175 +124,46 @@
    changes in the model.
 
 -  **Stable Baseline 3 Integration**. Some functionalities like callbacks
    have been customized by our team in order to test easily these environments
    with deep reinforcement learning algorithms. 
    This tool can be used with any other DRL library that supports the * Gymnasium* interface as well.
 
--  **Google Cloud Integration**. Whether you have a Google Cloud account and you want to
-   use your infrastructure with *Sinergym*, we tell you some details about how doing it.
-
--  **Mlflow tracking server**. [Mlflow](https://mlflow.org/) is an open source platform for the machine
-   learning lifecycle. This can be used with Google Cloud remote server (if you have Google Cloud account) 
-   or using local store. This will help you to manage and store your runs and artifacts generated in an orderly
-   manner.
+-  **Weights & Biases tracking and visualization**. One of Sinergym's objectives is to automate
+   and facilitate the training, reproducibility and comparison of agents in simulation-based 
+   building control problems, managing and monitoring model lifecycle from training to deployment. [WandB](https://wandb.ai/site) 
+   is an open-source platform for the machine learning lifecycle helping us with this issue. 
+   It lets us register experiments hyperparameters, visualize data recorded in real-time, 
+   and store artifacts with experiment outputs and best obtained models. 
 
--  **Data Visualization**. Using *Sinergym* logger or Tensorboard server to visualize training and evaluation information
-   in real-time.
+-  **Google Cloud Integration**. Whether you have a Google Cloud account and you want to
+   use your infrastructure with *Sinergym*, we tell you some details about how to do it.
 
 -  **Notebooks examples**. *Sinergym* develops code in notebook format with the purpose of offering use cases to 
    the users in order to help them become familiar with the tool. They are constantly updated, along with the updates 
    and improvements of the tool itself.
 
 -  This project is accompanied by extensive **documentation**, **unit tests** and **github actions workflows** to make 
    *Sinergym* an efficient ecosystem for both understanding and development.
 
 -  Many more!
 
-_This is a work in progress project. Stay tuned for upcoming releases._
+_This is a project in active development. Stay tuned for upcoming releases._
 
 <div align="center">
   <img src="images/operation_diagram.png"><br><br>
 </div>
 
 ## List of available environments
 
 If you would like to see a complete and updated list of our available environments, please visit [our list](https://ugr-sail.github.io/sinergym/compilation/main/pages/environments.html#) in the official *Sinergym* documentation.
 
 ## Installation
 
-For more detailed information, please visit our [documentation](https://ugr-sail.github.io/sinergym/compilation/main/index.html).
-
-### Docker container
-
-We include a **Dockerfile** for installing all dependencies and setting
-up the image for running *Sinergym*. 
-
-By default, Dockerfile will do `pip install -e .[extras]`, if you want to install a different setup, you will have to do in root repository:
-
-```sh
-  $ docker build -t <tag_name> --build-arg SINERGYM_EXTRAS=[<setup_tag(s)>] .
-```
-
-For example, if you want a container with only documentation libraries and testing:
-
-```sh
-  $ docker build -t example1/sinergym:latest --build-arg SINERGYM_EXTRAS=[doc,test] .
-```
-
-On the other hand, if you don't want any extra library, it's necessary to write an empty value like this:
-
-```sh
-  $ docker build -t example1/sinergym:latest --build-arg SINERGYM_EXTRAS= .
-```
-
-:pencil: You can install directly our container from `Docker Hub repository <https://hub.docker.com/repository/docker/sailugr/sinergym>`__, all releases of this project are there.
-
-:pencil: If you use [Visual Studio Code](https://code.visualstudio.com/), by simply opening the root directory and clicking on the pop-up button *Reopen in container*, all the dependencies will be installed automatically and you will be able to run *Sinergym* in an isolated environment. For more information about how to use this functionality, check [VSCode Containers extension documentation](https://code.visualstudio.com/docs/remote/containers).
-
-### Manual installation
-
-To install *Sinergym* manually instead of through the container (not recommended), follow these steps:
-
-#### 1. Configure Python environment
-
-- First, clone this repository:
-
-```sh
-  $ git clone https://github.com/ugr-sail/sinergym.git
-  $ cd sinergym
-```
-
-- Then, it is recommended to create a **virtual environment**. You can do so by:
-
-```sh
-  $ sudo apt-get install python-virtualenv virtualenv
-  $ virtualenv env_sinergym --python=python3.10
-  $ source env_sinergym/bin/activate
-  $ pip install -e .[extras]
-```
-
-- There are other alternatives like **conda environments** (recommended). Conda is very comfortable to use and we have a file to configure it automatically:
-
-```sh
-  $ cd sinergym
-  $ conda env create -f python_environment.yml
-  $ conda activate sinergym
-```
-
-Sinergym has been updating the compatibility with different components, here it is a summary about important versions support:
-
-| **Sinergym version** | **Ubuntu version** | **Python version** | **EnergyPlus version** |
-| -------------------- | ------------------ | ------------------ | ---------------------- |
-| **0.0**              | 18.04 LTS          | 3.6                | 8.3.0                  |
-| **1.1.0**            | 18.04 LTS          | 3.6                | **9.5.0**              |
-| **1.7.0**            | 18.04 LTS          | **3.9**            | 9.5.0                  |
-| **1.9.5**            | **22.04 LTS**      | **3.10**           | 9.5.0                  |
-
-- Now, we have a correct python version with required modules to run *Sinergym*. Let's continue with the rest of the programs that are needed outside of Python to run the simulations:
-
-#### 2. Install EnergyPlus 9.5.0
-
-Install EnergyPlus. Currently it has been update compatibility to 9.5.0 and it has
-been tested, but code may also work with other versions. Other combination may works, but they don't have been tested.
-
-Follow the instructions [here](https://energyplus.net/downloads) and
-install it for Linux (only Ubuntu is supported). Choose any location
-to install the software. Once installed, a folder called
-`Energyplus-9-5-0` should appear in the selected location.
-
-#### 3. Install BCVTB software
-
-Follow the instructions
-[here](https://simulationresearch.lbl.gov/bcvtb/Download) for
-installing BCVTB software. Another option is to copy the `bcvtb`
-folder from [this repository](https://github.com/zhangzhizza/Gym-Eplus/tree/master/eplus_env/envs)
-
-#### 4. Set environment variables
-
-Two environment variables must be set: `EPLUS_PATH` and
-`BCVTB_PATH`, with the locations where EnergyPlus and BCVTB are
-installed respectively.
-
-
-## About Sinergym package
-
-As we have told you in section *Manual Installation*, Python environment can be set up using *python_environment.yml* with *conda*.
-However, we can make an installation using the Github repository itself:
-
-```sh
-  $ cd sinergym
-  $ pip install -e .
-```
-
-Extra libraries can be installed by typing ``pip install -e .[extras]``.
-*extras* include all optional libraries which have been considered in this project such as 
-testing, visualization, Deep Reinforcement Learning, monitoring , etc.
-It's possible to select a subset of these libraries instead of 'extras' tag in which we select all optional libraries, for example:
-
-```sh
-  $ pip install -e .[test,doc]
-```
-
-In order to check all our tag list, visit `setup.py <https://github.com/ugr-sail/sinergym/blob/main/setup.py>`__ in *Sinergym* root repository. In any case, they are not a requirement of the package.
-
-You can also install from `oficial pypi repository <https://pypi.org/project/sinergym/>`__ with last stable version by default:
-
-```sh
-  $ pip install sinergym[extras]
-```
-
-## Check Installation
-
-This project is automatically supervised using tests developed specifically for it. If you want to check *Sinergym* has been installed successfully, run next command:
-
-```sh
-$ pytest tests/ -vv
-```
-Anyway, every time *Sinergym* repository is updated, the tests will run automatically in a remote container using the Dockerfile to build it. `Github Action <https://docs.github.com/es/actions/>`__ will do that job (see our documentation for more information).
+Please, visit [INSTALL.md](https://github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for more information about Sinergym installation.
 
 ## Usage example
 
 If you used our Dockerfile during installation, you should have the *try_env.py* file in your workspace as soon as you enter in. In case you have installed everything on your local machine directly, place it inside our cloned repository. In any case, we start from the point that you have at your disposal a terminal with the appropriate python version and *Sinergym* running correctly.
 
 *Sinergym* uses the standard Gymnasium API. So basic loop should be something like:
 
@@ -319,18 +187,32 @@
 
 Notice that a folder will be created in the working directory after creating the environment. It will contain the EnergyPlus outputs produced during the simulation.
 
 :pencil: For more examples and details, please visit our [usage examples](https://ugr-sail.github.io/sinergym/compilation/main/pages/notebooks/basic_example.html#Basic-example) documentation section.
 
 ## Google Cloud Platform support
 
-Cloud Computing 
-
 For more information about this functionality, please, visit our documentation [here](https://ugr-sail.github.io/sinergym/compilation/main/pages/gcloudAPI.html#sinergym-with-google-cloud).
 
+## Projects using Sinergym
+
+The following are some of the projects benefiting from the advantages of Sinergym:
+
+- [Demosthen/ActiveRL](https://github.com/Demosthen/ActiveRL)
+- [VectorInstitute/HV-Ai-C](https://github.com/VectorInstitute/HV-Ai-C)
+- [rdnfn/beobench](https://github.com/rdnfn/beobench)
+
+:pencil: If you want to appear in this list, do not hesitate to send us a PR and include the following badge in your repository:
+
+<p align="center">
+  <a href="https://github.com/ugr-sail/sinergym">
+      <img src="https://img.shields.io/badge/Powered%20by-Sinergym%20%E2%86%92-gray.svg?colorA=00BABF&colorB=4BF2F7&style=for-the-badge"/>
+  </a>
+</p>
+
 ## Citing Sinergym
 
 If you use *Sinergym* in your work, please cite our [paper](https://dl.acm.org/doi/abs/10.1145/3486611.3488729):
 
 ```bibtex
 @inproceedings{2021sinergym,
     title={Sinergym: A Building Simulation and Control Framework for Training Reinforcement Learning Agents},
```

#### html2text {}

```diff
@@ -1,23 +1,20 @@
-Metadata-Version: 2.1 Name: sinergym Version: 2.3.2 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 2.3.3 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
 Python :: 3.10 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 Provides-Extra: DRL Provides-Extra: doc Provides-Extra: extras Provides-Extra:
 gcloud Provides-Extra: test Provides-Extra: visualization License-File: LICENSE
-# Sinergym > :warning: Stable Baselines 3 are working in order to have
-[gymnasium support](https://github.com/DLR-RM/stable-baselines3/pull/780). It
-is possible that SB3 algorithms don't work correctly with Sinergym environments
-temporally.
+# Sinergym
                                [images/logo.png]
 
  [Github_latest_release] [Github_last_commit] [Pypi_version] [Pypi_downloads]
  [https://codecov.io/gh/ugr-sail/sinergym/branch/main/graph/badge.svg] [GitHub
   Contributors] [Github_issues] [GitHub_pull_requests] [Github_License] [Pypi
                                Python_version]
 
@@ -29,19 +26,21 @@
 The goal of this project is to create an environment following [Gymnasium
 interface](https://gymnasium.farama.org/), for wrapping simulation engines for
 building control using **deep reinforcement learning**. Please, help us to
 improve by **reporting your questions and issues** [here](https://github.com/
 ugr-sail/sinergym/issues). It is easy, just 2 clicks using our issue templates
 (questions, bugs, improvements, etc.). More detailed info on how to report
 issues [here](https://docs.github.com/en/issues/tracking-your-work-with-issues/
-creating-an-issue). The main functionalities of *Sinergym* are the following :
-- **Include different simulation engines**. Communication between Python and
-[EnergyPlus](https://energyplus.net/) is established using [BCVTB](https://
-simulationresearch.lbl.gov/bcvtb/FrontPage) middleware. Since this tool allows
-for interacting with several simulation engines, more of them (e.g.
+creating-an-issue). Don't forget to take a look at [CONTRIBUTING.md](https://
+github.com/ugr-sail/sinergym/blob/main/CONTRIBUTING.md) if you're thinking
+about contributing to Sinergym. The main functionalities of *Sinergym* are the
+following : - **Include different simulation engines**. Communication between
+Python and [EnergyPlus](https://energyplus.net/) is established using [BCVTB]
+(https://simulationresearch.lbl.gov/bcvtb/FrontPage) middleware. Since this
+tool allows for interacting with several simulation engines, more of them (e.g.
 [OpenModelica](https://openmodelica.org/)) could be included in the backend
 while maintaining the Gymnasium API. - **Benchmark environments**. Similarly to
 *Atari* or *Mujoco* environments for RL community, we are designing a set of
 environments for benchmarking and testing deep RL algorithms. These
 environments may include different buildings, weathers, action/observation
 spaces, function rewards, etc. - **Customizable environments**. We aim to
 provide a package that allows to modify experimental settings in an easy
@@ -73,131 +72,70 @@
 building and, then, control them with an external interface from an agent. To
 do this, users will make an **action definition** in which it is indicated
 which default controllers they want to replace in a specific format and
 *Sinergym* will take care of the relevant internal changes in the model. -
 **Stable Baseline 3 Integration**. Some functionalities like callbacks have
 been customized by our team in order to test easily these environments with
 deep reinforcement learning algorithms. This tool can be used with any other
-DRL library that supports the * Gymnasium* interface as well. - **Google Cloud
-Integration**. Whether you have a Google Cloud account and you want to use your
-infrastructure with *Sinergym*, we tell you some details about how doing it. -
-**Mlflow tracking server**. [Mlflow](https://mlflow.org/) is an open source
-platform for the machine learning lifecycle. This can be used with Google Cloud
-remote server (if you have Google Cloud account) or using local store. This
-will help you to manage and store your runs and artifacts generated in an
-orderly manner. - **Data Visualization**. Using *Sinergym* logger or
-Tensorboard server to visualize training and evaluation information in real-
-time. - **Notebooks examples**. *Sinergym* develops code in notebook format
-with the purpose of offering use cases to the users in order to help them
-become familiar with the tool. They are constantly updated, along with the
-updates and improvements of the tool itself. - This project is accompanied by
-extensive **documentation**, **unit tests** and **github actions workflows** to
-make *Sinergym* an efficient ecosystem for both understanding and development.
-- Many more! _This is a work in progress project. Stay tuned for upcoming
-releases._
+DRL library that supports the * Gymnasium* interface as well. - **Weights &
+Biases tracking and visualization**. One of Sinergym's objectives is to
+automate and facilitate the training, reproducibility and comparison of agents
+in simulation-based building control problems, managing and monitoring model
+lifecycle from training to deployment. [WandB](https://wandb.ai/site) is an
+open-source platform for the machine learning lifecycle helping us with this
+issue. It lets us register experiments hyperparameters, visualize data recorded
+in real-time, and store artifacts with experiment outputs and best obtained
+models. - **Google Cloud Integration**. Whether you have a Google Cloud account
+and you want to use your infrastructure with *Sinergym*, we tell you some
+details about how to do it. - **Notebooks examples**. *Sinergym* develops code
+in notebook format with the purpose of offering use cases to the users in order
+to help them become familiar with the tool. They are constantly updated, along
+with the updates and improvements of the tool itself. - This project is
+accompanied by extensive **documentation**, **unit tests** and **github actions
+workflows** to make *Sinergym* an efficient ecosystem for both understanding
+and development. - Many more! _This is a project in active development. Stay
+tuned for upcoming releases._
                         [images/operation_diagram.png]
 
 ## List of available environments If you would like to see a complete and
 updated list of our available environments, please visit [our list](https://
 ugr-sail.github.io/sinergym/compilation/main/pages/environments.html#) in the
-official *Sinergym* documentation. ## Installation For more detailed
-information, please visit our [documentation](https://ugr-sail.github.io/
-sinergym/compilation/main/index.html). ### Docker container We include a
-**Dockerfile** for installing all dependencies and setting up the image for
-running *Sinergym*. By default, Dockerfile will do `pip install -e .[extras]`,
-if you want to install a different setup, you will have to do in root
-repository: ```sh $ docker build -t  --build-arg SINERGYM_EXTRAS=[
-s)>] . ``` For example, if you want a container with only documentation
-libraries and testing: ```sh $ docker build -t example1/sinergym:latest --
-build-arg SINERGYM_EXTRAS=[doc,test] . ``` On the other hand, if you don't want
-any extra library, it's necessary to write an empty value like this: ```sh $
-docker build -t example1/sinergym:latest --build-arg SINERGYM_EXTRAS= . ``` :
-pencil: You can install directly our container from `Docker Hub repository
-hub.docker.com/repository/docker/sailugr/sinergym>`__, all releases of this
-project are there. :pencil: If you use [Visual Studio Code](https://
-code.visualstudio.com/), by simply opening the root directory and clicking on
-the pop-up button *Reopen in container*, all the dependencies will be installed
-automatically and you will be able to run *Sinergym* in an isolated
-environment. For more information about how to use this functionality, check
-[VSCode Containers extension documentation](https://code.visualstudio.com/docs/
-remote/containers). ### Manual installation To install *Sinergym* manually
-instead of through the container (not recommended), follow these steps: #### 1.
-Configure Python environment - First, clone this repository: ```sh $ git clone
-https://github.com/ugr-sail/sinergym.git $ cd sinergym ``` - Then, it is
-recommended to create a **virtual environment**. You can do so by: ```sh $ sudo
-apt-get install python-virtualenv virtualenv $ virtualenv env_sinergym --
-python=python3.10 $ source env_sinergym/bin/activate $ pip install -e .[extras]
-``` - There are other alternatives like **conda environments** (recommended).
-Conda is very comfortable to use and we have a file to configure it
-automatically: ```sh $ cd sinergym $ conda env create -f python_environment.yml
-$ conda activate sinergym ``` Sinergym has been updating the compatibility with
-different components, here it is a summary about important versions support: |
-**Sinergym version** | **Ubuntu version** | **Python version** | **EnergyPlus
-version** | | -------------------- | ------------------ | ------------------ |
----------------------- | | **0.0** | 18.04 LTS | 3.6 | 8.3.0 | | **1.1.0** |
-18.04 LTS | 3.6 | **9.5.0** | | **1.7.0** | 18.04 LTS | **3.9** | 9.5.0 | |
-**1.9.5** | **22.04 LTS** | **3.10** | 9.5.0 | - Now, we have a correct python
-version with required modules to run *Sinergym*. Let's continue with the rest
-of the programs that are needed outside of Python to run the simulations: ####
-2. Install EnergyPlus 9.5.0 Install EnergyPlus. Currently it has been update
-compatibility to 9.5.0 and it has been tested, but code may also work with
-other versions. Other combination may works, but they don't have been tested.
-Follow the instructions [here](https://energyplus.net/downloads) and install it
-for Linux (only Ubuntu is supported). Choose any location to install the
-software. Once installed, a folder called `Energyplus-9-5-0` should appear in
-the selected location. #### 3. Install BCVTB software Follow the instructions
-[here](https://simulationresearch.lbl.gov/bcvtb/Download) for installing BCVTB
-software. Another option is to copy the `bcvtb` folder from [this repository]
-(https://github.com/zhangzhizza/Gym-Eplus/tree/master/eplus_env/envs) #### 4.
-Set environment variables Two environment variables must be set: `EPLUS_PATH`
-and `BCVTB_PATH`, with the locations where EnergyPlus and BCVTB are installed
-respectively. ## About Sinergym package As we have told you in section *Manual
-Installation*, Python environment can be set up using *python_environment.yml*
-with *conda*. However, we can make an installation using the Github repository
-itself: ```sh $ cd sinergym $ pip install -e . ``` Extra libraries can be
-installed by typing ``pip install -e .[extras]``. *extras* include all optional
-libraries which have been considered in this project such as testing,
-visualization, Deep Reinforcement Learning, monitoring , etc. It's possible to
-select a subset of these libraries instead of 'extras' tag in which we select
-all optional libraries, for example: ```sh $ pip install -e .[test,doc] ``` In
-order to check all our tag list, visit `setup.py
-github.com/ugr-sail/sinergym/blob/main/setup.py>`__ in *Sinergym* root
-repository. In any case, they are not a requirement of the package. You can
-also install from `oficial pypi repository
-pypi.org/project/sinergym/>`__ with last stable version by default: ```sh $ pip
-install sinergym[extras] ``` ## Check Installation This project is
-automatically supervised using tests developed specifically for it. If you want
-to check *Sinergym* has been installed successfully, run next command: ```sh $
-pytest tests/ -vv ``` Anyway, every time *Sinergym* repository is updated, the
-tests will run automatically in a remote container using the Dockerfile to
-build it. `Github Action
-docs.github.com/es/actions/>`__ will do that job (see our documentation for
-more information). ## Usage example If you used our Dockerfile during
-installation, you should have the *try_env.py* file in your workspace as soon
-as you enter in. In case you have installed everything on your local machine
-directly, place it inside our cloned repository. In any case, we start from the
-point that you have at your disposal a terminal with the appropriate python
-version and *Sinergym* running correctly. *Sinergym* uses the standard
-Gymnasium API. So basic loop should be something like: ```python import
-gymnasium as gym import sinergym # Create the environment env = gym.make
-('Eplus-datacenter-mixed-continuous-stochastic-v1') # Initialize the episode
-obs, info = env.reset() terminated = False R = 0.0 while not terminated: a =
-env.action_space.sample() # random action selection obs, reward, terminated,
-truncated, info = env.step(a) # get new observation and reward R += reward
-print('Total reward for the episode: %.4f' % R) env.close() ``` Notice that a
-folder will be created in the working directory after creating the environment.
-It will contain the EnergyPlus outputs produced during the simulation. :pencil:
-For more examples and details, please visit our [usage examples](https://ugr-
-sail.github.io/sinergym/compilation/main/pages/notebooks/
-basic_example.html#Basic-example) documentation section. ## Google Cloud
-Platform support Cloud Computing For more information about this functionality,
-please, visit our documentation [here](https://ugr-sail.github.io/sinergym/
-compilation/main/pages/gcloudAPI.html#sinergym-with-google-cloud). ## Citing
-Sinergym If you use *Sinergym* in your work, please cite our [paper](https://
-dl.acm.org/doi/abs/10.1145/3486611.3488729): ```bibtex @inproceedings
+official *Sinergym* documentation. ## Installation Please, visit [INSTALL.md]
+(https://github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for more
+information about Sinergym installation. ## Usage example If you used our
+Dockerfile during installation, you should have the *try_env.py* file in your
+workspace as soon as you enter in. In case you have installed everything on
+your local machine directly, place it inside our cloned repository. In any
+case, we start from the point that you have at your disposal a terminal with
+the appropriate python version and *Sinergym* running correctly. *Sinergym*
+uses the standard Gymnasium API. So basic loop should be something like:
+```python import gymnasium as gym import sinergym # Create the environment env
+= gym.make('Eplus-datacenter-mixed-continuous-stochastic-v1') # Initialize the
+episode obs, info = env.reset() terminated = False R = 0.0 while not
+terminated: a = env.action_space.sample() # random action selection obs,
+reward, terminated, truncated, info = env.step(a) # get new observation and
+reward R += reward print('Total reward for the episode: %.4f' % R) env.close()
+``` Notice that a folder will be created in the working directory after
+creating the environment. It will contain the EnergyPlus outputs produced
+during the simulation. :pencil: For more examples and details, please visit our
+[usage examples](https://ugr-sail.github.io/sinergym/compilation/main/pages/
+notebooks/basic_example.html#Basic-example) documentation section. ## Google
+Cloud Platform support For more information about this functionality, please,
+visit our documentation [here](https://ugr-sail.github.io/sinergym/compilation/
+main/pages/gcloudAPI.html#sinergym-with-google-cloud). ## Projects using
+Sinergym The following are some of the projects benefiting from the advantages
+of Sinergym: - [Demosthen/ActiveRL](https://github.com/Demosthen/ActiveRL) -
+[VectorInstitute/HV-Ai-C](https://github.com/VectorInstitute/HV-Ai-C) - [rdnfn/
+beobench](https://github.com/rdnfn/beobench) :pencil: If you want to appear in
+this list, do not hesitate to send us a PR and include the following badge in
+your repository:
+       [https://img.shields.io/badge/Powered%20by-Sinergym%20%E2%86%92-
+           gray.svg?colorA=00BABF&colorB=4BF2F7&style=for-the-badge]
+## Citing Sinergym If you use *Sinergym* in your work, please cite our [paper]
+(https://dl.acm.org/doi/abs/10.1145/3486611.3488729): ```bibtex @inproceedings
 {2021sinergym, title={Sinergym: A Building Simulation and Control Framework for
 Training Reinforcement Learning Agents}, author={JimÃ©nez-Raboso, Javier and
 Campoy-Nieves, Alejandro and Manjavacas-Lucas, Antonio and GÃ³mez-Romero, Juan
 and Molina-Solana, Miguel}, year={2021}, isbn = {9781450391146}, publisher =
 {Association for Computing Machinery}, address = {New York, NY, USA}, url =
 {https://doi.org/10.1145/3486611.3488729}, doi = {10.1145/3486611.3488729},
 booktitle = {Proceedings of the 8th ACM International Conference on Systems for
```

### Comparing `sinergym-2.3.2/README.md` & `sinergym-2.3.3/sinergym.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,31 @@
-# Sinergym
+Metadata-Version: 2.1
+Name: sinergym
+Version: 2.3.3
+Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
+Home-page: https://github.com/ugr-sail/sinergym
+Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
+Author-email: alejandroac79@gmail.com
+License: MIT
+Keywords: control reinforcement-learning buildings reinforcement-learning-environments
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: DRL
+Provides-Extra: doc
+Provides-Extra: extras
+Provides-Extra: gcloud
+Provides-Extra: test
+Provides-Extra: visualization
+License-File: LICENSE
 
-> :warning: Stable Baselines 3 are working in order to have [gymnasium support](https://github.com/DLR-RM/stable-baselines3/pull/780). It is possible that SB3 algorithms don't work correctly with Sinergym environments temporally.
+# Sinergym
 
 <div align="center">
   <img src="images/logo.png" width=40%><br><br>
 </div>
 
 </p>
   <p align="center">
@@ -49,19 +70,18 @@
 
 <div align="center">
   <img src="images/general_blueprint.png" width=80%><br><br>
 </div>
 
 The goal of this project is to create an environment following [Gymnasium interface](https://gymnasium.farama.org/), for wrapping simulation engines for building control using **deep reinforcement learning**.
 
-Please, help us to improve by **reporting your questions and issues** [here](https://github.com/ugr-sail/sinergym/issues). It is easy, just 2 clicks using our issue templates (questions, bugs, improvements, etc.). More detailed info on how to report issues [here](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue). 
+Please, help us to improve by **reporting your questions and issues** [here](https://github.com/ugr-sail/sinergym/issues). It is easy, just 2 clicks using our issue templates (questions, bugs, improvements, etc.). More detailed info on how to report issues [here](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue). Don't forget to take a look at [CONTRIBUTING.md](https://github.com/ugr-sail/sinergym/blob/main/CONTRIBUTING.md) if you're thinking about contributing to Sinergym.
 
 The main functionalities of *Sinergym* are the following :
 
-
 -  **Include different simulation engines**. Communication between
    Python and [EnergyPlus](https://energyplus.net/) is established
    using [BCVTB](https://simulationresearch.lbl.gov/bcvtb/FrontPage) middleware.
    Since this tool allows for interacting with several simulation
    engines, more of them (e.g.
    [OpenModelica](https://openmodelica.org/)) could be included in
    the backend while maintaining the Gymnasium API.
@@ -104,175 +124,46 @@
    changes in the model.
 
 -  **Stable Baseline 3 Integration**. Some functionalities like callbacks
    have been customized by our team in order to test easily these environments
    with deep reinforcement learning algorithms. 
    This tool can be used with any other DRL library that supports the * Gymnasium* interface as well.
 
--  **Google Cloud Integration**. Whether you have a Google Cloud account and you want to
-   use your infrastructure with *Sinergym*, we tell you some details about how doing it.
-
--  **Mlflow tracking server**. [Mlflow](https://mlflow.org/) is an open source platform for the machine
-   learning lifecycle. This can be used with Google Cloud remote server (if you have Google Cloud account) 
-   or using local store. This will help you to manage and store your runs and artifacts generated in an orderly
-   manner.
+-  **Weights & Biases tracking and visualization**. One of Sinergym's objectives is to automate
+   and facilitate the training, reproducibility and comparison of agents in simulation-based 
+   building control problems, managing and monitoring model lifecycle from training to deployment. [WandB](https://wandb.ai/site) 
+   is an open-source platform for the machine learning lifecycle helping us with this issue. 
+   It lets us register experiments hyperparameters, visualize data recorded in real-time, 
+   and store artifacts with experiment outputs and best obtained models. 
 
--  **Data Visualization**. Using *Sinergym* logger or Tensorboard server to visualize training and evaluation information
-   in real-time.
+-  **Google Cloud Integration**. Whether you have a Google Cloud account and you want to
+   use your infrastructure with *Sinergym*, we tell you some details about how to do it.
 
 -  **Notebooks examples**. *Sinergym* develops code in notebook format with the purpose of offering use cases to 
    the users in order to help them become familiar with the tool. They are constantly updated, along with the updates 
    and improvements of the tool itself.
 
 -  This project is accompanied by extensive **documentation**, **unit tests** and **github actions workflows** to make 
    *Sinergym* an efficient ecosystem for both understanding and development.
 
 -  Many more!
 
-_This is a work in progress project. Stay tuned for upcoming releases._
+_This is a project in active development. Stay tuned for upcoming releases._
 
 <div align="center">
   <img src="images/operation_diagram.png"><br><br>
 </div>
 
 ## List of available environments
 
 If you would like to see a complete and updated list of our available environments, please visit [our list](https://ugr-sail.github.io/sinergym/compilation/main/pages/environments.html#) in the official *Sinergym* documentation.
 
 ## Installation
 
-For more detailed information, please visit our [documentation](https://ugr-sail.github.io/sinergym/compilation/main/index.html).
-
-### Docker container
-
-We include a **Dockerfile** for installing all dependencies and setting
-up the image for running *Sinergym*. 
-
-By default, Dockerfile will do `pip install -e .[extras]`, if you want to install a different setup, you will have to do in root repository:
-
-```sh
-  $ docker build -t <tag_name> --build-arg SINERGYM_EXTRAS=[<setup_tag(s)>] .
-```
-
-For example, if you want a container with only documentation libraries and testing:
-
-```sh
-  $ docker build -t example1/sinergym:latest --build-arg SINERGYM_EXTRAS=[doc,test] .
-```
-
-On the other hand, if you don't want any extra library, it's necessary to write an empty value like this:
-
-```sh
-  $ docker build -t example1/sinergym:latest --build-arg SINERGYM_EXTRAS= .
-```
-
-:pencil: You can install directly our container from `Docker Hub repository <https://hub.docker.com/repository/docker/sailugr/sinergym>`__, all releases of this project are there.
-
-:pencil: If you use [Visual Studio Code](https://code.visualstudio.com/), by simply opening the root directory and clicking on the pop-up button *Reopen in container*, all the dependencies will be installed automatically and you will be able to run *Sinergym* in an isolated environment. For more information about how to use this functionality, check [VSCode Containers extension documentation](https://code.visualstudio.com/docs/remote/containers).
-
-### Manual installation
-
-To install *Sinergym* manually instead of through the container (not recommended), follow these steps:
-
-#### 1. Configure Python environment
-
-- First, clone this repository:
-
-```sh
-  $ git clone https://github.com/ugr-sail/sinergym.git
-  $ cd sinergym
-```
-
-- Then, it is recommended to create a **virtual environment**. You can do so by:
-
-```sh
-  $ sudo apt-get install python-virtualenv virtualenv
-  $ virtualenv env_sinergym --python=python3.10
-  $ source env_sinergym/bin/activate
-  $ pip install -e .[extras]
-```
-
-- There are other alternatives like **conda environments** (recommended). Conda is very comfortable to use and we have a file to configure it automatically:
-
-```sh
-  $ cd sinergym
-  $ conda env create -f python_environment.yml
-  $ conda activate sinergym
-```
-
-Sinergym has been updating the compatibility with different components, here it is a summary about important versions support:
-
-| **Sinergym version** | **Ubuntu version** | **Python version** | **EnergyPlus version** |
-| -------------------- | ------------------ | ------------------ | ---------------------- |
-| **0.0**              | 18.04 LTS          | 3.6                | 8.3.0                  |
-| **1.1.0**            | 18.04 LTS          | 3.6                | **9.5.0**              |
-| **1.7.0**            | 18.04 LTS          | **3.9**            | 9.5.0                  |
-| **1.9.5**            | **22.04 LTS**      | **3.10**           | 9.5.0                  |
-
-- Now, we have a correct python version with required modules to run *Sinergym*. Let's continue with the rest of the programs that are needed outside of Python to run the simulations:
-
-#### 2. Install EnergyPlus 9.5.0
-
-Install EnergyPlus. Currently it has been update compatibility to 9.5.0 and it has
-been tested, but code may also work with other versions. Other combination may works, but they don't have been tested.
-
-Follow the instructions [here](https://energyplus.net/downloads) and
-install it for Linux (only Ubuntu is supported). Choose any location
-to install the software. Once installed, a folder called
-`Energyplus-9-5-0` should appear in the selected location.
-
-#### 3. Install BCVTB software
-
-Follow the instructions
-[here](https://simulationresearch.lbl.gov/bcvtb/Download) for
-installing BCVTB software. Another option is to copy the `bcvtb`
-folder from [this repository](https://github.com/zhangzhizza/Gym-Eplus/tree/master/eplus_env/envs)
-
-#### 4. Set environment variables
-
-Two environment variables must be set: `EPLUS_PATH` and
-`BCVTB_PATH`, with the locations where EnergyPlus and BCVTB are
-installed respectively.
-
-
-## About Sinergym package
-
-As we have told you in section *Manual Installation*, Python environment can be set up using *python_environment.yml* with *conda*.
-However, we can make an installation using the Github repository itself:
-
-```sh
-  $ cd sinergym
-  $ pip install -e .
-```
-
-Extra libraries can be installed by typing ``pip install -e .[extras]``.
-*extras* include all optional libraries which have been considered in this project such as 
-testing, visualization, Deep Reinforcement Learning, monitoring , etc.
-It's possible to select a subset of these libraries instead of 'extras' tag in which we select all optional libraries, for example:
-
-```sh
-  $ pip install -e .[test,doc]
-```
-
-In order to check all our tag list, visit `setup.py <https://github.com/ugr-sail/sinergym/blob/main/setup.py>`__ in *Sinergym* root repository. In any case, they are not a requirement of the package.
-
-You can also install from `oficial pypi repository <https://pypi.org/project/sinergym/>`__ with last stable version by default:
-
-```sh
-  $ pip install sinergym[extras]
-```
-
-## Check Installation
-
-This project is automatically supervised using tests developed specifically for it. If you want to check *Sinergym* has been installed successfully, run next command:
-
-```sh
-$ pytest tests/ -vv
-```
-Anyway, every time *Sinergym* repository is updated, the tests will run automatically in a remote container using the Dockerfile to build it. `Github Action <https://docs.github.com/es/actions/>`__ will do that job (see our documentation for more information).
+Please, visit [INSTALL.md](https://github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for more information about Sinergym installation.
 
 ## Usage example
 
 If you used our Dockerfile during installation, you should have the *try_env.py* file in your workspace as soon as you enter in. In case you have installed everything on your local machine directly, place it inside our cloned repository. In any case, we start from the point that you have at your disposal a terminal with the appropriate python version and *Sinergym* running correctly.
 
 *Sinergym* uses the standard Gymnasium API. So basic loop should be something like:
 
@@ -296,18 +187,32 @@
 
 Notice that a folder will be created in the working directory after creating the environment. It will contain the EnergyPlus outputs produced during the simulation.
 
 :pencil: For more examples and details, please visit our [usage examples](https://ugr-sail.github.io/sinergym/compilation/main/pages/notebooks/basic_example.html#Basic-example) documentation section.
 
 ## Google Cloud Platform support
 
-Cloud Computing 
-
 For more information about this functionality, please, visit our documentation [here](https://ugr-sail.github.io/sinergym/compilation/main/pages/gcloudAPI.html#sinergym-with-google-cloud).
 
+## Projects using Sinergym
+
+The following are some of the projects benefiting from the advantages of Sinergym:
+
+- [Demosthen/ActiveRL](https://github.com/Demosthen/ActiveRL)
+- [VectorInstitute/HV-Ai-C](https://github.com/VectorInstitute/HV-Ai-C)
+- [rdnfn/beobench](https://github.com/rdnfn/beobench)
+
+:pencil: If you want to appear in this list, do not hesitate to send us a PR and include the following badge in your repository:
+
+<p align="center">
+  <a href="https://github.com/ugr-sail/sinergym">
+      <img src="https://img.shields.io/badge/Powered%20by-Sinergym%20%E2%86%92-gray.svg?colorA=00BABF&colorB=4BF2F7&style=for-the-badge"/>
+  </a>
+</p>
+
 ## Citing Sinergym
 
 If you use *Sinergym* in your work, please cite our [paper](https://dl.acm.org/doi/abs/10.1145/3486611.3488729):
 
 ```bibtex
 @inproceedings{2021sinergym,
     title={Sinergym: A Building Simulation and Control Framework for Training Reinforcement Learning Agents}, 
@@ -319,7 +224,9 @@
     url = {https://doi.org/10.1145/3486611.3488729},
     doi = {10.1145/3486611.3488729},
     booktitle = {Proceedings of the 8th ACM International Conference on Systems for Energy-Efficient Buildings, Cities, and Transportation},
     pages = {319–323},
     numpages = {5},
 }
 ```
+
+
```

#### html2text {}

```diff
@@ -1,11 +1,20 @@
-# Sinergym > :warning: Stable Baselines 3 are working in order to have
-[gymnasium support](https://github.com/DLR-RM/stable-baselines3/pull/780). It
-is possible that SB3 algorithms don't work correctly with Sinergym environments
-temporally.
+Metadata-Version: 2.1 Name: sinergym Version: 2.3.3 Summary: The goal of
+sinergym is to create an environment following OpenAI Gym interface for
+wrapping simulation engines for building control using deep reinforcement
+learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
+J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
+alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
+buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
+Development Status :: 5 - Production/Stable Classifier: Programming Language ::
+Python :: 3.10 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Description-Content-Type: text/markdown
+Provides-Extra: DRL Provides-Extra: doc Provides-Extra: extras Provides-Extra:
+gcloud Provides-Extra: test Provides-Extra: visualization License-File: LICENSE
+# Sinergym
                                [images/logo.png]
 
  [Github_latest_release] [Github_last_commit] [Pypi_version] [Pypi_downloads]
  [https://codecov.io/gh/ugr-sail/sinergym/branch/main/graph/badge.svg] [GitHub
   Contributors] [Github_issues] [GitHub_pull_requests] [Github_License] [Pypi
                                Python_version]
 
@@ -17,19 +26,21 @@
 The goal of this project is to create an environment following [Gymnasium
 interface](https://gymnasium.farama.org/), for wrapping simulation engines for
 building control using **deep reinforcement learning**. Please, help us to
 improve by **reporting your questions and issues** [here](https://github.com/
 ugr-sail/sinergym/issues). It is easy, just 2 clicks using our issue templates
 (questions, bugs, improvements, etc.). More detailed info on how to report
 issues [here](https://docs.github.com/en/issues/tracking-your-work-with-issues/
-creating-an-issue). The main functionalities of *Sinergym* are the following :
-- **Include different simulation engines**. Communication between Python and
-[EnergyPlus](https://energyplus.net/) is established using [BCVTB](https://
-simulationresearch.lbl.gov/bcvtb/FrontPage) middleware. Since this tool allows
-for interacting with several simulation engines, more of them (e.g.
+creating-an-issue). Don't forget to take a look at [CONTRIBUTING.md](https://
+github.com/ugr-sail/sinergym/blob/main/CONTRIBUTING.md) if you're thinking
+about contributing to Sinergym. The main functionalities of *Sinergym* are the
+following : - **Include different simulation engines**. Communication between
+Python and [EnergyPlus](https://energyplus.net/) is established using [BCVTB]
+(https://simulationresearch.lbl.gov/bcvtb/FrontPage) middleware. Since this
+tool allows for interacting with several simulation engines, more of them (e.g.
 [OpenModelica](https://openmodelica.org/)) could be included in the backend
 while maintaining the Gymnasium API. - **Benchmark environments**. Similarly to
 *Atari* or *Mujoco* environments for RL community, we are designing a set of
 environments for benchmarking and testing deep RL algorithms. These
 environments may include different buildings, weathers, action/observation
 spaces, function rewards, etc. - **Customizable environments**. We aim to
 provide a package that allows to modify experimental settings in an easy
@@ -61,131 +72,70 @@
 building and, then, control them with an external interface from an agent. To
 do this, users will make an **action definition** in which it is indicated
 which default controllers they want to replace in a specific format and
 *Sinergym* will take care of the relevant internal changes in the model. -
 **Stable Baseline 3 Integration**. Some functionalities like callbacks have
 been customized by our team in order to test easily these environments with
 deep reinforcement learning algorithms. This tool can be used with any other
-DRL library that supports the * Gymnasium* interface as well. - **Google Cloud
-Integration**. Whether you have a Google Cloud account and you want to use your
-infrastructure with *Sinergym*, we tell you some details about how doing it. -
-**Mlflow tracking server**. [Mlflow](https://mlflow.org/) is an open source
-platform for the machine learning lifecycle. This can be used with Google Cloud
-remote server (if you have Google Cloud account) or using local store. This
-will help you to manage and store your runs and artifacts generated in an
-orderly manner. - **Data Visualization**. Using *Sinergym* logger or
-Tensorboard server to visualize training and evaluation information in real-
-time. - **Notebooks examples**. *Sinergym* develops code in notebook format
-with the purpose of offering use cases to the users in order to help them
-become familiar with the tool. They are constantly updated, along with the
-updates and improvements of the tool itself. - This project is accompanied by
-extensive **documentation**, **unit tests** and **github actions workflows** to
-make *Sinergym* an efficient ecosystem for both understanding and development.
-- Many more! _This is a work in progress project. Stay tuned for upcoming
-releases._
+DRL library that supports the * Gymnasium* interface as well. - **Weights &
+Biases tracking and visualization**. One of Sinergym's objectives is to
+automate and facilitate the training, reproducibility and comparison of agents
+in simulation-based building control problems, managing and monitoring model
+lifecycle from training to deployment. [WandB](https://wandb.ai/site) is an
+open-source platform for the machine learning lifecycle helping us with this
+issue. It lets us register experiments hyperparameters, visualize data recorded
+in real-time, and store artifacts with experiment outputs and best obtained
+models. - **Google Cloud Integration**. Whether you have a Google Cloud account
+and you want to use your infrastructure with *Sinergym*, we tell you some
+details about how to do it. - **Notebooks examples**. *Sinergym* develops code
+in notebook format with the purpose of offering use cases to the users in order
+to help them become familiar with the tool. They are constantly updated, along
+with the updates and improvements of the tool itself. - This project is
+accompanied by extensive **documentation**, **unit tests** and **github actions
+workflows** to make *Sinergym* an efficient ecosystem for both understanding
+and development. - Many more! _This is a project in active development. Stay
+tuned for upcoming releases._
                         [images/operation_diagram.png]
 
 ## List of available environments If you would like to see a complete and
 updated list of our available environments, please visit [our list](https://
 ugr-sail.github.io/sinergym/compilation/main/pages/environments.html#) in the
-official *Sinergym* documentation. ## Installation For more detailed
-information, please visit our [documentation](https://ugr-sail.github.io/
-sinergym/compilation/main/index.html). ### Docker container We include a
-**Dockerfile** for installing all dependencies and setting up the image for
-running *Sinergym*. By default, Dockerfile will do `pip install -e .[extras]`,
-if you want to install a different setup, you will have to do in root
-repository: ```sh $ docker build -t  --build-arg SINERGYM_EXTRAS=[
-s)>] . ``` For example, if you want a container with only documentation
-libraries and testing: ```sh $ docker build -t example1/sinergym:latest --
-build-arg SINERGYM_EXTRAS=[doc,test] . ``` On the other hand, if you don't want
-any extra library, it's necessary to write an empty value like this: ```sh $
-docker build -t example1/sinergym:latest --build-arg SINERGYM_EXTRAS= . ``` :
-pencil: You can install directly our container from `Docker Hub repository
-hub.docker.com/repository/docker/sailugr/sinergym>`__, all releases of this
-project are there. :pencil: If you use [Visual Studio Code](https://
-code.visualstudio.com/), by simply opening the root directory and clicking on
-the pop-up button *Reopen in container*, all the dependencies will be installed
-automatically and you will be able to run *Sinergym* in an isolated
-environment. For more information about how to use this functionality, check
-[VSCode Containers extension documentation](https://code.visualstudio.com/docs/
-remote/containers). ### Manual installation To install *Sinergym* manually
-instead of through the container (not recommended), follow these steps: #### 1.
-Configure Python environment - First, clone this repository: ```sh $ git clone
-https://github.com/ugr-sail/sinergym.git $ cd sinergym ``` - Then, it is
-recommended to create a **virtual environment**. You can do so by: ```sh $ sudo
-apt-get install python-virtualenv virtualenv $ virtualenv env_sinergym --
-python=python3.10 $ source env_sinergym/bin/activate $ pip install -e .[extras]
-``` - There are other alternatives like **conda environments** (recommended).
-Conda is very comfortable to use and we have a file to configure it
-automatically: ```sh $ cd sinergym $ conda env create -f python_environment.yml
-$ conda activate sinergym ``` Sinergym has been updating the compatibility with
-different components, here it is a summary about important versions support: |
-**Sinergym version** | **Ubuntu version** | **Python version** | **EnergyPlus
-version** | | -------------------- | ------------------ | ------------------ |
----------------------- | | **0.0** | 18.04 LTS | 3.6 | 8.3.0 | | **1.1.0** |
-18.04 LTS | 3.6 | **9.5.0** | | **1.7.0** | 18.04 LTS | **3.9** | 9.5.0 | |
-**1.9.5** | **22.04 LTS** | **3.10** | 9.5.0 | - Now, we have a correct python
-version with required modules to run *Sinergym*. Let's continue with the rest
-of the programs that are needed outside of Python to run the simulations: ####
-2. Install EnergyPlus 9.5.0 Install EnergyPlus. Currently it has been update
-compatibility to 9.5.0 and it has been tested, but code may also work with
-other versions. Other combination may works, but they don't have been tested.
-Follow the instructions [here](https://energyplus.net/downloads) and install it
-for Linux (only Ubuntu is supported). Choose any location to install the
-software. Once installed, a folder called `Energyplus-9-5-0` should appear in
-the selected location. #### 3. Install BCVTB software Follow the instructions
-[here](https://simulationresearch.lbl.gov/bcvtb/Download) for installing BCVTB
-software. Another option is to copy the `bcvtb` folder from [this repository]
-(https://github.com/zhangzhizza/Gym-Eplus/tree/master/eplus_env/envs) #### 4.
-Set environment variables Two environment variables must be set: `EPLUS_PATH`
-and `BCVTB_PATH`, with the locations where EnergyPlus and BCVTB are installed
-respectively. ## About Sinergym package As we have told you in section *Manual
-Installation*, Python environment can be set up using *python_environment.yml*
-with *conda*. However, we can make an installation using the Github repository
-itself: ```sh $ cd sinergym $ pip install -e . ``` Extra libraries can be
-installed by typing ``pip install -e .[extras]``. *extras* include all optional
-libraries which have been considered in this project such as testing,
-visualization, Deep Reinforcement Learning, monitoring , etc. It's possible to
-select a subset of these libraries instead of 'extras' tag in which we select
-all optional libraries, for example: ```sh $ pip install -e .[test,doc] ``` In
-order to check all our tag list, visit `setup.py
-github.com/ugr-sail/sinergym/blob/main/setup.py>`__ in *Sinergym* root
-repository. In any case, they are not a requirement of the package. You can
-also install from `oficial pypi repository
-pypi.org/project/sinergym/>`__ with last stable version by default: ```sh $ pip
-install sinergym[extras] ``` ## Check Installation This project is
-automatically supervised using tests developed specifically for it. If you want
-to check *Sinergym* has been installed successfully, run next command: ```sh $
-pytest tests/ -vv ``` Anyway, every time *Sinergym* repository is updated, the
-tests will run automatically in a remote container using the Dockerfile to
-build it. `Github Action
-docs.github.com/es/actions/>`__ will do that job (see our documentation for
-more information). ## Usage example If you used our Dockerfile during
-installation, you should have the *try_env.py* file in your workspace as soon
-as you enter in. In case you have installed everything on your local machine
-directly, place it inside our cloned repository. In any case, we start from the
-point that you have at your disposal a terminal with the appropriate python
-version and *Sinergym* running correctly. *Sinergym* uses the standard
-Gymnasium API. So basic loop should be something like: ```python import
-gymnasium as gym import sinergym # Create the environment env = gym.make
-('Eplus-datacenter-mixed-continuous-stochastic-v1') # Initialize the episode
-obs, info = env.reset() terminated = False R = 0.0 while not terminated: a =
-env.action_space.sample() # random action selection obs, reward, terminated,
-truncated, info = env.step(a) # get new observation and reward R += reward
-print('Total reward for the episode: %.4f' % R) env.close() ``` Notice that a
-folder will be created in the working directory after creating the environment.
-It will contain the EnergyPlus outputs produced during the simulation. :pencil:
-For more examples and details, please visit our [usage examples](https://ugr-
-sail.github.io/sinergym/compilation/main/pages/notebooks/
-basic_example.html#Basic-example) documentation section. ## Google Cloud
-Platform support Cloud Computing For more information about this functionality,
-please, visit our documentation [here](https://ugr-sail.github.io/sinergym/
-compilation/main/pages/gcloudAPI.html#sinergym-with-google-cloud). ## Citing
-Sinergym If you use *Sinergym* in your work, please cite our [paper](https://
-dl.acm.org/doi/abs/10.1145/3486611.3488729): ```bibtex @inproceedings
+official *Sinergym* documentation. ## Installation Please, visit [INSTALL.md]
+(https://github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for more
+information about Sinergym installation. ## Usage example If you used our
+Dockerfile during installation, you should have the *try_env.py* file in your
+workspace as soon as you enter in. In case you have installed everything on
+your local machine directly, place it inside our cloned repository. In any
+case, we start from the point that you have at your disposal a terminal with
+the appropriate python version and *Sinergym* running correctly. *Sinergym*
+uses the standard Gymnasium API. So basic loop should be something like:
+```python import gymnasium as gym import sinergym # Create the environment env
+= gym.make('Eplus-datacenter-mixed-continuous-stochastic-v1') # Initialize the
+episode obs, info = env.reset() terminated = False R = 0.0 while not
+terminated: a = env.action_space.sample() # random action selection obs,
+reward, terminated, truncated, info = env.step(a) # get new observation and
+reward R += reward print('Total reward for the episode: %.4f' % R) env.close()
+``` Notice that a folder will be created in the working directory after
+creating the environment. It will contain the EnergyPlus outputs produced
+during the simulation. :pencil: For more examples and details, please visit our
+[usage examples](https://ugr-sail.github.io/sinergym/compilation/main/pages/
+notebooks/basic_example.html#Basic-example) documentation section. ## Google
+Cloud Platform support For more information about this functionality, please,
+visit our documentation [here](https://ugr-sail.github.io/sinergym/compilation/
+main/pages/gcloudAPI.html#sinergym-with-google-cloud). ## Projects using
+Sinergym The following are some of the projects benefiting from the advantages
+of Sinergym: - [Demosthen/ActiveRL](https://github.com/Demosthen/ActiveRL) -
+[VectorInstitute/HV-Ai-C](https://github.com/VectorInstitute/HV-Ai-C) - [rdnfn/
+beobench](https://github.com/rdnfn/beobench) :pencil: If you want to appear in
+this list, do not hesitate to send us a PR and include the following badge in
+your repository:
+       [https://img.shields.io/badge/Powered%20by-Sinergym%20%E2%86%92-
+           gray.svg?colorA=00BABF&colorB=4BF2F7&style=for-the-badge]
+## Citing Sinergym If you use *Sinergym* in your work, please cite our [paper]
+(https://dl.acm.org/doi/abs/10.1145/3486611.3488729): ```bibtex @inproceedings
 {2021sinergym, title={Sinergym: A Building Simulation and Control Framework for
 Training Reinforcement Learning Agents}, author={JimÃ©nez-Raboso, Javier and
 Campoy-Nieves, Alejandro and Manjavacas-Lucas, Antonio and GÃ³mez-Romero, Juan
 and Molina-Solana, Miguel}, year={2021}, isbn = {9781450391146}, publisher =
 {Association for Computing Machinery}, address = {New York, NY, USA}, url =
 {https://doi.org/10.1145/3486611.3488729}, doi = {10.1145/3486611.3488729},
 booktitle = {Proceedings of the 8th ACM International Conference on Systems for
```

### Comparing `sinergym-2.3.2/setup.py` & `sinergym-2.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/__init__.py` & `sinergym-2.3.3/sinergym/__init__.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf` & `sinergym-2.3.3/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/buildings/5ZoneAutoDXVAV.idf` & `sinergym-2.3.3/sinergym/data/buildings/5ZoneAutoDXVAV.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf` & `sinergym-2.3.3/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf` & `sinergym-2.3.3/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/buildings/OfficeGridStorageSmoothing.idf` & `sinergym-2.3.3/sinergym/data/buildings/OfficeGridStorageSmoothing.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/buildings/ShopWithVandBattery.idf` & `sinergym-2.3.3/sinergym/data/buildings/ShopWithVandBattery.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd` & `sinergym-2.3.3/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/variables/5ZoneAutoDXVAV.rdd` & `sinergym-2.3.3/sinergym/data/variables/5ZoneAutoDXVAV.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd` & `sinergym-2.3.3/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd` & `sinergym-2.3.3/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/variables/OfficeGridStorageSmoothing.rdd` & `sinergym-2.3.3/sinergym/data/variables/OfficeGridStorageSmoothing.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/variables/ShopWithVandBattery.rdd` & `sinergym-2.3.3/sinergym/data/variables/ShopWithVandBattery.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy` & `sinergym-2.3.3/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw` & `sinergym-2.3.3/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy` & `sinergym-2.3.3/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/COL_Bogota.802220_IWEC.epw` & `sinergym-2.3.3/sinergym/data/weather/COL_Bogota.802220_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy` & `sinergym-2.3.3/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/ESP_Granada.084190_SWEC.epw` & `sinergym-2.3.3/sinergym/data/weather/ESP_Granada.084190_SWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy` & `sinergym-2.3.3/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw` & `sinergym-2.3.3/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy` & `sinergym-2.3.3/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw` & `sinergym-2.3.3/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy` & `sinergym-2.3.3/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw` & `sinergym-2.3.3/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy` & `sinergym-2.3.3/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw` & `sinergym-2.3.3/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy` & `sinergym-2.3.3/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw` & `sinergym-2.3.3/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy` & `sinergym-2.3.3/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw` & `sinergym-2.3.3/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy` & `sinergym-2.3.3/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw` & `sinergym-2.3.3/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy` & `sinergym-2.3.3/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw` & `sinergym-2.3.3/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy` & `sinergym-2.3.3/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw` & `sinergym-2.3.3/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy` & `sinergym-2.3.3/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw` & `sinergym-2.3.3/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/envs/eplus_env.py` & `sinergym-2.3.3/sinergym/envs/eplus_env.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/simulators/base.py` & `sinergym-2.3.3/sinergym/simulators/base.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/simulators/eplus.py` & `sinergym-2.3.3/sinergym/simulators/eplus.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/simulators/eplus_alpha.py` & `sinergym-2.3.3/sinergym/simulators/eplus_alpha.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/utils/callbacks.py` & `sinergym-2.3.3/sinergym/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/utils/common.py` & `sinergym-2.3.3/sinergym/utils/common.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/utils/config.py` & `sinergym-2.3.3/sinergym/utils/config.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/utils/constants.py` & `sinergym-2.3.3/sinergym/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/utils/controllers.py` & `sinergym-2.3.3/sinergym/utils/controllers.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/utils/env_checker.py` & `sinergym-2.3.3/sinergym/utils/env_checker.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/utils/evaluation.py` & `sinergym-2.3.3/sinergym/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/utils/gcloud.py` & `sinergym-2.3.3/sinergym/utils/gcloud.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/utils/logger.py` & `sinergym-2.3.3/sinergym/utils/logger.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/utils/rewards.py` & `sinergym-2.3.3/sinergym/utils/rewards.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym/utils/wrappers.py` & `sinergym-2.3.3/sinergym/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym.egg-info/SOURCES.txt` & `sinergym-2.3.3/sinergym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.2/sinergym.egg-info/requires.txt` & `sinergym-2.3.3/sinergym.egg-info/requires.txt`

 * *Files identical despite different names*


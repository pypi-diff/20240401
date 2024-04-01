# Comparing `tmp/sinergym-3.2.4.tar.gz` & `tmp/sinergym-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinergym-3.2.4.tar", last modified: Mon Feb 26 16:18:36 2024, max compression
+gzip compressed data, was "sinergym-3.2.7.tar", last modified: Wed Mar 13 10:52:10 2024, max compression
```

## Comparing `sinergym-3.2.4.tar` & `sinergym-3.2.7.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:18:36.039314 sinergym-3.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-26 16:18:31.000000 sinergym-3.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-26 16:18:31.000000 sinergym-3.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13632 2024-02-26 16:18:36.039314 sinergym-3.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-02-26 16:18:31.000000 sinergym-3.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-26 16:18:35.000000 sinergym-3.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-26 16:18:36.039314 sinergym-3.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-02-26 16:18:35.000000 sinergym-3.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:18:35.999314 sinergym-3.2.4/sinergym/
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:18:35.999314 sinergym-3.2.4/sinergym/config/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29305 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/config/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:18:35.999314 sinergym-3.2.4/sinergym/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:18:36.003314 sinergym-3.2.4/sinergym/data/buildings/
--rw-r--r--   0 runner    (1001) docker     (127)    66897 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/buildings/1ZoneDataCenterCRAC_wApproachTemp.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   151242 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   145450 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   595437 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   272977 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   512302 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   245040 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/buildings/ShopWithPVandBattery.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   389111 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/buildings/autobalance_model.epJSON
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:18:36.007314 sinergym-3.2.4/sinergym/data/default_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/default_configuration/1ZoneDataCenterCRAC_wApproachTemp.json
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/default_configuration/2ZoneDataCenterHVAC_wEconomizer.json
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/default_configuration/5ZoneAutoDXVAV.json
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/default_configuration/ASHRAE901_OfficeMedium_STD2019_Denver.json
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/default_configuration/ASHRAE901_Warehouse_STD2019_Denver.json
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/default_configuration/LrgOff_GridStorageScheduled.json
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/default_configuration/ShopWithPVandBattery.json
--rw-r--r--   0 runner    (1001) docker     (127)    12388 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/default_configuration/autobalance_model.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:18:36.035314 sinergym-3.2.4/sinergym/data/weather/
--rw-r--r--   0 runner    (1001) docker     (127)    28629 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1565086 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28503 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1550279 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28704 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1621761 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28716 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1553382 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28801 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1558629 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28740 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1558423 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28659 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1601571 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29165 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1550263 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29016 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1637298 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29489 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1629153 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28793 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1639985 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29614 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1613784 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29529 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1624547 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29243 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1625209 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:18:36.039314 sinergym-3.2.4/sinergym/envs/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26783 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/envs/eplus_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:18:36.039314 sinergym-3.2.4/sinergym/simulators/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/simulators/eplus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:18:36.039314 sinergym-3.2.4/sinergym/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22490 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/utils/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/utils/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/utils/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/utils/rewards.py
--rw-r--r--   0 runner    (1001) docker     (127)    36173 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/utils/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:18:35.999314 sinergym-3.2.4/sinergym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13632 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-26 16:18:35.000000 sinergym-3.2.4/sinergym.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.910455 sinergym-3.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-13 10:52:06.000000 sinergym-3.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-13 10:52:06.000000 sinergym-3.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13632 2024-03-13 10:52:10.910455 sinergym-3.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-03-13 10:52:06.000000 sinergym-3.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-13 10:52:10.000000 sinergym-3.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-13 10:52:10.910455 sinergym-3.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-03-13 10:52:10.000000 sinergym-3.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.870455 sinergym-3.2.7/sinergym/
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.874455 sinergym-3.2.7/sinergym/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29305 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/config/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.870455 sinergym-3.2.7/sinergym/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.874455 sinergym-3.2.7/sinergym/data/buildings/
+-rw-r--r--   0 runner    (1001) docker     (127)    66897 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/1ZoneDataCenterCRAC_wApproachTemp.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   151242 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   145181 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   595437 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   272977 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   512302 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   245040 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/ShopWithPVandBattery.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   389111 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/radiant_residential_building.epJSON
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.878455 sinergym-3.2.7/sinergym/data/default_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/1ZoneDataCenterCRAC_wApproachTemp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/2ZoneDataCenterHVAC_wEconomizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/5ZoneAutoDXVAV.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/ASHRAE901_OfficeMedium_STD2019_Denver.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/ASHRAE901_Warehouse_STD2019_Denver.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/LrgOff_GridStorageScheduled.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/ShopWithPVandBattery.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/radiant_residential_building.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.906455 sinergym-3.2.7/sinergym/data/weather/
+-rw-r--r--   0 runner    (1001) docker     (127)    28629 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1565086 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28503 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1550279 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28704 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1621761 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28716 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1553382 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28801 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1558629 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28740 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1558423 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28659 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1601571 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29165 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1550263 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29016 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1637298 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29489 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1629153 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28793 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1639985 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29614 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1613784 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29529 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1624547 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29243 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1625209 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.906455 sinergym-3.2.7/sinergym/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26793 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/envs/eplus_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.906455 sinergym-3.2.7/sinergym/simulators/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/simulators/eplus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.910455 sinergym-3.2.7/sinergym/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22490 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36173 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.874455 sinergym-3.2.7/sinergym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13632 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym.egg-info/top_level.txt
```

### Comparing `sinergym-3.2.4/LICENSE` & `sinergym-3.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/PKG-INFO` & `sinergym-3.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 3.2.4
+Version: 3.2.7
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 3.2.4 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 3.2.7 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-3.2.4/README.md` & `sinergym-3.2.7/README.md`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/setup.py` & `sinergym-3.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/__init__.py` & `sinergym-3.2.7/sinergym/__init__.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/config/modeling.py` & `sinergym-3.2.7/sinergym/config/modeling.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/buildings/1ZoneDataCenterCRAC_wApproachTemp.epJSON` & `sinergym-3.2.7/sinergym/data/buildings/1ZoneDataCenterCRAC_wApproachTemp.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON` & `sinergym-3.2.7/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON` & `sinergym-3.2.7/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999768089053804%*

 * *Differences: {"'Schedule:Compact'": "{'Min OARequirements Sched': {'data': {1: {'field': 'For: AllDays'}, 3: "*

 * *                       "{'field': 0.005}, delete: [3, 2, 1]}}}"}*

```diff
@@ -3000,30 +3000,21 @@
         },
         "Min OARequirements Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
-                    "field": "For: Weekdays SummerDesignDay WinterDesignDay"
+                    "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 1.0
-                },
-                {
-                    "field": "For: AllOtherDays"
-                },
-                {
-                    "field": "Until: 24:00"
-                },
-                {
-                    "field": 0.25
+                    "field": 0.005
                 }
             ],
             "schedule_type_limits_name": "Any Number"
         },
         "OCCUPY-1": {
             "data": [
                 {
```

### Comparing `sinergym-3.2.4/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON` & `sinergym-3.2.7/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON` & `sinergym-3.2.7/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON` & `sinergym-3.2.7/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/buildings/ShopWithPVandBattery.epJSON` & `sinergym-3.2.7/sinergym/data/buildings/ShopWithPVandBattery.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/buildings/autobalance_model.epJSON` & `sinergym-3.2.7/sinergym/data/buildings/radiant_residential_building.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/default_configuration/1ZoneDataCenterCRAC_wApproachTemp.json` & `sinergym-3.2.7/sinergym/data/default_configuration/1ZoneDataCenterCRAC_wApproachTemp.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/default_configuration/2ZoneDataCenterHVAC_wEconomizer.json` & `sinergym-3.2.7/sinergym/data/default_configuration/2ZoneDataCenterHVAC_wEconomizer.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/default_configuration/5ZoneAutoDXVAV.json` & `sinergym-3.2.7/sinergym/data/default_configuration/5ZoneAutoDXVAV.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'action_space'": "'gym.spaces.Box(low=np.array([12.0, 23.25], dtype=np.float32), "*

 * *                   "high=np.array([23.25, 30.0], dtype=np.float32), shape=(2,), dtype=np.float32)'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "action_space": "gym.spaces.Box(low=np.array([12.0, 23.5], dtype=np.float32), high=np.array([21.5, 40.0], dtype=np.float32), shape=(2,), dtype=np.float32)",
+    "action_space": "gym.spaces.Box(low=np.array([12.0, 23.25], dtype=np.float32), high=np.array([23.25, 30.0], dtype=np.float32), shape=(2,), dtype=np.float32)",
     "action_space_discrete": "gym.spaces.Discrete(10)",
     "actuators": {
         "CLG-SETP-SCH": {
             "element_type": "Schedule:Compact",
             "value_type": "Schedule Value",
             "variable_name": "Cooling_Setpoint_RL"
         },
```

### Comparing `sinergym-3.2.4/sinergym/data/default_configuration/ASHRAE901_OfficeMedium_STD2019_Denver.json` & `sinergym-3.2.7/sinergym/data/default_configuration/ASHRAE901_OfficeMedium_STD2019_Denver.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/default_configuration/ASHRAE901_Warehouse_STD2019_Denver.json` & `sinergym-3.2.7/sinergym/data/default_configuration/ASHRAE901_Warehouse_STD2019_Denver.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/default_configuration/LrgOff_GridStorageScheduled.json` & `sinergym-3.2.7/sinergym/data/default_configuration/LrgOff_GridStorageScheduled.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/default_configuration/ShopWithPVandBattery.json` & `sinergym-3.2.7/sinergym/data/default_configuration/ShopWithPVandBattery.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/default_configuration/autobalance_model.json` & `sinergym-3.2.7/sinergym/data/default_configuration/radiant_residential_building.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'building_file'": "'radiant_residential_building.epJSON'",*

 * * "'id_base'": "'radiant'",*

 * * "'only_discrete'": 'True'}*

```diff
@@ -29,20 +29,20 @@
         },
         "LIVING RADIANT AVAILAVILITY": {
             "element_type": "Schedule:Compact",
             "value_type": "Schedule Value",
             "variable_name": "radiant_livroom"
         }
     },
-    "building_file": "autobalance_model.epJSON",
+    "building_file": "radiant_residential_building.epJSON",
     "config_params": null,
-    "id_base": "autobalance",
+    "id_base": "radiant",
     "max_ep_data_store_num": 10,
     "meters": {},
-    "only_discrete": false,
+    "only_discrete": true,
     "reward": "LinearReward",
     "reward_kwargs": {
         "energy_variables": [
             "HVAC_electricity_demand_rate"
         ],
         "energy_weight": 0.5,
         "lambda_energy": 1.0,
```

### Comparing `sinergym-3.2.4/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy` & `sinergym-3.2.7/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw` & `sinergym-3.2.7/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy` & `sinergym-3.2.7/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/COL_Bogota.802220_IWEC.epw` & `sinergym-3.2.7/sinergym/data/weather/COL_Bogota.802220_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy` & `sinergym-3.2.7/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/ESP_Granada.084190_SWEC.epw` & `sinergym-3.2.7/sinergym/data/weather/ESP_Granada.084190_SWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy` & `sinergym-3.2.7/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw` & `sinergym-3.2.7/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy` & `sinergym-3.2.7/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw` & `sinergym-3.2.7/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy` & `sinergym-3.2.7/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw` & `sinergym-3.2.7/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy` & `sinergym-3.2.7/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw` & `sinergym-3.2.7/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.ddy` & `sinergym-3.2.7/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.epw` & `sinergym-3.2.7/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy` & `sinergym-3.2.7/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw` & `sinergym-3.2.7/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy` & `sinergym-3.2.7/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw` & `sinergym-3.2.7/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy` & `sinergym-3.2.7/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw` & `sinergym-3.2.7/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy` & `sinergym-3.2.7/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw` & `sinergym-3.2.7/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy` & `sinergym-3.2.7/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw` & `sinergym-3.2.7/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy` & `sinergym-3.2.7/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw` & `sinergym-3.2.7/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/envs/eplus_env.py` & `sinergym-3.2.7/sinergym/envs/eplus_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,15 +544,15 @@
     - Weather file(s): {}
     - Current weather used: {}
     - Episodes executed: {}
     - Workspace directory: {}
     - Reward function: {}
     - Reset default options: {}
     - Run period: {}
-    - Episode length: {}
+    - Episode length (seconds): {}
     - Number of timesteps in an episode: {}
     - Timestep size (seconds): {}
     - It is discrete?: {}
     #----------------------------------------------------------------------------------#
                                 ENVIRONMENT SPACE:
     #----------------------------------------------------------------------------------#
     - Observation space: {}
```

### Comparing `sinergym-3.2.4/sinergym/simulators/eplus.py` & `sinergym-3.2.7/sinergym/simulators/eplus.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             self.energyplus_state, _warmup_complete)
 
         # register callback used to collect observations
         self.api.runtime.callback_end_zone_timestep_after_zone_reporting(
             self.energyplus_state, self._collect_obs_and_info)
 
         # register callback used to send actions
-        self.api.runtime.callback_begin_system_timestep_before_predictor(
+        self.api.runtime.callback_end_zone_timestep_after_zone_reporting(
             self.energyplus_state, self._process_action)
 
         # run EnergyPlus in a non-blocking way
         def _run_energyplus(runtime, cmd_args, state, results):
             self.logger.info(
                 'Running EnergyPlus with args: {}'.format(cmd_args))
```

### Comparing `sinergym-3.2.4/sinergym/utils/callbacks.py` & `sinergym-3.2.7/sinergym/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/utils/common.py` & `sinergym-3.2.7/sinergym/utils/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,36 @@
 import gymnasium as gym
 import numpy as np
 import pandas as pd
 import xlsxwriter
 from eppy.modeleditor import IDF
 from opyplus.epm.record import Record
 
+import sinergym
 from sinergym.utils.constants import YEAR
 from sinergym.utils.rewards import *
 
+# --------------------- Sinergym environment information --------------------- #
+
+
+def get_ids(start='Eplus') -> List[str]:
+    """
+    Returns a list of environment IDs created by Sinergym (starting by Eplus).
+
+    Parameters:
+        start (str): The prefix to filter the environment IDs. Defaults to 'Eplus'.
+
+    Returns:
+        List[str]: A list of Sinergym environment IDs.
+
+    """
+    envs_id = [env_id for env_id in gym.envs.registration.registry.keys()
+               if env_id.startswith(start)]
+    return envs_id
+
 # --------------------------------- Wrappers --------------------------------- #
 
 
 def is_wrapped(env: Type[gym.Env], wrapper_class: Type[gym.Wrapper]) -> bool:
     """
     Check if a given environment has been wrapped with a given wrapper.
```

### Comparing `sinergym-3.2.4/sinergym/utils/constants.py` & `sinergym-3.2.7/sinergym/utils/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,24 +40,24 @@
 
 def DEFAULT_5ZONE_DISCRETE_FUNCTION(action: int) -> List[float]:
     # SB3 algotihms returns a ndarray instead of a int
     if isinstance(action, np.ndarray):
         action = int(action.item())
 
     mapping = {
-        0: [13, 37],
-        1: [14, 34],
-        2: [15, 32],
-        3: [16, 30],
-        4: [17, 30],
-        5: [18, 30],
-        6: [19, 27],
-        7: [20, 26],
-        8: [21, 25],
-        9: [21, 24]
+        0: [12, 30],
+        1: [13, 30],
+        2: [14, 29],
+        3: [15, 28],
+        4: [16, 28],
+        5: [17, 27],
+        6: [18, 26],
+        7: [19, 25],
+        8: [20, 24],
+        9: [21, 23.25]
     }
 
     return mapping[action]
 
 
 # ----------------------------------DATACENTER--------------------------------- #
 
@@ -172,15 +172,15 @@
     }
 
     return mapping[action]
 
 # -------------------------------- AUTOBALANCE ------------------------------- #
 
 
-def DEFAULT_AUTOBALANCE_DISCRETE_FUNCTION(
+def DEFAULT_RADIANT_DISCRETE_FUNCTION(
         action: Union[np.ndarray, List[int]]) -> List[float]:
     action[5] += 25
     return list(action)
 
 
 # ----------------------------------HOSPITAL--------------------------------- #
 # DEFAULT_HOSPITAL_OBSERVATION_VARIABLES = [
```

### Comparing `sinergym-3.2.4/sinergym/utils/controllers.py` & `sinergym-3.2.7/sinergym/utils/controllers.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         self.env = env
 
         self.observation_variables = env.get_wrapper_attr(
             'observation_variables')
         self.action_variables = env.get_wrapper_attr('action_variables')
 
-        self.setpoints_summer = (22.5, 26.0)
+        self.setpoints_summer = (23.0, 26.0)
         self.setpoints_winter = (20.0, 23.5)
 
     def act(self, observation: List[Any]) -> Sequence[Any]:
         """Select action based on indoor temperature.
 
         Args:
             observation (List[Any]): Perceived observation.
```

### Comparing `sinergym-3.2.4/sinergym/utils/env_checker.py` & `sinergym-3.2.7/sinergym/utils/env_checker.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/utils/evaluation.py` & `sinergym-3.2.7/sinergym/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/utils/gcloud.py` & `sinergym-3.2.7/sinergym/utils/gcloud.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/utils/logger.py` & `sinergym-3.2.7/sinergym/utils/logger.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/utils/rewards.py` & `sinergym-3.2.7/sinergym/utils/rewards.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym/utils/wrappers.py` & `sinergym-3.2.7/sinergym/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.4/sinergym.egg-info/PKG-INFO` & `sinergym-3.2.7/sinergym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 3.2.4
+Version: 3.2.7
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 3.2.4 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 3.2.7 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-3.2.4/sinergym.egg-info/SOURCES.txt` & `sinergym-3.2.7/sinergym.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 sinergym/data/buildings/1ZoneDataCenterCRAC_wApproachTemp.epJSON
 sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON
 sinergym/data/buildings/5ZoneAutoDXVAV.epJSON
 sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON
 sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON
 sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON
 sinergym/data/buildings/ShopWithPVandBattery.epJSON
-sinergym/data/buildings/autobalance_model.epJSON
+sinergym/data/buildings/radiant_residential_building.epJSON
 sinergym/data/default_configuration/1ZoneDataCenterCRAC_wApproachTemp.json
 sinergym/data/default_configuration/2ZoneDataCenterHVAC_wEconomizer.json
 sinergym/data/default_configuration/5ZoneAutoDXVAV.json
 sinergym/data/default_configuration/ASHRAE901_OfficeMedium_STD2019_Denver.json
 sinergym/data/default_configuration/ASHRAE901_Warehouse_STD2019_Denver.json
 sinergym/data/default_configuration/LrgOff_GridStorageScheduled.json
 sinergym/data/default_configuration/ShopWithPVandBattery.json
-sinergym/data/default_configuration/autobalance_model.json
+sinergym/data/default_configuration/radiant_residential_building.json
 sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
 sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
 sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
 sinergym/data/weather/COL_Bogota.802220_IWEC.epw
 sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
 sinergym/data/weather/ESP_Granada.084190_SWEC.epw
 sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
```

### Comparing `sinergym-3.2.4/sinergym.egg-info/requires.txt` & `sinergym-3.2.7/sinergym.egg-info/requires.txt`

 * *Files identical despite different names*


# Comparing `tmp/emhass-0.8.4.tar.gz` & `tmp/emhass-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emhass-0.8.4.tar", last modified: Wed Mar 13 19:59:41 2024, max compression
+gzip compressed data, was "emhass-0.8.5.tar", last modified: Mon Apr  1 21:38:57 2024, max compression
```

## Comparing `emhass-0.8.4.tar` & `emhass-0.8.5.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:59:41.846814 emhass-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)    21003 2024-03-13 19:59:38.000000 emhass-0.8.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-03-13 19:59:38.000000 emhass-0.8.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-13 19:59:38.000000 emhass-0.8.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-13 19:59:38.000000 emhass-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-13 19:59:38.000000 emhass-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    34743 2024-03-13 19:59:41.846814 emhass-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33586 2024-03-13 19:59:38.000000 emhass-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:59:41.842814 emhass-0.8.4/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-13 19:59:38.000000 emhass-0.8.4/data/data_load_cost_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-13 19:59:38.000000 emhass-0.8.4/data/data_load_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-13 19:59:38.000000 emhass-0.8.4/data/data_prod_price_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)   185427 2024-03-13 19:59:38.000000 emhass-0.8.4/data/data_train_load_clustering.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   185431 2024-03-13 19:59:38.000000 emhass-0.8.4/data/data_train_load_forecast.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-13 19:59:38.000000 emhass-0.8.4/data/data_weather_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-13 19:59:38.000000 emhass-0.8.4/data/opt_res_latest.csv
--rw-r--r--   0 runner    (1001) docker     (127)    54568 2024-03-13 19:59:38.000000 emhass-0.8.4/data/opt_res_perfect_optim_cost.csv
--rw-r--r--   0 runner    (1001) docker     (127)    52501 2024-03-13 19:59:38.000000 emhass-0.8.4/data/opt_res_perfect_optim_profit.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53838 2024-03-13 19:59:38.000000 emhass-0.8.4/data/opt_res_perfect_optim_self-consumption.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-03-13 19:59:38.000000 emhass-0.8.4/data/test_df_final.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    97491 2024-03-13 19:59:38.000000 emhass-0.8.4/data/test_response_get_data_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-03-13 19:59:38.000000 emhass-0.8.4/data/test_response_scrapper_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-13 19:59:38.000000 emhass-0.8.4/data/test_response_solarforecast_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-03-13 19:59:38.000000 emhass-0.8.4/data/test_response_solcast_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-13 19:59:38.000000 emhass-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 19:59:41.846814 emhass-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-03-13 19:59:38.000000 emhass-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:59:41.834814 emhass-0.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:59:41.842814 emhass-0.8.4/src/emhass/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37464 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    43555 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)    15640 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)    37181 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    18400 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/retrieve_hass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:59:41.846814 emhass-0.8.4/src/emhass/static/
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/static/advanced.html
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/static/basic.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:59:41.846814 emhass-0.8.4/src/emhass/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/static/img/emhass_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    66736 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/static/img/emhass_logo_short.svg
--rw-r--r--   0 runner    (1001) docker     (127)    60319 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/static/img/feather-sprite.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18173 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/static/script.js
--rw-r--r--   0 runner    (1001) docker     (127)    15222 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:59:41.846814 emhass-0.8.4/src/emhass/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/templates/template.html
--rw-r--r--   0 runner    (1001) docker     (127)    46151 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21475 2024-03-13 19:59:38.000000 emhass-0.8.4/src/emhass/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:59:41.846814 emhass-0.8.4/src/emhass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    34743 2024-03-13 19:59:41.000000 emhass-0.8.4/src/emhass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-13 19:59:41.000000 emhass-0.8.4/src/emhass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 19:59:41.000000 emhass-0.8.4/src/emhass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-13 19:59:41.000000 emhass-0.8.4/src/emhass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-13 19:59:41.000000 emhass-0.8.4/src/emhass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-13 19:59:41.000000 emhass-0.8.4/src/emhass.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:59:41.846814 emhass-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    26128 2024-03-13 19:59:38.000000 emhass-0.8.4/tests/test_command_line_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27836 2024-03-13 19:59:38.000000 emhass-0.8.4/tests/test_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-03-13 19:59:38.000000 emhass-0.8.4/tests/test_machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)    17562 2024-03-13 19:59:38.000000 emhass-0.8.4/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-03-13 19:59:38.000000 emhass-0.8.4/tests/test_retrieve_hass.py
--rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-03-13 19:59:38.000000 emhass-0.8.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.183555 emhass-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    21750 2024-04-01 21:38:53.000000 emhass-0.8.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-01 21:38:53.000000 emhass-0.8.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-01 21:38:53.000000 emhass-0.8.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-01 21:38:53.000000 emhass-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 21:38:53.000000 emhass-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    34742 2024-04-01 21:38:57.183555 emhass-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33584 2024-04-01 21:38:53.000000 emhass-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.171555 emhass-0.8.5/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-01 21:38:53.000000 emhass-0.8.5/data/data_load_cost_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-01 21:38:53.000000 emhass-0.8.5/data/data_load_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-01 21:38:53.000000 emhass-0.8.5/data/data_prod_price_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   185427 2024-04-01 21:38:53.000000 emhass-0.8.5/data/data_train_load_clustering.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   185431 2024-04-01 21:38:53.000000 emhass-0.8.5/data/data_train_load_forecast.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-01 21:38:53.000000 emhass-0.8.5/data/data_weather_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-01 21:38:53.000000 emhass-0.8.5/data/opt_res_latest.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    54568 2024-04-01 21:38:53.000000 emhass-0.8.5/data/opt_res_perfect_optim_cost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    52501 2024-04-01 21:38:53.000000 emhass-0.8.5/data/opt_res_perfect_optim_profit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53838 2024-04-01 21:38:53.000000 emhass-0.8.5/data/opt_res_perfect_optim_self-consumption.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-01 21:38:53.000000 emhass-0.8.5/data/test_df_final.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    97491 2024-04-01 21:38:53.000000 emhass-0.8.5/data/test_response_get_data_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-01 21:38:53.000000 emhass-0.8.5/data/test_response_scrapper_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-01 21:38:53.000000 emhass-0.8.5/data/test_response_solarforecast_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-01 21:38:53.000000 emhass-0.8.5/data/test_response_solcast_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-01 21:38:53.000000 emhass-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:38:57.183555 emhass-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-01 21:38:53.000000 emhass-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.167555 emhass-0.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.175555 emhass-0.8.5/src/emhass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37462 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.175555 emhass-0.8.5/src/emhass/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   168272 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/data/cec_inverters.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)  1655747 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/data/cec_modules.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)    43796 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15640 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37197 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18406 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/retrieve_hass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.179556 emhass-0.8.5/src/emhass/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/advanced.html
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/basic.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.179556 emhass-0.8.5/src/emhass/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/img/emhass_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66736 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/img/emhass_logo_short.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    60319 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/img/feather-sprite.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/script.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15557 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.179556 emhass-0.8.5/src/emhass/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/templates/template.html
+-rw-r--r--   0 runner    (1001) docker     (127)    42394 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.183555 emhass-0.8.5/src/emhass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34742 2024-04-01 21:38:57.000000 emhass-0.8.5/src/emhass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-01 21:38:57.000000 emhass-0.8.5/src/emhass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:38:57.000000 emhass-0.8.5/src/emhass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 21:38:57.000000 emhass-0.8.5/src/emhass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-01 21:38:57.000000 emhass-0.8.5/src/emhass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 21:38:57.000000 emhass-0.8.5/src/emhass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.179556 emhass-0.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    25232 2024-04-01 21:38:53.000000 emhass-0.8.5/tests/test_command_line_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29703 2024-04-01 21:38:53.000000 emhass-0.8.5/tests/test_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-01 21:38:53.000000 emhass-0.8.5/tests/test_machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17562 2024-04-01 21:38:53.000000 emhass-0.8.5/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-01 21:38:53.000000 emhass-0.8.5/tests/test_retrieve_hass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-04-01 21:38:53.000000 emhass-0.8.5/tests/test_utils.py
```

### Comparing `emhass-0.8.4/CHANGELOG.md` & `emhass-0.8.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Changelog
 
+## 0.8.5 - 2024-04-01
+### Improvement
+- Simplified fetch urls to relatives
+- Improved code for passed forecast data error handling in utils.py
+- Added new tests for forecast longer than 24h by changing parameter `delta_forecast`
+- Added new files for updated PV modules and inverters database for use with PVLib
+- Added a new webapp to help configuring modules and inverters: [https://emhass-pvlib-database.streamlit.app/](https://emhass-pvlib-database.streamlit.app/)
+- Added a new `P_to_grid_max` variable, different from the current `P_from_grid_max` option
+### Fix
+- style.css auto format and adjusted table styling
+- Changed pandas datetime rounding to nonexistent='shift_forward' to help survive DST change
+- Dropped support for Python 3.9
+
 ## 0.8.4 - 2024-03-13
 ### Improvement
 - Improved documentation
 - Improved logging errors on missing day info
 ### Fix
 - Missing round treatment for DST survival in utils.py 
 - Webui large icons fix
```

### Comparing `emhass-0.8.4/CODE_OF_CONDUCT.md` & `emhass-0.8.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/CONTRIBUTING.md` & `emhass-0.8.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/LICENSE` & `emhass-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/PKG-INFO` & `emhass-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: emhass
-Version: 0.8.4
+Version: 0.8.5
 Summary: An Energy Management System for Home Assistant
 Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ
 Author-email: davidusb@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9, <3.12
+Requires-Python: >=3.10, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
 Requires-Dist: numpy==1.26.4
 Requires-Dist: scipy==1.12.0
 Requires-Dist: pandas<=2.0.3
 Requires-Dist: pvlib>=0.10.2
@@ -462,16 +462,14 @@
 curl -i -H 'Content-Type:application/json' -X POST -d '{"pv_power_forecast":[0, 70, 141.22, 246.18, 513.5, 753.27, 1049.89, 1797.93, 1697.3, 3078.93], "prediction_horizon":10, "soc_init":0.5,"soc_final":0.6}' http://192.168.3.159:5000/action/naive-mpc-optim
 ```
 *Example with :`def_total_hours`, `def_start_timestep`, `def_end_timestep`.*
 ```bash
 curl -i -H 'Content-Type:application/json' -X POST -d '{"pv_power_forecast":[0, 70, 141.22, 246.18, 513.5, 753.27, 1049.89, 1797.93, 1697.3, 3078.93], "prediction_horizon":10, "soc_init":0.5,"soc_final":0.6,"def_total_hours":[1,3],"def_start_timestep":[0,3],"def_end_timestep":[0,6]}' http://localhost:5000/action/naive-mpc-optim
 ```
 
-
-
 ## A machine learning forecaster
 
 Starting in v0.4.0 a new machine learning forecaster class was introduced.
 This is intended to provide a new and alternative method to forecast your household consumption and use it when such forecast is needed to optimize your energy through the available strategies.
 Check the dedicated section in the documentation here: [https://emhass.readthedocs.io/en/latest/mlforecaster.html](https://emhass.readthedocs.io/en/latest/mlforecaster.html)
 
 ## Development
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: emhass Version: 0.8.4 Summary: An Energy Management
+Metadata-Version: 2.1 Name: emhass Version: 0.8.5 Summary: An Energy Management
 System for Home Assistant Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ Author-email: davidusb@gmail.com Keywords:
 energy,management,optimization,hass Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.11 Classifier:
-Operating System :: OS Independent Requires-Python: >=3.9, <3.12 Description-
+Operating System :: OS Independent Requires-Python: >=3.10, <3.12 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: wheel
 Requires-Dist: numpy==1.26.4 Requires-Dist: scipy==1.12.0 Requires-Dist:
 pandas<=2.0.3 Requires-Dist: pvlib>=0.10.2 Requires-Dist: protobuf>=3.0.0
 Requires-Dist: pytz>=2021.1 Requires-Dist: requests>=2.25.1 Requires-Dist:
 beautifulsoup4>=4.9.3 Requires-Dist: h5py==3.10.0 Requires-Dist: pulp>=2.4
 Requires-Dist: pyyaml>=5.4.1 Requires-Dist: tables<=3.9.1 Requires-Dist:
 skforecast==0.11.0 Requires-Dist: flask>=2.0.3 Requires-Dist: waitress>=2.1.1
```

### Comparing `emhass-0.8.4/README.md` & `emhass-0.8.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -427,16 +427,14 @@
 curl -i -H 'Content-Type:application/json' -X POST -d '{"pv_power_forecast":[0, 70, 141.22, 246.18, 513.5, 753.27, 1049.89, 1797.93, 1697.3, 3078.93], "prediction_horizon":10, "soc_init":0.5,"soc_final":0.6}' http://192.168.3.159:5000/action/naive-mpc-optim
 ```
 *Example with :`def_total_hours`, `def_start_timestep`, `def_end_timestep`.*
 ```bash
 curl -i -H 'Content-Type:application/json' -X POST -d '{"pv_power_forecast":[0, 70, 141.22, 246.18, 513.5, 753.27, 1049.89, 1797.93, 1697.3, 3078.93], "prediction_horizon":10, "soc_init":0.5,"soc_final":0.6,"def_total_hours":[1,3],"def_start_timestep":[0,3],"def_end_timestep":[0,6]}' http://localhost:5000/action/naive-mpc-optim
 ```
 
-
-
 ## A machine learning forecaster
 
 Starting in v0.4.0 a new machine learning forecaster class was introduced.
 This is intended to provide a new and alternative method to forecast your household consumption and use it when such forecast is needed to optimize your energy through the available strategies.
 Check the dedicated section in the documentation here: [https://emhass.readthedocs.io/en/latest/mlforecaster.html](https://emhass.readthedocs.io/en/latest/mlforecaster.html)
 
 ## Development
```

### Comparing `emhass-0.8.4/data/data_load_cost_forecast.csv` & `emhass-0.8.5/data/data_load_cost_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/data_load_forecast.csv` & `emhass-0.8.5/data/data_load_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/data_prod_price_forecast.csv` & `emhass-0.8.5/data/data_prod_price_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/data_train_load_clustering.pkl` & `emhass-0.8.5/data/data_train_load_clustering.pkl`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/data_train_load_forecast.pkl` & `emhass-0.8.5/data/data_train_load_forecast.pkl`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/data_weather_forecast.csv` & `emhass-0.8.5/data/data_weather_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/opt_res_latest.csv` & `emhass-0.8.5/data/opt_res_latest.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/opt_res_perfect_optim_cost.csv` & `emhass-0.8.5/data/opt_res_perfect_optim_cost.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/opt_res_perfect_optim_profit.csv` & `emhass-0.8.5/data/opt_res_perfect_optim_profit.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/opt_res_perfect_optim_self-consumption.csv` & `emhass-0.8.5/data/opt_res_perfect_optim_self-consumption.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/test_df_final.pkl` & `emhass-0.8.5/data/test_df_final.pkl`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/test_response_get_data_get_method.pbz2` & `emhass-0.8.5/data/test_response_get_data_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/test_response_scrapper_get_method.pbz2` & `emhass-0.8.5/data/test_response_scrapper_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/test_response_solarforecast_get_method.pbz2` & `emhass-0.8.5/data/test_response_solarforecast_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/data/test_response_solcast_get_method.pbz2` & `emhass-0.8.5/data/test_response_solcast_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/setup.py` & `emhass-0.8.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='emhass',  # Required
-    version='0.8.4',  # Required
+    version='0.8.5',  # Required
     description='An Energy Management System for Home Assistant',  # Optional
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/davidusb-geek/emhass',  # Optional
     author='David HERNANDEZ',  # Optional
     author_email='davidusb@gmail.com',  # Optional
     classifiers=[  # Optional
@@ -33,15 +33,15 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.11',
         "Operating System :: OS Independent",
     ],
     keywords='energy, management, optimization, hass',  # Optional
     package_dir={'': 'src'},  # Optional
     packages=find_packages(where='src'),  # Required
-    python_requires='>=3.9, <3.12',
+    python_requires='>=3.10, <3.12',
     install_requires=[
         'wheel', 
         'numpy==1.26.4',
         'scipy==1.12.0',
         'pandas<=2.0.3',
         'pvlib>=0.10.2',
         'protobuf>=3.0.0',
@@ -59,9 +59,10 @@
     ],  # Optional
     entry_points={  # Optional
         'console_scripts': [
             'emhass=emhass.command_line:main',
         ],
     },
     package_data={'emhass': ['templates/index.html','templates/template.html','static/advanced.html','static/basic.html', 'static/script.js',
-    'static/style.css','static/img/emhass_icon.png','static/img/emhass_logo_short.svg', 'static/img/feather-sprite.svg']},
+    'static/style.css','static/img/emhass_icon.png','static/img/emhass_logo_short.svg', 'static/img/feather-sprite.svg',
+    'data/cec_modules.pbz2', 'data/cec_inverters.pbz2']},
 )
```

### Comparing `emhass-0.8.4/src/emhass/command_line.py` & `emhass-0.8.5/src/emhass/command_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         config_path, use_secrets=not(get_data_from_file), params=params)
     # Treat runtimeparams
     params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
         runtimeparams, params, retrieve_hass_conf, 
         optim_conf, plant_conf, set_type, logger)
     # Define main objects
     rh = RetrieveHass(retrieve_hass_conf['hass_url'], retrieve_hass_conf['long_lived_token'], 
-                       retrieve_hass_conf['freq'], retrieve_hass_conf['time_zone'], 
-                       params, base_path, logger, get_data_from_file=get_data_from_file)
+                      retrieve_hass_conf['freq'], retrieve_hass_conf['time_zone'], 
+                      params, base_path, logger, get_data_from_file=get_data_from_file)
     fcst = Forecast(retrieve_hass_conf, optim_conf, plant_conf,
                     params, base_path, logger, get_data_from_file=get_data_from_file)
     opt = Optimization(retrieve_hass_conf, optim_conf, plant_conf, 
                        fcst.var_load_cost, fcst.var_prod_price, 
                        costfun, base_path, logger)
     # Perform setup based on type of action
     if set_type == "perfect-optim":
```

### Comparing `emhass-0.8.4/src/emhass/forecast.py` & `emhass-0.8.5/src/emhass/forecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 
 import pathlib
 import pickle
 import copy
 import logging
 import json
 from typing import Optional
+import bz2
+import pickle as cPickle
 import pandas as pd
 import numpy as np
 from datetime import datetime, timedelta
 from requests import get
 from bs4 import BeautifulSoup
 import pvlib
 from pvlib.pvsystem import PVSystem
 from pvlib.location import Location
 from pvlib.modelchain import ModelChain
 from pvlib.temperature import TEMPERATURE_MODEL_PARAMETERS
 from pvlib.irradiance import disc
 
 from emhass.retrieve_hass import RetrieveHass
 from emhass.machine_learning_forecaster import MLForecaster
-from emhass.utils import get_days_list
+from emhass.utils import get_days_list, get_root
 
 
 class Forecast(object):
     r"""
     Generate weather, load and costs forecasts needed as inputs to the optimization.
     
     In EMHASS we have basically 4 forecasts to deal with:
@@ -129,15 +131,15 @@
         self.retrieve_hass_conf = retrieve_hass_conf
         self.optim_conf = optim_conf
         self.plant_conf = plant_conf
         self.freq = self.retrieve_hass_conf['freq']
         self.time_zone = self.retrieve_hass_conf['time_zone']
         self.method_ts_round = self.retrieve_hass_conf['method_ts_round']
         self.timeStep = self.freq.seconds/3600 # in hours
-        self.time_delta = pd.to_timedelta(opt_time_delta, "hours") # The period of optimization
+        self.time_delta = pd.to_timedelta(opt_time_delta, "hours")
         self.var_PV = self.retrieve_hass_conf['var_PV']
         self.var_load = self.retrieve_hass_conf['var_load']
         self.var_load_new = self.var_load+'_positive'
         self.lat = self.retrieve_hass_conf['lat'] 
         self.lon = self.retrieve_hass_conf['lon']
         self.root = base_path
         self.logger = logger
@@ -155,15 +157,15 @@
         elif self.method_ts_round == 'last':
             self.start_forecast = pd.Timestamp(datetime.now(), tz=self.time_zone).replace(microsecond=0).ceil(freq=self.freq)
         else:
             self.logger.error("Wrong method_ts_round passed parameter")
         self.end_forecast = (self.start_forecast + self.optim_conf['delta_forecast']).replace(microsecond=0)
         self.forecast_dates = pd.date_range(start=self.start_forecast, 
                                             end=self.end_forecast-self.freq, 
-                                            freq=self.freq).round(self.freq, ambiguous='infer', nonexistent=self.freq)
+                                            freq=self.freq).round(self.freq, ambiguous='infer', nonexistent='shift_forward')
         if params is not None:
             if 'prediction_horizon' in list(self.params['passed_data'].keys()):
                 if self.params['passed_data']['prediction_horizon'] is not None:
                     self.forecast_dates = self.forecast_dates[0:self.params['passed_data']['prediction_horizon']]
         
         
     def get_weather_forecast(self, method: Optional[str] = 'scrapper',
@@ -180,15 +182,15 @@
         """
         self.logger.info("Retrieving weather forecast data using method = "+method)
         self.weather_forecast_method = method # Saving this attribute for later use to identify csv method usage
         if method == 'scrapper':
             freq_scrap = pd.to_timedelta(60, "minutes") # The scrapping time step is 60min
             forecast_dates_scrap = pd.date_range(start=self.start_forecast,
                                                  end=self.end_forecast-freq_scrap, 
-                                                 freq=freq_scrap).round(freq_scrap, ambiguous='infer', nonexistent=freq_scrap)
+                                                 freq=freq_scrap).round(freq_scrap, ambiguous='infer', nonexistent='shift_forward')
             # Using the clearoutside webpage
             response = get("https://clearoutside.com/forecast/"+str(round(self.lat, 2))+"/"+str(round(self.lon, 2))+"?desktop=true")
             '''import bz2 # Uncomment to save a serialized data for tests
             import _pickle as cPickle
             with bz2.BZ2File("data/test_response_scrapper_get_method.pbz2", "w") as f: 
                 cPickle.dump(response.content, f)'''
             soup = BeautifulSoup(response.content, 'html.parser')
@@ -408,16 +410,18 @@
                 P_PV_forecast = df_weather['yhat']
                 P_PV_forecast.name = None
             else: # We will transform the weather data into electrical power
                 # Transform to power (Watts)
                 # Setting the main parameters of the PV plant
                 location = Location(latitude=self.lat, longitude=self.lon)
                 temp_params = TEMPERATURE_MODEL_PARAMETERS['sapm']['close_mount_glass_glass']
-                cec_modules = pvlib.pvsystem.retrieve_sam('CECMod')
-                cec_inverters = pvlib.pvsystem.retrieve_sam('cecinverter')
+                cec_modules = bz2.BZ2File(get_root(__file__, num_parent=2) / 'emhass/data/cec_modules.pbz2', "rb")
+                cec_modules = cPickle.load(cec_modules)
+                cec_inverters = bz2.BZ2File(get_root(__file__, num_parent=2) / 'emhass/data/cec_inverters.pbz2', "rb")
+                cec_inverters = cPickle.load(cec_inverters)
                 if type(self.plant_conf['module_model']) == list:
                     P_PV_forecast = pd.Series(0, index=df_weather.index)
                     for i in range(len(self.plant_conf['module_model'])):
                         # Selecting correct module and inverter
                         module = cec_modules[self.plant_conf['module_model'][i]]
                         inverter = cec_inverters[self.plant_conf['inverter_model'][i]]
                         # Building the PV system in PVLib
@@ -472,15 +476,15 @@
         elif self.method_ts_round == 'last':
             start_forecast_csv = pd.Timestamp(datetime.now(), tz=self.time_zone).replace(microsecond=0).ceil(freq=self.freq)
         else:
             self.logger.error("Wrong method_ts_round passed parameter")
         end_forecast_csv = (start_forecast_csv + self.optim_conf['delta_forecast']).replace(microsecond=0)
         forecast_dates_csv = pd.date_range(start=start_forecast_csv, 
                                            end=end_forecast_csv+timedelta(days=timedelta_days)-self.freq, 
-                                           freq=self.freq).round(self.freq, ambiguous='infer', nonexistent=self.freq)
+                                           freq=self.freq).round(self.freq, ambiguous='infer', nonexistent='shift_forward')
         if self.params is not None:
             if 'prediction_horizon' in list(self.params['passed_data'].keys()):
                 if self.params['passed_data']['prediction_horizon'] is not None:
                     forecast_dates_csv = forecast_dates_csv[0:self.params['passed_data']['prediction_horizon']]
         return forecast_dates_csv
     
     def get_forecast_out_from_csv(self, df_final: pd.DataFrame, forecast_dates_csv: pd.date_range,
```

### Comparing `emhass-0.8.4/src/emhass/machine_learning_forecaster.py` & `emhass-0.8.5/src/emhass/machine_learning_forecaster.py`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/src/emhass/optimization.py` & `emhass-0.8.5/src/emhass/optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,18 +158,18 @@
         
         n = len(data_opt.index)
         set_I = range(n)
         M = 10e10
         
         ## Add decision variables
         P_grid_neg  = {(i):plp.LpVariable(cat='Continuous',
-                                          lowBound=-self.plant_conf['P_grid_max'], upBound=0,
+                                          lowBound=-self.plant_conf['P_to_grid_max'], upBound=0,
                                           name="P_grid_neg{}".format(i)) for i in set_I}
         P_grid_pos  = {(i):plp.LpVariable(cat='Continuous',
-                                          lowBound=0, upBound=self.plant_conf['P_grid_max'],
+                                          lowBound=0, upBound=self.plant_conf['P_from_grid_max'],
                                           name="P_grid_pos{}".format(i)) for i in set_I}
         P_deferrable = []
         P_def_bin1 = []
         for k in range(self.optim_conf['num_def_loads']):
             if self.optim_conf['treat_def_as_semi_cont'][k]:
                 P_deferrable.append({(i):plp.LpVariable(cat='Continuous',
                                                         name="P_deferrable{}_{}".format(k, i)) for i in set_I})
@@ -263,21 +263,21 @@
                         sense = plp.LpConstraintLE,
                         rhs = 0)
                     for i in set_I})
         
         # Avoid injecting and consuming from grid at the same time
         constraints.update({"constraint_pgridpos_{}".format(i) : 
             plp.LpConstraint(
-                e = P_grid_pos[i] - self.plant_conf['P_grid_max']*D[i],
+                e = P_grid_pos[i] - self.plant_conf['P_from_grid_max']*D[i],
                 sense = plp.LpConstraintLE,
                 rhs = 0)
             for i in set_I})
         constraints.update({"constraint_pgridneg_{}".format(i) : 
             plp.LpConstraint(
-                e = -P_grid_neg[i] - self.plant_conf['P_grid_max']*(1-D[i]),
+                e = -P_grid_neg[i] - self.plant_conf['P_to_grid_max']*(1-D[i]),
                 sense = plp.LpConstraintLE,
                 rhs = 0)
             for i in set_I})
             
         # Treat deferrable loads constraints
         for k in range(self.optim_conf['num_def_loads']):
             # Total time of deferrable load
```

### Comparing `emhass-0.8.4/src/emhass/retrieve_hass.py` & `emhass-0.8.5/src/emhass/retrieve_hass.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,31 +129,31 @@
                 '''import bz2 # Uncomment to save a serialized data for tests
                 import _pickle as cPickle
                 with bz2.BZ2File("data/test_response_get_data_get_method.pbz2", "w") as f: 
                     cPickle.dump(response, f)'''
                 try: # Sometimes when there are connection problems we need to catch empty retrieved json
                     data = response.json()[0]
                 except IndexError:
-                    if x is 0:
+                    if x == 0:
                         self.logger.error("The retrieved JSON is empty, A sensor:" + var + " may have 0 days of history or passed sensor may not be correct")
                     else:
                         self.logger.error("The retrieved JSON is empty for day:"+ str(day) +", days_to_retrieve may be larger than the recorded history of sensor:" + var + " (check your recorder settings)")
                     return False
                 df_raw = pd.DataFrame.from_dict(data)
                 if len(df_raw) == 0:
-                    if x is 0:
+                    if x == 0:
                         self.logger.error("The retrieved Dataframe is empty, A sensor:" + var + " may have 0 days of history or passed sensor may not be correct")
                     else:
                         self.logger.error("Retrieved empty Dataframe for day:"+ str(day) +", days_to_retrieve may be larger than the recorded history of sensor:" + var + " (check your recorder settings)")
                     return False
                 if i == 0: # Defining the DataFrame container
                     from_date = pd.to_datetime(df_raw['last_changed'], format="ISO8601").min()
                     to_date = pd.to_datetime(df_raw['last_changed'], format="ISO8601").max()
                     ts = pd.to_datetime(pd.date_range(start=from_date, end=to_date, freq=self.freq), 
-                                        format='%Y-%d-%m %H:%M').round(self.freq, ambiguous='infer', nonexistent=self.freq)
+                                        format='%Y-%d-%m %H:%M').round(self.freq, ambiguous='infer', nonexistent='shift_forward')
                     df_day = pd.DataFrame(index = ts)
                 # Caution with undefined string data: unknown, unavailable, etc.
                 df_tp = df_raw.copy()[['state']].replace(
                     ['unknown', 'unavailable', ''], np.nan).astype(float).rename(columns={'state': var})
                 # Setting index, resampling and concatenation
                 df_tp.set_index(pd.to_datetime(df_raw['last_changed'], format="ISO8601"), inplace=True)
                 df_tp = df_tp.resample(self.freq).mean()
```

### Comparing `emhass-0.8.4/src/emhass/static/advanced.html` & `emhass-0.8.5/src/emhass/static/advanced.html`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/src/emhass/static/basic.html` & `emhass-0.8.5/src/emhass/static/basic.html`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/src/emhass/static/img/emhass_icon.png` & `emhass-0.8.5/src/emhass/static/img/emhass_icon.png`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/src/emhass/static/img/emhass_logo_short.svg` & `emhass-0.8.5/src/emhass/static/img/emhass_logo_short.svg`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/src/emhass/static/img/feather-sprite.svg` & `emhass-0.8.5/src/emhass/static/img/feather-sprite.svg`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/src/emhass/static/script.js` & `emhass-0.8.5/src/emhass/static/script.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,16 @@
-//before page load check for stylesheet
-document.onreadystatechange = async function() {
-    checkStyleSheets()
-}
-
 //on page reload get saved data
 window.onload = async function() {
 
     pageSelected = await loadBasicOrAdvanced();
 
     //add listener for basic and advanced html switch
     document.getElementById("basicOrAdvanced").addEventListener("click", () => SwitchBasicOrAdvanced());
 };
 
-//check style sheet is loaded 
-async function checkStyleSheets() {
-    var styleHREF = getHTMLURL() + `static/style.css`
-    var styles = document.styleSheets;
-    for (var i = 0; i < styles.length; i++) {
-        if (styles[i].href.match("style")["input"] == styleHREF) {
-            return true
-        }
-    }
-    //if could not find file
-    var style = document.createElement("link");
-    style.rel = "stylesheet";
-    style.href = styleHREF;
-    style.type = "text/css";
-    document.getElementsByTagName("head")[0].appendChild(style);
-}
-
 //add listeners to buttons (based on page)
 function loadButtons(page) {
     switch (page) {
         case "advanced":
             [
                 "dayahead-optim",
                 "forecast-model-fit",
@@ -118,28 +96,18 @@
     if (formContainerChildID === 'basic') {
         loadBasicOrAdvanced("advanced")
     } else {
         loadBasicOrAdvanced("basic")
     }
 }
 
-//set current url
-function getHTMLURL() {
-    var currentUrl
-    if (window.location) {
-        currentUrl = window.location.href; //get current url to append
-    } else {
-        currentUrl = ""
-    }
-    return currentUrl
-}
 
 //get html data from basic.html or advanced.html
 async function getHTMLData(htmlFile) {
-    const response = await fetch(getHTMLURL() + `static/` + htmlFile);
+    const response = await fetch(`static/` + htmlFile);
     blob = await response.blob(); //get data blob
     htmlTemplateData = await new Response(blob).text(); //obtain html from blob
     return await htmlTemplateData;
 }
 
 //function pushing data via post, triggered by button action
 async function formAction(action, page) {
@@ -148,15 +116,15 @@
         var data = inputToJson(page);
     } else {
         var data = {}
     } //send no data
 
     if (data !== 0) { //don't run if there is an error in the input (box/list) Json data
         showChangeStatus("loading", {}); // show loading div for status
-        const response = await fetch(getHTMLURL() + `action/${action}`, {
+        const response = await fetch(`action/` + action, {
             //fetch data from webserver.py
             method: "POST",
             headers: {
                 "Content-Type": "application/json",
             },
             body: JSON.stringify(data), //note that post can only send data via strings
         });
@@ -206,15 +174,15 @@
     }
 }
 
 //get rendered html template with containing new table data
 async function getTemplate() {
     //fetch data from webserver.py
     let htmlTemplateData = "";
-    response = await fetch(getHTMLURL() + `template/table-template`, {
+    response = await fetch(`template/table-template`, {
         method: "GET",
     });
     blob = await response.blob(); //get data blob
     htmlTemplateData = await new Response(blob).text(); //obtain html from blob
     templateDiv = document.getElementById("template"); //get template container element to override
     templateDiv.innerHTML = htmlTemplateData; //override container inner html with new data
     var scripts = Array.from(templateDiv.getElementsByTagName("script")); //replace script tags manually
```

### Comparing `emhass-0.8.4/src/emhass/static/style.css` & `emhass-0.8.5/src/emhass/static/style.css`

 * *Files 7% similar despite different names*

```diff
@@ -546,24 +546,24 @@
   width: 27px !important;
   height: 27px !important;
   stroke: currentColor !important;
   stroke-width: 2 !important;
   stroke-linecap: round !important;
   stroke-linejoin: round !important;
   fill: none !important;
-  filter: drop-shadow( #282928 .2px .2px) !important;
+  filter: drop-shadow(#282928 .2px .2px) !important;
   -webkit-text-size-adjust: none !important;
   -ms-text-size-adjust: none !important;
 
 }
 
-/* feather icons no background color */ 
+/* feather icons no background color */
 #top-links a {
   background: none !important;
-} 
+}
 
 /* -------------- */
 
 /* EMHASS added style */
 /* set rounded element radius */
 button,
 .main-svg,
@@ -582,29 +582,30 @@
   text-transform: none;
   border-width: 1px;
   border-style: solid;
   box-shadow: #3d3d3d 3px 3px;
 }
 
 
-.alert, .info {
+.alert,
+.info {
   max-width: 50%;
 }
 
 .info {
   margin: 0 auto;
   margin-top: 2em;
   padding-top: 1em;
 }
 
 h2 {
   margin-bottom: .3em;
 }
 
-.table_div h4{
+.table_div h4 {
   margin-top: .5em;
 }
 
 .info p {
   line-height: 2em;
 }
 
@@ -679,25 +680,57 @@
 
 .mystyle td {
   padding: 5px;
 }
 
 th {
   padding: 5px 7.77px;
+  text-align: center;
 }
 
-.mystyle tr:nth-child(even) {
+.mystyle tr:nth-child(even) td,
+th {
   background: #e1e1e1;
 }
 
-.mystyle tr:hover {
-  background: silver;
+.mystyle tr:nth-child(odd) td {
+  background: white;
+}
+
+.mystyle tr:hover td {
+  background-color: silver;
   cursor: pointer;
 }
 
+th:last-child {
+  border-top-right-radius: 7px;
+}
+
+th:first-child {
+  border-top-left-radius: 7px;
+}
+
+tr:last-child td:first-child {
+  border-bottom-left-radius: 7px;
+}
+
+tr:last-child td:last-child {
+  border-bottom-right-radius: 7px;
+}
+
+tr:hover td:first-child {
+  border-top-left-radius: 7px;
+  border-bottom-left-radius: 7px;
+}
+
+tr:hover td:last-child {
+  border-top-right-radius: 7px;
+  border-bottom-right-radius: 7px;
+}
+
 #top-links {
   display: flex;
   position: absolute;
   right: 13px;
   top: 13px;
 }
 
@@ -791,22 +824,28 @@
 
   100% {
     opacity: 1;
   }
 }
 
 /* Basic and Advanced fade transitions */
-.TabSelection, #advance, #basic, button, select, .info {
+.TabSelection,
+#advance,
+#basic,
+button,
+select,
+.info {
   animation-name: fadeInOpacity;
   animation-iteration-count: 1;
   animation-timing-function: ease-in-out;
   animation-duration: .3s;
 }
 
-.input-list, .input-box {
+.input-list,
+.input-box {
   animation-name: fadeInOpacity;
   animation-iteration-count: 1;
   animation-timing-function: ease-in-out;
   animation-duration: .1s;
 }
 
 /* Alert box styling */
@@ -940,36 +979,39 @@
   /* modbar disable drag layer and buttons*/
   .modebar-group:has(a[data-attr=dragmode]),
   .draglayer,
   .layer-below {
     display: none !important;
   }
 
-  .info, .alert {
+  .info,
+  .alert {
     max-width: 100%;
   }
 }
 
 /* Dark Theme Support */
 @media (prefers-color-scheme: dark) {
   html.adaptive {
     background: #111111;
     color: #e1e1e1;
   }
 
   img,
-  figure, svg.main-svg{
+  figure,
+  svg.main-svg {
     -webkit-filter: invert(.82);
     filter: invert(.82);
   }
-  
-  figure, svg.main-svg{
-  border-color: #181818;
-  border-style: solid;
-  border-width: 1px;
+
+  figure,
+  svg.main-svg {
+    border-color: #181818;
+    border-style: solid;
+    border-width: 1px;
   }
 
   button,
   .alert,
   .info,
   select {
     color: #e1e1e1;
@@ -1004,61 +1046,54 @@
   a:active {
     color: #aaccd6;
   }
 
   .modebar-btn svg path {
     fill: #111 !important;
   }
+
   .modebar-btn svg {
-    filter:invert(100%) sepia(64%) saturate(2%) hue-rotate(294deg) brightness(85%) contrast(93%) !important
+    filter: invert(100%) sepia(64%) saturate(2%) hue-rotate(294deg) brightness(85%) contrast(93%) !important
   }
-  .modebar-btn--logo svg{
+
+  .modebar-btn--logo svg {
     filter: None !important;
     /* filter: invert(100%) saturate(100%) brightness(87%) contrast(100%) !important */
   }
 
   .g-gtitle,
   .g-xtitle,
   .g-ytitle,
   legend,
   th {
     color: #e1e1e1;
   }
 
-  tr td:nth-child(even),
-  .mystyle tr td:nth-child(even) {
-    background-color: #3d3d3d;
+  .mystyle tr {
+    background: none;
   }
 
-  tr:nth-child(odd),
-  .mystyle tr:nth-child(odd) {
-    background-color: #111111;
+  .mystyle tr:nth-child(even) td,
+  th {
+    background: #282928;
   }
 
-  tr:nth-child(even),
-  .mystyle tr:nth-child(even) {
-    background-color: #181818;
+  .mystyle tr:nth-child(odd) td {
+    background: #111111;
   }
 
-  tr:hover td,
-  th {
+  .mystyle tr:hover td {
     background-color: #3f3f3f;
   }
 
-  tr:hover td,
-  th:last-child, th:first-child, td:first-child, td:last-child
-  {
-    border-radius: 7px
-  }
-
-  .modebar-group{
+  .modebar-group {
     background-color: #0000 !important;
   }
 
-  .modebar-btn{
+  .modebar-btn {
     background: #3f3f3f;
   }
 
   .input-list input,
   .input-box textarea {
     background-color: #282928;
     border-color: #e1e1e1;
@@ -1072,8 +1107,8 @@
   .loading {
     /* loading animation  */
     border: 16px solid #282928;
     border-top: 16px solid #ccf3ff;
   }
 
 
-}
+}
```

### Comparing `emhass-0.8.4/src/emhass/templates/index.html` & `emhass-0.8.5/src/emhass/templates/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 <!DOCTYPE html>
 <html class="adaptive">
 
 <head>
     <title>EMHASS: Energy Management Optimization for Home Assistant</title>
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <link rel="stylesheet" type="text/css" href="{{ basename }}/static/style.css">
-    <link rel="icon" type="image/x-icon" href="{{ basename }}/static/img/emhass_logo_short.svg">
-    <script src="{{ basename }}/static/script.js"></script>
+    <link rel="stylesheet" type="text/css" href="static/style.css?version=1"> <!-- change version on stylesheet changes  -->
+    <link rel="icon" type="image/x-icon" href="static/img/emhass_logo_short.svg">
+    <script src="static/script.js"></script>
 </head>
 
 <body style="margin: auto; align-items:center; text-align:center;">
 
     <div>
         <!-- Icons by feather https://github.com/feathericons/feather -->
         <div id="top-links">
             <!-- advanced or basic page switch -->
             <a id="basicOrAdvanced" style="margin-right: 24px; cursor: pointer; z-index: 1">
                 <svg class="feather">
-                    <use class="feather" href="{{ basename }}/static/img/feather-sprite.svg#tool" />
+                    <use class="feather" href="static/img/feather-sprite.svg#tool" />
                 </svg>
             </a>
             <a href="https://emhass.readthedocs.io/en/latest/">
                 <svg class="feather" style="margin-right: 12px;";>
-                    <use class="feather" href="{{ basename }}/static/img/feather-sprite.svg#book" />
+                    <use class="feather" href="static/img/feather-sprite.svg#book" />
                 </svg>
             </a>
             <a href="https://github.com/davidusb-geek/emhass" target="_blank" rel="noopener noreferrer">
                 <svg class="feather" style="margin-right: 0px;" >
-                    <use class="feather" href="{{ basename }}/static/img/feather-sprite.svg#git-branch" />
+                    <use class="feather" href="static/img/feather-sprite.svg#git-branch" />
                 </svg>
             </a>
         </div>
         <!-- Title -->
-        <img src="{{ basename }}/static/img/emhass_icon.png" alt="">
+        <img src="static/img/emhass_icon.png" alt="">
         <h2>EMHASS: Energy Management Optimization for Home Assistant</h2>
     </div>
 
 
     <div class="center">
         <div id=TabSelection class="form">
             <!-- Basic and Advance pages will be loaded here  -->
```

### Comparing `emhass-0.8.4/src/emhass/utils.py` & `emhass-0.8.5/src/emhass/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     
     """
     freq = pd.to_timedelta(freq, "minutes")
     start_forecast = pd.Timestamp(datetime.now()).replace(hour=0, minute=0, second=0, microsecond=0)
     end_forecast = (start_forecast + pd.Timedelta(days=delta_forecast)).replace(microsecond=0)
     forecast_dates = pd.date_range(start=start_forecast, 
         end=end_forecast+timedelta(days=timedelta_days)-freq, 
-        freq=freq).round(freq, ambiguous='infer', nonexistent=freq)
+        freq=freq).round(freq, ambiguous='infer', nonexistent='shift_forward')
     return forecast_dates
 
 def treat_runtimeparams(runtimeparams: str, params: str, retrieve_hass_conf: dict, optim_conf: dict, plant_conf: dict,
                         set_type: str, logger: logging.Logger) -> Tuple[str, dict]:
     """
     Treat the passed optimization runtime parameters. 
     
@@ -204,70 +204,31 @@
             params['passed_data']['soc_final'] = None
             params['passed_data']['def_total_hours'] = None
             params['passed_data']['def_start_timestep'] = None
             params['passed_data']['def_end_timestep'] = None
             params['passed_data']['alpha'] = None
             params['passed_data']['beta'] = None
         # Treat passed forecast data lists
-        if 'pv_power_forecast' in runtimeparams.keys():
-            if type(runtimeparams['pv_power_forecast']) == list and len(runtimeparams['pv_power_forecast']) >= len(forecast_dates):
-                params['passed_data']['pv_power_forecast'] = runtimeparams['pv_power_forecast']
-                optim_conf['weather_forecast_method'] = 'list'
+        list_forecast_key = ['pv_power_forecast', 'load_power_forecast', 'load_cost_forecast', 'prod_price_forecast']
+        forecast_methods = ['weather_forecast_method', 'load_forecast_method', 'load_cost_forecast_method', 'prod_price_forecast_method']
+        for method, forecast_key in enumerate(list_forecast_key):
+            if forecast_key in runtimeparams.keys():
+                if type(runtimeparams[forecast_key]) == list and len(runtimeparams[forecast_key]) >= len(forecast_dates):
+                    params['passed_data'][forecast_key] = runtimeparams[forecast_key]
+                    optim_conf[forecast_methods[method]] = 'list'
+                else:
+                    logger.error(f"ERROR: The passed data is either not a list or the length is not correct, length should be {str(len(forecast_dates))}")
+                    logger.error(f"Passed type is {str(type(runtimeparams[forecast_key]))} and length is {str(len(runtimeparams[forecast_key]))}")
+                list_non_digits = [x for x in runtimeparams[forecast_key] if not (isinstance(x, int) or isinstance(x, float))]
+                if len(list_non_digits) > 0:
+                    logger.warning(f"There are non numeric values on the passed data for {forecast_key}, check for missing values (nans, null, etc)")
+                    for x in list_non_digits:
+                        logger.warning(f"This value in {forecast_key} was detected as non digits: {str(x)}")
             else:
-                logger.error("ERROR: The passed data is either not a list or the length is not correct, length should be "+str(len(forecast_dates)))
-                logger.error("Passed type is "+str(type(runtimeparams['pv_power_forecast']))+" and length is "+str(len(runtimeparams['pv_power_forecast'])))
-            list_non_digits = [x for x in runtimeparams['pv_power_forecast'] if not (isinstance(x, int) or isinstance(x, float))]
-            if len(list_non_digits) > 0:
-                logger.warning("There are non numeric values on the passed data for pv_power_forecast, check for missing values (nans, null, etc)")
-                for x in list_non_digits:
-                    logger.warning("This value in pv_power_forecast was detected as non digits: "+str(x))
-        else:
-            params['passed_data']['pv_power_forecast'] = None
-        if 'load_power_forecast' in runtimeparams.keys():
-            if type(runtimeparams['load_power_forecast']) == list and len(runtimeparams['load_power_forecast']) >= len(forecast_dates):
-                params['passed_data']['load_power_forecast'] = runtimeparams['load_power_forecast']
-                optim_conf['load_forecast_method'] = 'list'
-            else:
-                logger.error("ERROR: The passed data is either not a list or the length is not correct, length should be "+str(len(forecast_dates)))
-                logger.error("Passed type is "+str(type(runtimeparams['load_power_forecast']))+" and length is "+str(len(runtimeparams['load_power_forecast'])))
-            list_non_digits = [x for x in runtimeparams['load_power_forecast'] if not (isinstance(x, int) or isinstance(x, float))]
-            if len(list_non_digits) > 0:
-                logger.warning("There are non numeric values on the passed data for load_power_forecast, check for missing values (nans, null, etc)")
-                for x in list_non_digits:
-                    logger.warning("This value in load_power_forecast was detected as non digits: "+str(x))
-        else:
-            params['passed_data']['load_power_forecast'] = None
-        if 'load_cost_forecast' in runtimeparams.keys():
-            if type(runtimeparams['load_cost_forecast']) == list and len(runtimeparams['load_cost_forecast']) >= len(forecast_dates):
-                params['passed_data']['load_cost_forecast'] = runtimeparams['load_cost_forecast']
-                optim_conf['load_cost_forecast_method'] = 'list'
-            else:
-                logger.error("ERROR: The passed data is either not a list or the length is not correct, length should be "+str(len(forecast_dates)))
-                logger.error("Passed type is "+str(type(runtimeparams['load_cost_forecast']))+" and length is "+str(len(runtimeparams['load_cost_forecast'])))
-            list_non_digits = [x for x in runtimeparams['load_cost_forecast'] if not (isinstance(x, int) or isinstance(x, float))]
-            if len(list_non_digits) > 0:
-                logger.warning("There are non numeric values on the passed data or load_cost_forecast, check for missing values (nans, null, etc)")
-                for x in list_non_digits:
-                    logger.warning("This value in load_cost_forecast was detected as non digits: "+str(x))
-        else:
-            params['passed_data']['load_cost_forecast'] = None
-        if 'prod_price_forecast' in runtimeparams.keys():
-            if type(runtimeparams['prod_price_forecast']) == list and len(runtimeparams['prod_price_forecast']) >= len(forecast_dates):
-                params['passed_data']['prod_price_forecast'] = runtimeparams['prod_price_forecast']
-                optim_conf['prod_price_forecast_method'] = 'list'
-            else:
-                logger.error("ERROR: The passed data is either not a list or the length is not correct, length should be "+str(len(forecast_dates)))
-                logger.error("Passed type is "+str(type(runtimeparams['prod_price_forecast']))+" and length is "+str(len(runtimeparams['prod_price_forecast'])))
-            list_non_digits = [x for x in runtimeparams['prod_price_forecast'] if not (isinstance(x, int) or isinstance(x, float))]
-            if len(list_non_digits) > 0:
-                logger.warning("There are non numeric values on the passed data for prod_price_forecast, check for missing values (nans, null, etc)")
-                for x in list_non_digits:
-                    logger.warning("This value in prod_price_forecast was detected as non digits: "+str(x))
-        else:
-            params['passed_data']['prod_price_forecast'] = None
+                params['passed_data'][forecast_key] = None
         # Treat passed data for forecast model fit/predict/tune at runtime
         if 'days_to_retrieve' not in runtimeparams.keys():
             days_to_retrieve = 9
         else:
             days_to_retrieve = runtimeparams['days_to_retrieve']
         params['passed_data']['days_to_retrieve'] = days_to_retrieve
         if 'model_type' not in runtimeparams.keys():
@@ -630,16 +591,17 @@
         params['optim_conf']['battery_dynamic_min'] = options.get('battery_dynamic_min',params['optim_conf']['battery_dynamic_min'])
         params['optim_conf']['weight_battery_discharge'] = options.get('weight_battery_discharge',params['optim_conf']['weight_battery_discharge'])
         params['optim_conf']['weight_battery_charge'] = options.get('weight_battery_charge',params['optim_conf']['weight_battery_charge'])
         if options.get('list_start_timesteps_of_each_deferrable_load',None) != None: 
             params['optim_conf']['def_start_timestep'] = [i['start_timesteps_of_each_deferrable_load'] for i in options.get('list_start_timesteps_of_each_deferrable_load')]
         if options.get('list_end_timesteps_of_each_deferrable_load',None) != None: 
             params['optim_conf']['def_end_timestep'] = [i['end_timesteps_of_each_deferrable_load'] for i in options.get('list_end_timesteps_of_each_deferrable_load')]
-        # Updating variables in plant_con
-            params['plant_conf']['P_grid_max'] = options.get('maximum_power_from_grid',params['plant_conf']['P_grid_max'])
+        # Updating variables in plant_conf
+        params['plant_conf']['P_from_grid_max'] = options.get('maximum_power_from_grid',params['plant_conf']['P_from_grid_max'])
+        params['plant_conf']['P_to_grid_max'] = options.get('maximum_power_to_grid',params['plant_conf']['P_to_grid_max'])
         if options.get('list_pv_module_model',None) != None:         
             params['plant_conf']['module_model'] = [i['pv_module_model'] for i in options.get('list_pv_module_model')]
         if options.get('list_pv_inverter_model',None) != None:        
             params['plant_conf']['inverter_model'] = [i['pv_inverter_model'] for i in options.get('list_pv_inverter_model')]
         if options.get('list_surface_tilt',None) != None:        
             params['plant_conf']['surface_tilt'] = [i['surface_tilt'] for i in options.get('list_surface_tilt')]
         if options.get('list_surface_azimuth',None) != None:         
@@ -652,16 +614,15 @@
         params['plant_conf']['Pc_max'] = options.get('battery_charge_power_max',params['plant_conf']['Pc_max'])
         params['plant_conf']['eta_disch'] = options.get('battery_discharge_efficiency',params['plant_conf']['eta_disch'])
         params['plant_conf']['eta_ch'] = options.get('battery_charge_efficiency',params['plant_conf']['eta_ch'])
         params['plant_conf']['Enom'] = options.get('battery_nominal_energy_capacity',params['plant_conf']['Enom'])
         params['plant_conf']['SOCmin'] = options.get('battery_minimum_state_of_charge',params['plant_conf']['SOCmin']) 
         params['plant_conf']['SOCmax'] = options.get('battery_maximum_state_of_charge',params['plant_conf']['SOCmax']) 
         params['plant_conf']['SOCtarget'] = options.get('battery_target_state_of_charge',params['plant_conf']['SOCtarget'])
-
-                # Check parameter lists have the same amounts as deferrable loads
+        # Check parameter lists have the same amounts as deferrable loads
         # If not, set defaults it fill in gaps
         if params['optim_conf']['num_def_loads'] is not len(params['optim_conf']['def_start_timestep']):
             logger.warning("def_start_timestep / list_start_timesteps_of_each_deferrable_load does not match number in num_def_loads, adding default values to parameter")
             for x in range(len(params['optim_conf']['def_start_timestep']), params['optim_conf']['num_def_loads']):
                 params['optim_conf']['def_start_timestep'].append(0)
         if params['optim_conf']['num_def_loads'] is not len(params['optim_conf']['def_end_timestep']):
             logger.warning("def_end_timestep / list_end_timesteps_of_each_deferrable_load does not match number in num_def_loads, adding default values to parameter")
@@ -679,18 +640,14 @@
             logger.warning("def_total_hours / list_operating_hours_of_each_deferrable_load does not match number in num_def_loads, adding default values to parameter")
             for x in range(len(params['optim_conf']['def_total_hours']), params['optim_conf']['num_def_loads']):
                 params['optim_conf']['def_total_hours'].append(0)                   
         if params['optim_conf']['num_def_loads'] is not len(params['optim_conf']['P_deferrable_nom']):
             logger.warning("P_deferrable_nom / list_nominal_power_of_deferrable_loads does not match number in num_def_loads, adding default values to parameter")
             for x in range(len(params['optim_conf']['P_deferrable_nom']), params['optim_conf']['num_def_loads']):
                 params['optim_conf']['P_deferrable_nom'].append(0)   
-        if params['optim_conf']['num_def_loads'] is not len(params['optim_conf']['list_hp_periods']):
-            logger.warning("list_hp_periods / list_peak_hours_periods_(start&end)_hours does not match number in num_def_loads, adding default values to parameter")
-            for x in range(len(params['optim_conf']['list_hp_periods']), params['optim_conf']['num_def_loads']):
-                params['optim_conf']['list_hp_periods'].append({'period_hp_'+str(x+1):[{'start':'02:54'},{'end':'20:24'}]})
         # days_to_retrieve should be no less then 2
         if params['retrieve_hass_conf']['days_to_retrieve'] < 2:
             params['retrieve_hass_conf']['days_to_retrieve'] = 2
             logger.warning("days_to_retrieve should not be lower then 2, setting days_to_retrieve to 2. Make sure your sensors also have at least 2 days of history")
     else:
         params['params_secrets'] = params_secrets
     # The params dict
```

### Comparing `emhass-0.8.4/src/emhass/web_server.py` & `emhass-0.8.5/src/emhass/web_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,21 @@
     # Load cache dict
     if (data_path / 'injection_dict.pkl').exists():
         with open(str(data_path / 'injection_dict.pkl'), "rb") as fid:
             injection_dict = pickle.load(fid)
     else:
         app.logger.warning("The data container dictionary is empty... Please launch an optimization task")
         injection_dict={}
-    basename = request.headers.get("X-Ingress-Path", "")
-    return make_response(template.render(injection_dict=injection_dict, basename=basename))
+
+    # replace {{basename}} in html template html with path root  
+    # basename = request.headers.get("X-Ingress-Path", "")
+    # return make_response(template.render(injection_dict=injection_dict, basename=basename))
+    
+    return make_response(template.render(injection_dict=injection_dict))
+
 
 #get actions 
 @app.route('/template/<action_name>', methods=['GET'])
 def template_action(action_name):
     app.logger.info(" >> Sending rendered template table data")
     if action_name == 'table-template':
         file_loader = PackageLoader('emhass', 'templates')
@@ -82,16 +87,15 @@
         template = env.get_template('template.html')
         if (data_path / 'injection_dict.pkl').exists():
             with open(str(data_path / 'injection_dict.pkl'), "rb") as fid:
                 injection_dict = pickle.load(fid)
         else:
             app.logger.warning("The data container dictionary is empty... Please launch an optimization task")
             injection_dict={}        
-        basename = request.headers.get("X-Ingress-Path", "")    
-        return make_response(template.render(injection_dict=injection_dict, basename=basename))
+        return make_response(template.render(injection_dict=injection_dict))
 
 #post actions 
 @app.route('/action/<action_name>', methods=['POST'])
 def action_call(action_name):
     with open(str(data_path / 'params.pkl'), "rb") as fid:
         config_path, params = pickle.load(fid)
     runtimeparams = request.get_json(force=True)
```

### Comparing `emhass-0.8.4/src/emhass.egg-info/PKG-INFO` & `emhass-0.8.5/src/emhass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: emhass
-Version: 0.8.4
+Version: 0.8.5
 Summary: An Energy Management System for Home Assistant
 Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ
 Author-email: davidusb@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9, <3.12
+Requires-Python: >=3.10, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
 Requires-Dist: numpy==1.26.4
 Requires-Dist: scipy==1.12.0
 Requires-Dist: pandas<=2.0.3
 Requires-Dist: pvlib>=0.10.2
@@ -462,16 +462,14 @@
 curl -i -H 'Content-Type:application/json' -X POST -d '{"pv_power_forecast":[0, 70, 141.22, 246.18, 513.5, 753.27, 1049.89, 1797.93, 1697.3, 3078.93], "prediction_horizon":10, "soc_init":0.5,"soc_final":0.6}' http://192.168.3.159:5000/action/naive-mpc-optim
 ```
 *Example with :`def_total_hours`, `def_start_timestep`, `def_end_timestep`.*
 ```bash
 curl -i -H 'Content-Type:application/json' -X POST -d '{"pv_power_forecast":[0, 70, 141.22, 246.18, 513.5, 753.27, 1049.89, 1797.93, 1697.3, 3078.93], "prediction_horizon":10, "soc_init":0.5,"soc_final":0.6,"def_total_hours":[1,3],"def_start_timestep":[0,3],"def_end_timestep":[0,6]}' http://localhost:5000/action/naive-mpc-optim
 ```
 
-
-
 ## A machine learning forecaster
 
 Starting in v0.4.0 a new machine learning forecaster class was introduced.
 This is intended to provide a new and alternative method to forecast your household consumption and use it when such forecast is needed to optimize your energy through the available strategies.
 Check the dedicated section in the documentation here: [https://emhass.readthedocs.io/en/latest/mlforecaster.html](https://emhass.readthedocs.io/en/latest/mlforecaster.html)
 
 ## Development
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: emhass Version: 0.8.4 Summary: An Energy Management
+Metadata-Version: 2.1 Name: emhass Version: 0.8.5 Summary: An Energy Management
 System for Home Assistant Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ Author-email: davidusb@gmail.com Keywords:
 energy,management,optimization,hass Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.11 Classifier:
-Operating System :: OS Independent Requires-Python: >=3.9, <3.12 Description-
+Operating System :: OS Independent Requires-Python: >=3.10, <3.12 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: wheel
 Requires-Dist: numpy==1.26.4 Requires-Dist: scipy==1.12.0 Requires-Dist:
 pandas<=2.0.3 Requires-Dist: pvlib>=0.10.2 Requires-Dist: protobuf>=3.0.0
 Requires-Dist: pytz>=2021.1 Requires-Dist: requests>=2.25.1 Requires-Dist:
 beautifulsoup4>=4.9.3 Requires-Dist: h5py==3.10.0 Requires-Dist: pulp>=2.4
 Requires-Dist: pyyaml>=5.4.1 Requires-Dist: tables<=3.9.1 Requires-Dist:
 skforecast==0.11.0 Requires-Dist: flask>=2.0.3 Requires-Dist: waitress>=2.1.1
```

### Comparing `emhass-0.8.4/src/emhass.egg-info/SOURCES.txt` & `emhass-0.8.5/src/emhass.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 src/emhass/web_server.py
 src/emhass.egg-info/PKG-INFO
 src/emhass.egg-info/SOURCES.txt
 src/emhass.egg-info/dependency_links.txt
 src/emhass.egg-info/entry_points.txt
 src/emhass.egg-info/requires.txt
 src/emhass.egg-info/top_level.txt
+src/emhass/data/cec_inverters.pbz2
+src/emhass/data/cec_modules.pbz2
 src/emhass/static/advanced.html
 src/emhass/static/basic.html
 src/emhass/static/script.js
 src/emhass/static/style.css
 src/emhass/static/img/emhass_icon.png
 src/emhass/static/img/emhass_logo_short.svg
 src/emhass/static/img/feather-sprite.svg
```

### Comparing `emhass-0.8.4/tests/test_command_line_utils.py` & `emhass-0.8.5/tests/test_command_line_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,18 +35,18 @@
             }
             })
         return params
 
     def setUp(self):
         params = TestCommandLineUtils.get_test_params()
         runtimeparams = {
-            'pv_power_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48],
-            'load_power_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48],
-            'load_cost_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48],
-            'prod_price_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48]
+            'pv_power_forecast':[i+1 for i in range(48)],
+            'load_power_forecast':[i+1 for i in range(48)],
+            'load_cost_forecast':[i+1 for i in range(48)],
+            'prod_price_forecast':[i+1 for i in range(48)]
         }
         self.runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         self.params_json = json.dumps(params)
         
     def test_set_input_data_dict(self):
         config_path = pathlib.Path(root+'/config_emhass.yaml')
@@ -109,16 +109,16 @@
         self.assertTrue(input_data_dict['df_input_data_dayahead'].index.freq is not None)
         self.assertTrue(input_data_dict['df_input_data_dayahead'].isnull().sum().sum()==0)
         self.assertTrue(len(input_data_dict['df_input_data_dayahead'])==10) # The fixed value for prediction_horizon
         # Test passing just load cost and prod price as lists
         action = 'dayahead-optim'
         params = TestCommandLineUtils.get_test_params()
         runtimeparams = {
-            'load_cost_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48],
-            'prod_price_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48]
+            'load_cost_forecast':[i+1 for i in range(48)],
+            'prod_price_forecast':[i+1 for i in range(48)]
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
         input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         self.assertTrue(input_data_dict['fcst'].optim_conf['load_cost_forecast_method']=='list')
@@ -150,16 +150,16 @@
         self.assertIsInstance(opt_res, pd.DataFrame)
         self.assertTrue(opt_res.isnull().sum().sum()==0)
         self.assertTrue(len(opt_res)==len(params['passed_data']['pv_power_forecast']))
         # Test passing just load cost and prod price as lists
         action = 'dayahead-optim'
         params = TestCommandLineUtils.get_test_params()
         runtimeparams = {
-            'load_cost_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48],
-            'prod_price_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48]
+            'load_cost_forecast':[i+1 for i in range(48)],
+            'prod_price_forecast':[i+1 for i in range(48)]
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
         input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         opt_res = dayahead_forecast_optim(input_data_dict, logger, debug=True)
```

### Comparing `emhass-0.8.4/tests/test_forecast.py` & `emhass-0.8.5/tests/test_forecast.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,17 +99,14 @@
         self.assertIsInstance(P_PV_forecast, pd.core.series.Series)
         self.assertIsInstance(P_PV_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(P_PV_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
         self.assertEqual(P_PV_forecast.index.tz, self.fcst.time_zone)
         self.assertEqual(len(self.df_weather_csv), len(P_PV_forecast))
         df_weather_none = self.fcst.get_weather_forecast(method='none')
         self.assertTrue(df_weather_none == None)
-        
-    def test_get_weather_forecast_mlforecaster(self):
-        pass
     
     def test_get_weather_forecast_scrapper_method_mock(self):
         with requests_mock.mock() as m:
             data = bz2.BZ2File(str(pathlib.Path(root+'/data/test_response_scrapper_get_method.pbz2')), "rb")
             data = cPickle.load(data)
             get_url = "https://clearoutside.com/forecast/"+str(round(self.fcst.lat, 2))+"/"+str(round(self.fcst.lon, 2))+"?desktop=true"
             m.get(get_url, content=data)
@@ -151,15 +148,15 @@
             self.assertIsInstance(df_weather_scrap.index, pd.core.indexes.datetimes.DatetimeIndex)
             self.assertIsInstance(df_weather_scrap.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
             self.assertEqual(df_weather_scrap.index.tz, self.fcst.time_zone)
             self.assertTrue(self.fcst.start_forecast < ts for ts in df_weather_scrap.index)
             self.assertEqual(len(df_weather_scrap), 
                             int(self.optim_conf['delta_forecast'].total_seconds()/3600/self.fcst.timeStep))
         
-    def test_get_weather_forecast_solarforecast_method(self):
+    def test_get_weather_forecast_solarforecast_method_mock(self):
         with requests_mock.mock() as m:
             data = bz2.BZ2File(str(pathlib.Path(root+'/data/test_response_solarforecast_get_method.pbz2')), "rb")
             data = cPickle.load(data)
             for i in range(len(self.plant_conf['module_model'])):
                 get_url = "https://api.forecast.solar/estimate/"+str(round(self.fcst.lat, 2))+"/"+str(round(self.fcst.lon, 2))+\
                     "/"+str(self.plant_conf["surface_tilt"][i])+"/"+str(self.plant_conf["surface_azimuth"][i]-180)+\
                     "/"+str(5)
@@ -183,18 +180,18 @@
                 'time_zone': 'Europe/Paris',
                 'lat': 45.83,
                 'lon': 6.86,
                 'alt': 4807.8
             }
             })
         runtimeparams = {
-            'pv_power_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48],
-            'load_power_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48],
-            'load_cost_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48],
-            'prod_price_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48]
+            'pv_power_forecast':[i+1 for i in range(48)],
+            'load_power_forecast':[i+1 for i in range(48)],
+            'load_cost_forecast':[i+1 for i in range(48)],
+            'prod_price_forecast':[i+1 for i in range(48)]
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
         retrieve_hass_conf, optim_conf, plant_conf = get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), 
                                                                     use_secrets=False, params=params_json)
         set_type = "dayahead-optim"
@@ -213,26 +210,25 @@
             rh.get_data(days_list, var_list,
                         minimal_response=False, significant_changes_only=False)
         rh.prepare_data(retrieve_hass_conf['var_load'], load_negative = retrieve_hass_conf['load_negative'],
                         set_zero_min = retrieve_hass_conf['set_zero_min'], 
                         var_replace_zero = retrieve_hass_conf['var_replace_zero'], 
                         var_interp = retrieve_hass_conf['var_interp'])
         df_input_data = rh.df_final.copy()
-        
         fcst = Forecast(retrieve_hass_conf, optim_conf, plant_conf, 
                         params_json, root, logger, get_data_from_file=True)
         df_input_data = copy.deepcopy(df_input_data).iloc[-49:-1]
         P_PV_forecast = fcst.get_weather_forecast(method='list')
         df_input_data.index = P_PV_forecast.index
         df_input_data.index.freq = rh.df_final.index.freq
         self.assertIsInstance(P_PV_forecast, type(pd.DataFrame()))
         self.assertIsInstance(P_PV_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(P_PV_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
-        self.assertEqual(P_PV_forecast.index.tz, self.fcst.time_zone)
-        self.assertTrue(self.fcst.start_forecast < ts for ts in P_PV_forecast.index)
+        self.assertEqual(P_PV_forecast.index.tz, fcst.time_zone)
+        self.assertTrue(fcst.start_forecast < ts for ts in P_PV_forecast.index)
         self.assertTrue(P_PV_forecast.values[0][0] == 1)
         self.assertTrue(P_PV_forecast.values[-1][0] == 48)
         P_load_forecast = fcst.get_load_forecast(method='list')
         self.assertIsInstance(P_load_forecast, pd.core.series.Series)
         self.assertIsInstance(P_load_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(P_load_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
         self.assertEqual(P_load_forecast.index.tz, fcst.time_zone)
@@ -245,14 +241,60 @@
         self.assertTrue(df_input_data['unit_load_cost'].values[0] == 1)
         self.assertTrue(df_input_data['unit_load_cost'].values[-1] == 48)
         df_input_data = fcst.get_prod_price_forecast(df_input_data, method='list')
         self.assertTrue(fcst.var_prod_price in df_input_data.columns)
         self.assertTrue(df_input_data.isnull().sum().sum()==0)
         self.assertTrue(df_input_data['unit_prod_price'].values[0] == 1)
         self.assertTrue(df_input_data['unit_prod_price'].values[-1] == 48)
+        # Test with longer lists
+        with open(root+'/config_emhass.yaml', 'r') as file:
+            params = yaml.load(file, Loader=yaml.FullLoader)
+        params.update({
+            'params_secrets': {
+                'hass_url': 'http://supervisor/core/api',
+                'long_lived_token': '${SUPERVISOR_TOKEN}',
+                'time_zone': 'Europe/Paris',
+                'lat': 45.83,
+                'lon': 6.86,
+                'alt': 4807.8
+            }
+            })
+        runtimeparams = {
+            'pv_power_forecast':[i+1 for i in range(2*48)],
+            'load_power_forecast':[i+1 for i in range(2*48)],
+            'load_cost_forecast':[i+1 for i in range(2*48)],
+            'prod_price_forecast':[i+1 for i in range(2*48)]
+        }
+        runtimeparams_json = json.dumps(runtimeparams)
+        params['passed_data'] = runtimeparams
+        params_json = json.dumps(params)
+        retrieve_hass_conf, optim_conf, plant_conf = get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), 
+                                                                    use_secrets=False, params=params_json)
+        optim_conf['delta_forecast'] = pd.Timedelta(days=2)
+        params, retrieve_hass_conf, optim_conf, plant_conf = treat_runtimeparams(
+            runtimeparams_json, params_json, retrieve_hass_conf, 
+            optim_conf, plant_conf, set_type, logger)
+        fcst = Forecast(retrieve_hass_conf, optim_conf, plant_conf, 
+                        params_json, root, logger, opt_time_delta=48, get_data_from_file=True)
+        P_PV_forecast = fcst.get_weather_forecast(method='list')
+        self.assertIsInstance(P_PV_forecast, type(pd.DataFrame()))
+        self.assertIsInstance(P_PV_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
+        self.assertIsInstance(P_PV_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
+        self.assertEqual(P_PV_forecast.index.tz, fcst.time_zone)
+        self.assertTrue(fcst.start_forecast < ts for ts in P_PV_forecast.index)
+        self.assertTrue(P_PV_forecast.values[0][0] == 1)
+        self.assertTrue(P_PV_forecast.values[-1][0] == 2*48)
+        P_load_forecast = fcst.get_load_forecast(method='list')
+        self.assertIsInstance(P_load_forecast, pd.core.series.Series)
+        self.assertIsInstance(P_load_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
+        self.assertIsInstance(P_load_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
+        self.assertEqual(P_load_forecast.index.tz, fcst.time_zone)
+        self.assertEqual(len(P_PV_forecast), len(P_load_forecast))
+        self.assertTrue(P_load_forecast.values[0] == 1)
+        self.assertTrue(P_load_forecast.values[-1] == 2*48)
         
     def test_get_forecasts_with_lists_special_case(self):
         with open(root+'/config_emhass.yaml', 'r') as file:
             params = yaml.load(file, Loader=yaml.FullLoader)
         params.update({
             'params_secrets': {
                 'hass_url': 'http://supervisor/core/api',
@@ -260,16 +302,16 @@
                 'time_zone': 'Europe/Paris',
                 'lat': 45.83,
                 'lon': 6.86,
                 'alt': 4807.8
             }
             })
         runtimeparams = {
-            'load_cost_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48],
-            'prod_price_forecast':[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48]
+            'load_cost_forecast':[i+1 for i in range(48)],
+            'prod_price_forecast':[i+1 for i in range(48)]
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
         retrieve_hass_conf, optim_conf, plant_conf = get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), 
                                                                     use_secrets=False, params=params_json)
         set_type = "dayahead-optim"
@@ -288,29 +330,28 @@
             rh.get_data(days_list, var_list,
                         minimal_response=False, significant_changes_only=False)
         rh.prepare_data(retrieve_hass_conf['var_load'], load_negative = retrieve_hass_conf['load_negative'],
                         set_zero_min = retrieve_hass_conf['set_zero_min'], 
                         var_replace_zero = retrieve_hass_conf['var_replace_zero'], 
                         var_interp = retrieve_hass_conf['var_interp'])
         df_input_data = rh.df_final.copy()
-        
         fcst = Forecast(retrieve_hass_conf, optim_conf, plant_conf, 
                         params_json, root, logger, get_data_from_file=True)
         df_input_data = copy.deepcopy(df_input_data).iloc[-49:-1]
         P_PV_forecast = fcst.get_weather_forecast()
         df_input_data.index = P_PV_forecast.index
         df_input_data.index.freq = rh.df_final.index.freq
         df_input_data = fcst.get_load_cost_forecast(
-            df_input_data, method=fcst.optim_conf['load_cost_forecast_method'])
+            df_input_data, method='list')
         self.assertTrue(fcst.var_load_cost in df_input_data.columns)
         self.assertTrue(df_input_data.isnull().sum().sum()==0)
         self.assertTrue(df_input_data['unit_load_cost'].values[0] == 1)
         self.assertTrue(df_input_data['unit_load_cost'].values[-1] == 48)
         df_input_data = fcst.get_prod_price_forecast(
-            df_input_data, method=fcst.optim_conf['prod_price_forecast_method'])
+            df_input_data, method='list')
         self.assertTrue(fcst.var_prod_price in df_input_data.columns)
         self.assertTrue(df_input_data.isnull().sum().sum()==0)
         self.assertTrue(df_input_data['unit_prod_price'].values[0] == 1)
         self.assertTrue(df_input_data['unit_prod_price'].values[-1] == 48)
         
     def test_get_power_from_weather(self):
         self.assertIsInstance(self.P_PV_forecast, pd.core.series.Series)
```

### Comparing `emhass-0.8.4/tests/test_machine_learning_forecaster.py` & `emhass-0.8.5/tests/test_machine_learning_forecaster.py`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/tests/test_optimization.py` & `emhass-0.8.5/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/tests/test_retrieve_hass.py` & `emhass-0.8.5/tests/test_retrieve_hass.py`

 * *Files identical despite different names*

### Comparing `emhass-0.8.4/tests/test_utils.py` & `emhass-0.8.5/tests/test_utils.py`

 * *Files identical despite different names*


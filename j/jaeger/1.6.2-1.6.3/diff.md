# Comparing `tmp/jaeger-1.6.2.tar.gz` & `tmp/jaeger-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaeger-1.6.2.tar", max compression
+gzip compressed data, was "jaeger-1.6.3.tar", max compression
```

## Comparing `jaeger-1.6.2.tar` & `jaeger-1.6.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1504 2024-02-27 20:57:51.752602 jaeger-1.6.2/LICENSE.md
--rw-r--r--   0        0        0     2398 2024-02-27 20:57:51.752602 jaeger-1.6.2/README.md
--rw-r--r--   0        0        0     3477 2024-02-27 20:57:51.756602 jaeger-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     1745 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/__init__.py
--rw-r--r--   0        0        0    20331 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/__main__.py
--rw-r--r--   0        0        0       61 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/__init__.py
--rw-r--r--   0        0        0     5033 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/actor.py
--rw-r--r--   0        0        0      816 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/__init__.py
--rw-r--r--   0        0        0     1029 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/alerts.py
--rw-r--r--   0        0        0     1182 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/can.py
--rw-r--r--   0        0        0     3381 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/chiller.py
--rw-r--r--   0        0        0    34526 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/configuration.py
--rw-r--r--   0        0        0      722 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/debug.py
--rw-r--r--   0        0        0     2690 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/disable.py
--rw-r--r--   0        0        0    15031 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/fvc.py
--rw-r--r--   0        0        0    11347 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/home.py
--rw-r--r--   0        0        0     5314 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/ieb.py
--rw-r--r--   0        0        0     1410 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/pollers.py
--rw-r--r--   0        0        0    16070 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/positioner.py
--rw-r--r--   0        0        0     9994 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/power.py
--rw-r--r--   0        0        0      990 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/snapshot.py
--rw-r--r--   0        0        0     1323 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/talk.py
--rw-r--r--   0        0        0     1034 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/testing.py
--rw-r--r--   0        0        0     3579 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/unwind.py
--rw-r--r--   0        0        0      949 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/actor/commands/version.py
--rw-r--r--   0        0        0    14065 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/alerts.py
--rw-r--r--   0        0        0    21709 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/can.py
--rw-r--r--   0        0        0     5257 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/chiller.py
--rw-r--r--   0        0        0     3964 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/commands/__init__.py
--rw-r--r--   0        0        0    22135 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/commands/base.py
--rw-r--r--   0        0        0     9010 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/commands/bootloader.py
--rw-r--r--   0        0        0    12181 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/commands/calibration.py
--rw-r--r--   0        0        0    10788 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/commands/goto.py
--rw-r--r--   0        0        0     6013 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/commands/status.py
--rw-r--r--   0        0        0    26797 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/commands/trajectory.py
--rw-r--r--   0        0        0    10030 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/etc/chiller_APO.yaml
--rw-r--r--   0        0        0     7487 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/etc/chiller_APO_variables.csv
--rw-r--r--   0        0        0     1317 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/etc/fvc.yaml
--rw-r--r--   0        0        0    10541 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/etc/ieb_APO.yaml
--rw-r--r--   0        0        0    10539 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/etc/ieb_LCO.yaml
--rw-r--r--   0        0        0     3329 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/etc/jaeger_APO.yml
--rw-r--r--   0        0        0     3302 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/etc/jaeger_LCO.yml
--rw-r--r--   0        0        0     8711 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/etc/schema.json
--rw-r--r--   0        0        0     1815 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/etc/sextants/epfl.yaml
--rw-r--r--   0        0        0     2367 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/etc/sextants/osu.yaml
--rw-r--r--   0        0        0     1512 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/etc/sextants/schema.json
--rw-r--r--   0        0        0     2364 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/etc/sextants/uw.yaml
--rw-r--r--   0        0        0     3545 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/exceptions.py
--rw-r--r--   0        0        0    52222 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/fps.py
--rw-r--r--   0        0        0    40780 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/fvc.py
--rw-r--r--   0        0        0     4510 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/ieb.py
--rw-r--r--   0        0        0      162 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/interfaces/__init__.py
--rw-r--r--   0        0        0     1142 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/interfaces/bus.py
--rw-r--r--   0        0        0     6759 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/interfaces/cannet.py
--rw-r--r--   0        0        0    12892 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/interfaces/message.py
--rw-r--r--   0        0        0     1874 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/interfaces/notifier.py
--rw-r--r--   0        0        0     1199 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/interfaces/virtual.py
--rw-r--r--   0        0        0    19803 2024-02-27 20:57:51.756602 jaeger-1.6.2/python/jaeger/kaiju.py
--rw-r--r--   0        0        0     8034 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/maskbits.py
--rw-r--r--   0        0        0     7296 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/plotting.py
--rw-r--r--   0        0        0    18121 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/positioner.py
--rw-r--r--   0        0        0        0 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/scripts/__init__.py
--rw-r--r--   0        0        0     1825 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/scripts/generate_chiller_yaml.py
--rwxr-xr-x   0        0        0    19975 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/scripts/robotcalib.py
--rw-r--r--   0        0        0      293 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/target/__init__.py
--rw-r--r--   0        0        0    65093 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/target/configuration.py
--rw-r--r--   0        0        0     9413 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/target/design.py
--rw-r--r--   0        0        0    11797 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/target/tools.py
--rw-r--r--   0        0        0    12403 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/testing.py
--rw-r--r--   0        0        0       60 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/utils/__init__.py
--rw-r--r--   0        0        0     9562 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/utils/database.py
--rw-r--r--   0        0        0    14766 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/utils/helpers.py
--rw-r--r--   0        0        0     9549 2024-02-27 20:57:51.760602 jaeger-1.6.2/python/jaeger/utils/utils.py
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 jaeger-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-04-01 21:45:34.112062 jaeger-1.6.3/LICENSE.md
+-rw-r--r--   0        0        0     2398 2024-04-01 21:45:34.112062 jaeger-1.6.3/README.md
+-rw-r--r--   0        0        0     3477 2024-04-01 21:45:34.116062 jaeger-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0     1745 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/__init__.py
+-rw-r--r--   0        0        0    20331 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/__main__.py
+-rw-r--r--   0        0        0       61 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/__init__.py
+-rw-r--r--   0        0        0     5033 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/actor.py
+-rw-r--r--   0        0        0      816 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1029 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/alerts.py
+-rw-r--r--   0        0        0     1182 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/can.py
+-rw-r--r--   0        0        0     3381 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/chiller.py
+-rw-r--r--   0        0        0    35257 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/configuration.py
+-rw-r--r--   0        0        0      722 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/debug.py
+-rw-r--r--   0        0        0     2690 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/disable.py
+-rw-r--r--   0        0        0    15031 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/fvc.py
+-rw-r--r--   0        0        0    11347 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/home.py
+-rw-r--r--   0        0        0     5314 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/ieb.py
+-rw-r--r--   0        0        0     1410 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/pollers.py
+-rw-r--r--   0        0        0    16070 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/positioner.py
+-rw-r--r--   0        0        0     9994 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/power.py
+-rw-r--r--   0        0        0      990 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/snapshot.py
+-rw-r--r--   0        0        0     1323 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/talk.py
+-rw-r--r--   0        0        0     1034 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/testing.py
+-rw-r--r--   0        0        0     3579 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/unwind.py
+-rw-r--r--   0        0        0      949 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/version.py
+-rw-r--r--   0        0        0    14065 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/alerts.py
+-rw-r--r--   0        0        0    21709 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/can.py
+-rw-r--r--   0        0        0     5257 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/chiller.py
+-rw-r--r--   0        0        0     3964 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/__init__.py
+-rw-r--r--   0        0        0    22135 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/base.py
+-rw-r--r--   0        0        0     9010 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/bootloader.py
+-rw-r--r--   0        0        0    12181 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/calibration.py
+-rw-r--r--   0        0        0    10788 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/goto.py
+-rw-r--r--   0        0        0     6013 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/status.py
+-rw-r--r--   0        0        0    26797 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/trajectory.py
+-rw-r--r--   0        0        0    10030 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/chiller_APO.yaml
+-rw-r--r--   0        0        0     7487 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/chiller_APO_variables.csv
+-rw-r--r--   0        0        0     1317 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/fvc.yaml
+-rw-r--r--   0        0        0    10541 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/ieb_APO.yaml
+-rw-r--r--   0        0        0    10539 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/ieb_LCO.yaml
+-rw-r--r--   0        0        0     3329 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/jaeger_APO.yml
+-rw-r--r--   0        0        0     3302 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/jaeger_LCO.yml
+-rw-r--r--   0        0        0     8711 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/etc/schema.json
+-rw-r--r--   0        0        0     1815 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/etc/sextants/epfl.yaml
+-rw-r--r--   0        0        0     2367 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/etc/sextants/osu.yaml
+-rw-r--r--   0        0        0     1512 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/etc/sextants/schema.json
+-rw-r--r--   0        0        0     2364 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/etc/sextants/uw.yaml
+-rw-r--r--   0        0        0     3545 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/exceptions.py
+-rw-r--r--   0        0        0    52222 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/fps.py
+-rw-r--r--   0        0        0    40780 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/fvc.py
+-rw-r--r--   0        0        0     4510 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/ieb.py
+-rw-r--r--   0        0        0      162 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/interfaces/__init__.py
+-rw-r--r--   0        0        0     1142 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/interfaces/bus.py
+-rw-r--r--   0        0        0     6759 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/interfaces/cannet.py
+-rw-r--r--   0        0        0    12892 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/interfaces/message.py
+-rw-r--r--   0        0        0     1874 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/interfaces/notifier.py
+-rw-r--r--   0        0        0     1199 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/interfaces/virtual.py
+-rw-r--r--   0        0        0    19803 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/kaiju.py
+-rw-r--r--   0        0        0     8034 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/maskbits.py
+-rw-r--r--   0        0        0     7296 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/plotting.py
+-rw-r--r--   0        0        0    18121 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/positioner.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/scripts/__init__.py
+-rw-r--r--   0        0        0     1825 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/scripts/generate_chiller_yaml.py
+-rwxr-xr-x   0        0        0    19975 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/scripts/robotcalib.py
+-rw-r--r--   0        0        0      293 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/target/__init__.py
+-rw-r--r--   0        0        0    65093 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/target/configuration.py
+-rw-r--r--   0        0        0     9413 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/target/design.py
+-rw-r--r--   0        0        0    11797 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/target/tools.py
+-rw-r--r--   0        0        0    12403 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/testing.py
+-rw-r--r--   0        0        0       60 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/utils/__init__.py
+-rw-r--r--   0        0        0     9562 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/utils/database.py
+-rw-r--r--   0        0        0    14766 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/utils/helpers.py
+-rw-r--r--   0        0        0     9549 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/utils/utils.py
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 jaeger-1.6.3/PKG-INFO
```

### Comparing `jaeger-1.6.2/LICENSE.md` & `jaeger-1.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/README.md` & `jaeger-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/pyproject.toml` & `jaeger-1.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaeger"
-version = "1.6.2"
+version = "1.6.3"
 description = "Controllers for the SDSS-V FPS"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/jaeger"
 repository = "https://github.com/sdss/jaeger"
 documentation = "https://sdss-jaeger.readthedocs.io/en/latest/"
```

### Comparing `jaeger-1.6.2/python/jaeger/__init__.py` & `jaeger-1.6.3/python/jaeger/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/__main__.py` & `jaeger-1.6.3/python/jaeger/__main__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/actor.py` & `jaeger-1.6.3/python/jaeger/actor/actor.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/__init__.py` & `jaeger-1.6.3/python/jaeger/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/alerts.py` & `jaeger-1.6.3/python/jaeger/actor/commands/alerts.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/can.py` & `jaeger-1.6.3/python/jaeger/actor/commands/can.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/chiller.py` & `jaeger-1.6.3/python/jaeger/actor/commands/chiller.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/configuration.py` & `jaeger-1.6.3/python/jaeger/actor/commands/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     design_id: int | None = None,
     preload: bool = False,
     no_clone: bool = False,
     scale: float | None = None,
     fudge_factor: float | None = None,
     epoch: float | None = None,
     epoch_delay: float = 0.0,
+    extra_epoch_delay: float = 0.0,
     boss_wavelength: float | None = None,
     apogee_wavelength: float | None = None,
     get_paths: bool = True,
     path_generation_mode: str | None = None,
     safety_factor: float = 1,
     offset_min_skybrightness: float = 0.5,
 ):
@@ -68,15 +69,17 @@
 
     if design_id is None:
         design_id, _epoch_delay = get_designid_from_queue(
             pop=not preload,
             epoch_delay=True,
         )
         if epoch_delay == 0.0 and _epoch_delay is not None:
-            epoch_delay = _epoch_delay
+            epoch_delay = _epoch_delay + extra_epoch_delay
+        else:
+            epoch_delay += extra_epoch_delay
 
     if design_id is None:
         command.error("Failed getting a new design from the queue.")
         return False
 
     if preload:
         command.info(f"Preloading design {design_id}.")
@@ -259,14 +262,21 @@
 @click.option(
     "--epoch-delay",
     type=float,
     default=0.0,
     help="A delay in seconds for the epoch for which the configuration is calculated.",
 )
 @click.option(
+    "--extra-epoch-delay",
+    type=float,
+    default=0.0,
+    help="A delay in seconds to be added on top of the --epoch-delay. This is "
+    "mainly used by HAL when it preloads a design ahead of time..",
+)
+@click.option(
     "--boss-wavelength",
     type=click.FloatRange(3000, 10000),
     help="Optimise positioning of BOSS fibres to this wavelength.",
 )
 @click.option(
     "--apogee-wavelength",
     type=click.FloatRange(16000, 17000),
@@ -345,14 +355,15 @@
     reload: bool = False,
     replace: bool = False,
     from_positions: bool = False,
     from_preloaded: bool = False,
     generate_paths: bool = False,
     epoch: float | None = None,
     epoch_delay: float = 0.0,
+    extra_epoch_delay: float = 0.0,
     apogee_wavelength: float | None = None,
     boss_wavelength: float | None = None,
     ingest: bool = False,
     write_summary: bool = False,
     execute: bool = False,
     reissue: bool = False,
     scale: float | None = None,
@@ -398,14 +409,15 @@
             design_id=designid,
             fudge_factor=fudge_factor,
             preload=False,
             no_clone=no_clone,
             scale=scale,
             epoch=epoch,
             epoch_delay=epoch_delay,
+            extra_epoch_delay=extra_epoch_delay,
             boss_wavelength=boss_wavelength,
             apogee_wavelength=apogee_wavelength,
             get_paths=False,
             path_generation_mode=path_generation_mode,
             safety_factor=safety_factor,
             offset_min_skybrightness=offset_min_skybrightness,
         )
@@ -576,14 +588,21 @@
 @click.option(
     "--epoch-delay",
     type=float,
     default=0.0,
     help="A delay in seconds for the epoch for which the configuration is calculated.",
 )
 @click.option(
+    "--extra-epoch-delay",
+    type=float,
+    default=0.0,
+    help="A delay in seconds to be added on top of the --epoch-delay. This is "
+    "mainly used by HAL when it preloads a design ahead of time..",
+)
+@click.option(
     "--boss-wavelength",
     type=click.FloatRange(3000, 10000),
     help="Optimise positioning of BOSS fibres to this wavelength.",
 )
 @click.option(
     "--apogee-wavelength",
     type=click.FloatRange(16000, 17000),
@@ -632,14 +651,15 @@
 @timeout(300)
 async def preload(
     command: JaegerCommandType,
     fps: FPS,
     designid: int | None = None,
     epoch: float | None = None,
     epoch_delay: float = 0.0,
+    extra_epoch_delay: float = 0.0,
     apogee_wavelength: float | None = None,
     boss_wavelength: float | None = None,
     scale: float | None = None,
     fudge_factor: float | None = None,
     no_clone: bool = False,
     make_active: bool = True,
     clear: bool = False,
@@ -666,14 +686,15 @@
         design_id=designid,
         preload=True,
         no_clone=no_clone,
         scale=scale,
         fudge_factor=fudge_factor,
         epoch=epoch,
         epoch_delay=epoch_delay,
+        extra_epoch_delay=extra_epoch_delay,
         boss_wavelength=boss_wavelength,
         apogee_wavelength=apogee_wavelength,
         safety_factor=safety_factor,
         offset_min_skybrightness=offset_min_skybrightness,
     )
 
     if configuration is False:
```

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/debug.py` & `jaeger-1.6.3/python/jaeger/actor/commands/debug.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/disable.py` & `jaeger-1.6.3/python/jaeger/actor/commands/disable.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/fvc.py` & `jaeger-1.6.3/python/jaeger/actor/commands/fvc.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/home.py` & `jaeger-1.6.3/python/jaeger/actor/commands/home.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/ieb.py` & `jaeger-1.6.3/python/jaeger/actor/commands/ieb.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/pollers.py` & `jaeger-1.6.3/python/jaeger/actor/commands/pollers.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/positioner.py` & `jaeger-1.6.3/python/jaeger/actor/commands/positioner.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/power.py` & `jaeger-1.6.3/python/jaeger/actor/commands/power.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/snapshot.py` & `jaeger-1.6.3/python/jaeger/actor/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/talk.py` & `jaeger-1.6.3/python/jaeger/actor/commands/talk.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/testing.py` & `jaeger-1.6.3/python/jaeger/actor/commands/testing.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/unwind.py` & `jaeger-1.6.3/python/jaeger/actor/commands/unwind.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/actor/commands/version.py` & `jaeger-1.6.3/python/jaeger/actor/commands/version.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/alerts.py` & `jaeger-1.6.3/python/jaeger/alerts.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/can.py` & `jaeger-1.6.3/python/jaeger/can.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/chiller.py` & `jaeger-1.6.3/python/jaeger/chiller.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/commands/__init__.py` & `jaeger-1.6.3/python/jaeger/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/commands/base.py` & `jaeger-1.6.3/python/jaeger/commands/base.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/commands/bootloader.py` & `jaeger-1.6.3/python/jaeger/commands/bootloader.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/commands/calibration.py` & `jaeger-1.6.3/python/jaeger/commands/calibration.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/commands/goto.py` & `jaeger-1.6.3/python/jaeger/commands/goto.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/commands/status.py` & `jaeger-1.6.3/python/jaeger/commands/status.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/commands/trajectory.py` & `jaeger-1.6.3/python/jaeger/commands/trajectory.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/etc/chiller_APO.yaml` & `jaeger-1.6.3/python/jaeger/etc/chiller_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/etc/chiller_APO_variables.csv` & `jaeger-1.6.3/python/jaeger/etc/chiller_APO_variables.csv`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/etc/fvc.yaml` & `jaeger-1.6.3/python/jaeger/etc/fvc.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/etc/ieb_APO.yaml` & `jaeger-1.6.3/python/jaeger/etc/ieb_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/etc/ieb_LCO.yaml` & `jaeger-1.6.3/python/jaeger/etc/ieb_LCO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/etc/jaeger_APO.yml` & `jaeger-1.6.3/python/jaeger/etc/jaeger_APO.yml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/etc/jaeger_LCO.yml` & `jaeger-1.6.3/python/jaeger/etc/jaeger_LCO.yml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/etc/schema.json` & `jaeger-1.6.3/python/jaeger/etc/schema.json`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/etc/sextants/epfl.yaml` & `jaeger-1.6.3/python/jaeger/etc/sextants/epfl.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/etc/sextants/osu.yaml` & `jaeger-1.6.3/python/jaeger/etc/sextants/osu.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/etc/sextants/schema.json` & `jaeger-1.6.3/python/jaeger/etc/sextants/schema.json`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/etc/sextants/uw.yaml` & `jaeger-1.6.3/python/jaeger/etc/sextants/uw.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/exceptions.py` & `jaeger-1.6.3/python/jaeger/exceptions.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/fps.py` & `jaeger-1.6.3/python/jaeger/fps.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/fvc.py` & `jaeger-1.6.3/python/jaeger/fvc.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/ieb.py` & `jaeger-1.6.3/python/jaeger/ieb.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/interfaces/bus.py` & `jaeger-1.6.3/python/jaeger/interfaces/bus.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/interfaces/cannet.py` & `jaeger-1.6.3/python/jaeger/interfaces/cannet.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/interfaces/message.py` & `jaeger-1.6.3/python/jaeger/interfaces/message.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/interfaces/notifier.py` & `jaeger-1.6.3/python/jaeger/interfaces/notifier.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/interfaces/virtual.py` & `jaeger-1.6.3/python/jaeger/interfaces/virtual.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/kaiju.py` & `jaeger-1.6.3/python/jaeger/kaiju.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/maskbits.py` & `jaeger-1.6.3/python/jaeger/maskbits.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/plotting.py` & `jaeger-1.6.3/python/jaeger/plotting.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/positioner.py` & `jaeger-1.6.3/python/jaeger/positioner.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/scripts/generate_chiller_yaml.py` & `jaeger-1.6.3/python/jaeger/scripts/generate_chiller_yaml.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/scripts/robotcalib.py` & `jaeger-1.6.3/python/jaeger/scripts/robotcalib.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/target/configuration.py` & `jaeger-1.6.3/python/jaeger/target/configuration.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/target/design.py` & `jaeger-1.6.3/python/jaeger/target/design.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/target/tools.py` & `jaeger-1.6.3/python/jaeger/target/tools.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/testing.py` & `jaeger-1.6.3/python/jaeger/testing.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/utils/database.py` & `jaeger-1.6.3/python/jaeger/utils/database.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/utils/helpers.py` & `jaeger-1.6.3/python/jaeger/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/python/jaeger/utils/utils.py` & `jaeger-1.6.3/python/jaeger/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.2/PKG-INFO` & `jaeger-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaeger
-Version: 1.6.2
+Version: 1.6.3
 Summary: Controllers for the SDSS-V FPS
 Home-page: https://github.com/sdss/jaeger
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.9,<3.11
```


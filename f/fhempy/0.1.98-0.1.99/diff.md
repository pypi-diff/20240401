# Comparing `tmp/fhempy-0.1.98.tar.gz` & `tmp/fhempy-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fhempy-0.1.98.tar", last modified: Fri Aug 27 12:03:29 2021, max compression
+gzip compressed data, was "dist/fhempy-0.1.99.tar", last modified: Fri Aug 27 17:39:23 2021, max compression
```

## Comparing `fhempy-0.1.98.tar` & `fhempy-0.1.99.tar`

### file list

```diff
@@ -1,284 +1,284 @@
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/.github/
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/.github/workflows/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1862 2021-01-27 22:27:34.000000 fhempy-0.1.98/.github/workflows/release.yml
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      345 2021-01-27 22:27:34.000000 fhempy-0.1.98/.github/workflows/stale.yml
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1163 2021-08-27 12:03:18.000000 fhempy-0.1.98/.github/workflows/tests.yml
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1805 2021-01-10 19:35:29.000000 fhempy-0.1.98/.gitignore
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      628 2021-01-05 09:10:54.000000 fhempy-0.1.98/CHANGED
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    16020 2021-08-27 12:03:20.000000 fhempy-0.1.98/CHANGELOG.md
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    14335 2021-07-30 18:50:12.000000 fhempy-0.1.98/FHEM/10_BindingsIo.pm
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4583 2021-08-25 20:02:45.000000 fhempy-0.1.98/FHEM/10_PythonBinding.pm
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3170 2021-08-27 12:03:19.000000 fhempy-0.1.98/FHEM/10_PythonModule.pm
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/bin/
--rwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)     3668 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/bin/fhempy
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       14 2020-12-30 15:56:20.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/__init__.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/__init__.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_presence/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1208 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_presence/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       23 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_presence/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    11491 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_presence/ble_presence.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       33 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_presence/manifest.json
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_reset/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      632 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_reset/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       33 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_reset/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     5039 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_reset/ble_reset.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       38 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_reset/manifest.json
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/bt_presence/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      312 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/bt_presence/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       29 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/bt_presence/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3564 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/bt_presence/bt_presence.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       61 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/bt_presence/manifest.json
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       16 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     8190 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/ble.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      108 2021-06-23 18:33:05.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/clientsession.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/discover_fhempy/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/discover_fhempy/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2981 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/discover_fhempy/discover_fhempy.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       50 2021-08-06 20:23:55.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/discover_fhempy/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       50 2021-08-06 20:23:55.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     6719 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/ssdp.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1137 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/zeroconf.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_ble/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_ble/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     5656 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_ble/discover_ble.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       39 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_ble/manifest.json
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_mdns/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_mdns/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     5592 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_mdns/discover_mdns.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       35 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_mdns/manifest.json
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_upnp/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       24 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_upnp/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3131 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_upnp/discover_upnp.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       83 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_upnp/manifest.json
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/dlna_dmr/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       25 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/dlna_dmr/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    13582 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/dlna_dmr/dlna_dmr.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       83 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/dlna_dmr/manifest.json
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1516 2020-12-22 22:51:37.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       22 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     7644 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/connection.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    20086 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/eq3bt.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    15702 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/eq3btsmart.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       76 2021-01-05 09:10:54.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)   688467 2020-12-22 22:51:37.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/screenshot.png
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4585 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/structures.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/erelax_vaillant/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      204 2021-07-27 20:16:57.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/erelax_vaillant/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-07-27 20:16:57.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/erelax_vaillant/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    15639 2021-07-30 18:50:12.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/erelax_vaillant/erelax_vaillant.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      104 2021-07-27 20:16:57.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/erelax_vaillant/manifest.json
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/esphome/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      174 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/esphome/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       11 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/esphome/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2859 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/esphome/esphome.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       42 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/esphome/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     8753 2021-07-30 18:50:12.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/fhem.py
--rwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)    20175 2021-08-02 20:17:48.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/fhem_pythonbinding.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/fusionsolar/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-08-01 15:40:09.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/fusionsolar/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1023 2021-08-01 18:19:22.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/fusionsolar/const.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1433 2021-08-01 16:54:51.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/fusionsolar/fusionsolar_api.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1149 2021-08-01 18:23:24.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/fusionsolar/fusiosolar.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       25 2021-08-01 15:40:10.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/fusionsolar/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3608 2021-01-03 20:14:20.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/generic.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/gfprobt/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/gfprobt/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     6661 2021-03-08 14:37:32.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/gfprobt/gfprobt.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       48 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/gfprobt/manifest.json
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/googlecast/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1598 2021-08-26 21:58:20.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/googlecast/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/googlecast/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    29993 2021-05-04 17:54:36.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/googlecast/googlecast.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      166 2021-05-04 17:54:36.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/googlecast/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)   333998 2020-12-22 22:51:37.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/googlecast/screenshot.png
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/helloworld/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/helloworld/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3850 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/helloworld/helloworld.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       25 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/helloworld/manifest.json
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miflora/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      751 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miflora/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       32 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miflora/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       44 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miflora/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4373 2021-08-25 20:02:45.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miflora/miflora.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miio/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1666 2020-12-22 22:51:37.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miio/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       25 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miio/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       54 2021-04-18 18:06:49.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miio/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     7377 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miio/miio.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      815 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       37 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       64 2021-08-25 20:26:45.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3732 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp/mitemp.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp2/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      829 2021-05-04 17:54:36.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp2/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       37 2021-05-04 17:54:36.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp2/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       40 2021-05-04 17:54:36.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp2/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1975 2021-05-04 17:54:36.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp2/mitemp2.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/nespresso_ble/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1156 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/nespresso_ble/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       37 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/nespresso_ble/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       55 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/nespresso_ble/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    13430 2021-01-30 08:34:18.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/nespresso_ble/nespresso.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     5767 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/nespresso_ble/nespresso_ble.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/object_detection/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      948 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/object_detection/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       26 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/object_detection/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)  4183312 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/object_detection/detect.tflite
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      665 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/object_detection/labelmap.txt
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       69 2021-01-05 09:10:54.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/object_detection/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    17932 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/object_detection/object_detection.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     6208 2021-08-25 20:22:56.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/pkg_installer.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ring/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      499 2021-07-13 19:05:16.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ring/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       23 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ring/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       54 2021-03-08 19:10:56.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ring/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    14877 2021-07-13 19:05:16.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ring/ring.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/skodaconnect/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      411 2021-06-23 14:14:13.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/skodaconnect/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-06-23 14:14:13.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/skodaconnect/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       54 2021-08-23 22:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/skodaconnect/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    10329 2021-08-23 16:37:52.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/skodaconnect/skodaconnect.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/spotify/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      704 2020-12-29 20:40:38.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/spotify/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-29 20:40:38.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/spotify/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       49 2021-05-04 17:54:36.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/spotify/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    14603 2021-05-04 17:54:36.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/spotify/spotify.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/spotify_connect_player/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      164 2021-01-05 09:10:54.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/spotify_connect_player/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-01-05 09:10:54.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/spotify_connect_player/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       88 2021-01-05 09:10:54.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/spotify_connect_player/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     7093 2021-05-04 17:54:36.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/spotify_connect_player/spotify_connect_player.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2454 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-01-08 21:51:39.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2972 2021-01-08 21:51:39.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya/const.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       49 2021-03-01 19:58:59.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)  3022362 2021-01-29 20:18:28.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya/mappings.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    21035 2021-07-30 18:50:12.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya/tuya.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya_cloud/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1333 2021-08-23 16:54:59.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya_cloud/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       11 2021-07-30 18:50:12.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya_cloud/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      374 2021-07-30 18:50:12.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya_cloud/const.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       56 2021-08-08 16:09:35.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya_cloud/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1910 2021-08-26 16:11:06.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya_cloud/tuya_cloud.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    11921 2021-08-27 12:03:19.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya_cloud/tuya_cloud_device.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     7497 2021-08-26 21:58:20.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya_cloud/tuya_cloud_setup.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     8632 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/utils.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       23 2021-08-27 12:03:20.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/version.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/volvooncall/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-08-07 19:48:15.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/volvooncall/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       53 2021-08-07 19:49:24.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/volvooncall/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    10200 2021-08-07 19:52:36.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/volvooncall/volvooncall.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/warema/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-08-27 12:03:18.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/warema/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       56 2021-08-27 12:03:18.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/warema/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     6362 2021-08-27 12:03:18.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/warema/warema.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/wienerlinien/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      266 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/wienerlinien/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       32 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/wienerlinien/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       34 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/wienerlinien/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4266 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/wienerlinien/wienerlinien.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      604 2020-12-22 22:51:37.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/__init__.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       14 2020-12-23 07:30:08.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    11967 2021-02-14 19:56:31.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/bluetooth.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    38790 2021-02-14 19:56:31.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/gateway3.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     7962 2021-02-14 19:56:31.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/mini_miio.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     5703 2021-02-14 19:56:31.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/shell.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     6239 2021-02-02 20:34:04.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/unqlite.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    20234 2021-02-14 19:56:31.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/utils.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     8064 2021-02-14 19:56:31.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/xiaomi_cloud.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       91 2020-12-22 22:51:37.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1855 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/miio_fix.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4848 2021-02-14 19:56:31.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/xiaomi_gateway3.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/__init__.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-26 20:05:39.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3513 2021-07-31 06:55:31.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/base.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2160 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/gateway.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1800 2021-02-10 20:33:08.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/sensor.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       61 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4080 2021-08-17 21:02:28.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/xiaomi_gateway3_device.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      805 2020-12-22 22:56:16.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       25 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       34 2020-12-09 20:57:30.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/manifest.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     6972 2021-02-14 19:56:31.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/xiaomi_tokens.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy.egg-info/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     9285 2021-08-27 12:03:24.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy.egg-info/PKG-INFO
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    11915 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy.egg-info/SOURCES.txt
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        1 2021-08-27 12:03:24.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy.egg-info/dependency_links.txt
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       79 2021-08-27 12:03:24.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy.egg-info/requires.txt
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       13 2021-08-27 12:03:24.000000 fhempy-0.1.98/FHEM/bindings/python/fhempy.egg-info/top_level.txt
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/tests/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-05 09:10:54.000000 fhempy-0.1.98/FHEM/bindings/python/tests/__init__.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/__init__.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/__init__.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/__init__.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      566 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_chime_health_attrs.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    10303 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_devices.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      882 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_ding_active.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      566 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_doorboot_health_attrs.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      566 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_doorboot_health_attrs_id987653.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      220 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_doorbots.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      214 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_oauth.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1248 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_session.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     5572 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/test_basics.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/__init__.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1095 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/device.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3518 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/devices.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1208 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/local_devices.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      234 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/token.json
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3900 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/test_device_ctrl.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2356 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/test_setup.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2246 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/test_modules_basic.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1049 2021-08-02 20:47:28.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/test_update.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     8731 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/tests/mocked/test_utils.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/tests/reallife/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/reallife/__init__.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/tests/reallife/modules/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/reallife/modules/__init__.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/tests/reallife/modules/googlecast/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/reallife/modules/googlecast/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4598 2021-02-01 17:04:33.000000 fhempy-0.1.98/FHEM/bindings/python/tests/reallife/modules/googlecast/test_reallife_basics.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/tests/reallife/modules/xiaomi_gateway3/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-02-14 19:56:31.000000 fhempy-0.1.98/FHEM/bindings/python/tests/reallife/modules/xiaomi_gateway3/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4547 2021-02-14 19:56:31.000000 fhempy-0.1.98/FHEM/bindings/python/tests/reallife/modules/xiaomi_gateway3/test_general.py
-drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 12:03:29.000000 fhempy-0.1.98/FHEM/bindings/python/tests/utils/
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.98/FHEM/bindings/python/tests/utils/__init__.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4224 2021-02-14 19:56:31.000000 fhempy-0.1.98/FHEM/bindings/python/tests/utils/mock_fhem.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1070 2020-12-04 22:15:54.000000 fhempy-0.1.98/LICENSE
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       94 2021-01-27 22:27:34.000000 fhempy-0.1.98/MANIFEST.in
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     9285 2021-08-27 12:03:29.000000 fhempy-0.1.98/PKG-INFO
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     7763 2021-08-25 20:02:45.000000 fhempy-0.1.98/README.md
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      359 2021-08-27 12:03:19.000000 fhempy-0.1.98/controls_pythonbinding.txt
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      463 2020-12-07 19:21:53.000000 fhempy-0.1.98/fhempy.service
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    32747 2020-09-19 15:52:13.000000 fhempy-0.1.98/flowchart.png
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      536 2021-01-20 20:58:13.000000 fhempy-0.1.98/install_python.sh
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      234 2020-12-05 19:16:34.000000 fhempy-0.1.98/install_systemd_fhempy.sh
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      916 2021-01-05 09:11:25.000000 fhempy-0.1.98/prepare_update.pl
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      670 2021-01-30 19:42:20.000000 fhempy-0.1.98/release.sh
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       78 2021-02-17 20:10:58.000000 fhempy-0.1.98/requirements.txt
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      188 2021-03-01 21:14:39.000000 fhempy-0.1.98/requirements_dev.txt
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      164 2021-02-17 20:10:58.000000 fhempy-0.1.98/requirements_tests.txt
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       38 2021-08-27 12:03:29.000000 fhempy-0.1.98/setup.cfg
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1161 2021-01-27 22:09:58.000000 fhempy-0.1.98/setup.py
--rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      259 2021-01-29 20:43:25.000000 fhempy-0.1.98/tox.ini
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:23.000000 fhempy-0.1.99/
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/.github/
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/.github/workflows/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1862 2021-01-27 22:27:34.000000 fhempy-0.1.99/.github/workflows/release.yml
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      345 2021-01-27 22:27:34.000000 fhempy-0.1.99/.github/workflows/stale.yml
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1163 2021-08-27 17:39:11.000000 fhempy-0.1.99/.github/workflows/tests.yml
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1805 2021-01-10 19:35:29.000000 fhempy-0.1.99/.gitignore
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      628 2021-01-05 09:10:54.000000 fhempy-0.1.99/CHANGED
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    16196 2021-08-27 17:39:13.000000 fhempy-0.1.99/CHANGELOG.md
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    14335 2021-07-30 18:50:12.000000 fhempy-0.1.99/FHEM/10_BindingsIo.pm
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4583 2021-08-25 20:02:45.000000 fhempy-0.1.99/FHEM/10_PythonBinding.pm
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3170 2021-08-27 17:39:12.000000 fhempy-0.1.99/FHEM/10_PythonModule.pm
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/bin/
+-rwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)     3668 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/bin/fhempy
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       14 2020-12-30 15:56:20.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/__init__.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/__init__.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_presence/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1208 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_presence/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       23 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_presence/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    11491 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_presence/ble_presence.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       33 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_presence/manifest.json
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_reset/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      632 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_reset/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       33 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_reset/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     5039 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_reset/ble_reset.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       38 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_reset/manifest.json
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/bt_presence/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      312 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/bt_presence/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       29 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/bt_presence/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3564 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/bt_presence/bt_presence.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       61 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/bt_presence/manifest.json
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       16 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     8190 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/ble.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      108 2021-06-23 18:33:05.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/clientsession.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/discover_fhempy/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/discover_fhempy/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2981 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/discover_fhempy/discover_fhempy.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       50 2021-08-06 20:23:55.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/discover_fhempy/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       50 2021-08-06 20:23:55.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     6719 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/ssdp.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1137 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/zeroconf.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_ble/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_ble/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     5656 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_ble/discover_ble.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       39 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_ble/manifest.json
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_mdns/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_mdns/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     5592 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_mdns/discover_mdns.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       35 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_mdns/manifest.json
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_upnp/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       24 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_upnp/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3131 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_upnp/discover_upnp.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       83 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_upnp/manifest.json
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/dlna_dmr/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       25 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/dlna_dmr/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    13582 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/dlna_dmr/dlna_dmr.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       83 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/dlna_dmr/manifest.json
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1516 2020-12-22 22:51:37.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       22 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     7644 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/connection.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    20086 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/eq3bt.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    15702 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/eq3btsmart.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       76 2021-01-05 09:10:54.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)   688467 2020-12-22 22:51:37.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/screenshot.png
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4585 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/structures.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/erelax_vaillant/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      204 2021-07-27 20:16:57.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/erelax_vaillant/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-07-27 20:16:57.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/erelax_vaillant/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    15639 2021-07-30 18:50:12.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/erelax_vaillant/erelax_vaillant.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      104 2021-07-27 20:16:57.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/erelax_vaillant/manifest.json
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/esphome/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      174 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/esphome/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       11 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/esphome/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2859 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/esphome/esphome.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       42 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/esphome/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     8753 2021-07-30 18:50:12.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/fhem.py
+-rwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)    20175 2021-08-02 20:17:48.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/fhem_pythonbinding.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/fusionsolar/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-08-01 15:40:09.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/fusionsolar/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1023 2021-08-01 18:19:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/fusionsolar/const.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1433 2021-08-01 16:54:51.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/fusionsolar/fusionsolar_api.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1149 2021-08-01 18:23:24.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/fusionsolar/fusiosolar.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       25 2021-08-01 15:40:10.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/fusionsolar/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3608 2021-01-03 20:14:20.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/generic.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/gfprobt/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/gfprobt/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     6661 2021-03-08 14:37:32.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/gfprobt/gfprobt.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       48 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/gfprobt/manifest.json
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/googlecast/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1598 2021-08-26 21:58:20.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/googlecast/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/googlecast/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    29993 2021-05-04 17:54:36.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/googlecast/googlecast.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      166 2021-05-04 17:54:36.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/googlecast/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)   333998 2020-12-22 22:51:37.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/googlecast/screenshot.png
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/helloworld/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/helloworld/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3850 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/helloworld/helloworld.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       25 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/helloworld/manifest.json
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miflora/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      751 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miflora/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       32 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miflora/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       44 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miflora/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4373 2021-08-25 20:02:45.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miflora/miflora.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miio/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1666 2020-12-22 22:51:37.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miio/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       25 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miio/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       54 2021-04-18 18:06:49.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miio/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     7377 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miio/miio.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      815 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       37 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       64 2021-08-25 20:26:45.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3732 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp/mitemp.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp2/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      829 2021-05-04 17:54:36.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp2/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       37 2021-05-04 17:54:36.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp2/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       40 2021-05-04 17:54:36.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp2/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1975 2021-05-04 17:54:36.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp2/mitemp2.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/nespresso_ble/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1156 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/nespresso_ble/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       37 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/nespresso_ble/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       55 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/nespresso_ble/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    13430 2021-01-30 08:34:18.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/nespresso_ble/nespresso.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     5767 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/nespresso_ble/nespresso_ble.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/object_detection/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      948 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/object_detection/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       26 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/object_detection/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)  4183312 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/object_detection/detect.tflite
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      665 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/object_detection/labelmap.txt
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       69 2021-01-05 09:10:54.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/object_detection/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    17932 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/object_detection/object_detection.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     6208 2021-08-25 20:22:56.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/pkg_installer.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ring/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      499 2021-07-13 19:05:16.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ring/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       23 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ring/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       54 2021-03-08 19:10:56.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ring/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    14877 2021-07-13 19:05:16.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ring/ring.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/skodaconnect/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      411 2021-06-23 14:14:13.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/skodaconnect/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-06-23 14:14:13.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/skodaconnect/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       54 2021-08-23 22:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/skodaconnect/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    10329 2021-08-23 16:37:52.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/skodaconnect/skodaconnect.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/spotify/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      704 2020-12-29 20:40:38.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/spotify/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-29 20:40:38.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/spotify/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       49 2021-05-04 17:54:36.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/spotify/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    14603 2021-05-04 17:54:36.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/spotify/spotify.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/spotify_connect_player/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      164 2021-01-05 09:10:54.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/spotify_connect_player/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-01-05 09:10:54.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/spotify_connect_player/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       88 2021-01-05 09:10:54.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/spotify_connect_player/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     7093 2021-05-04 17:54:36.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/spotify_connect_player/spotify_connect_player.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2454 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-01-08 21:51:39.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2972 2021-01-08 21:51:39.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya/const.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       49 2021-03-01 19:58:59.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)  3022362 2021-01-29 20:18:28.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya/mappings.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    21035 2021-07-30 18:50:12.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya/tuya.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya_cloud/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1333 2021-08-23 16:54:59.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya_cloud/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       11 2021-07-30 18:50:12.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya_cloud/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      374 2021-07-30 18:50:12.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya_cloud/const.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       56 2021-08-08 16:09:35.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya_cloud/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1910 2021-08-26 16:11:06.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya_cloud/tuya_cloud.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    11954 2021-08-27 17:39:12.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya_cloud/tuya_cloud_device.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     7497 2021-08-26 21:58:20.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya_cloud/tuya_cloud_setup.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     8632 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/utils.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       23 2021-08-27 17:39:13.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/version.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/volvooncall/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-08-07 19:48:15.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/volvooncall/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       53 2021-08-07 19:49:24.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/volvooncall/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    10200 2021-08-07 19:52:36.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/volvooncall/volvooncall.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/warema/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2021-08-27 17:39:11.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/warema/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       56 2021-08-27 17:39:11.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/warema/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     6362 2021-08-27 17:39:11.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/warema/warema.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/wienerlinien/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      266 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/wienerlinien/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       32 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/wienerlinien/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       34 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/wienerlinien/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4266 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/wienerlinien/wienerlinien.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      604 2020-12-22 22:51:37.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/__init__.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       14 2020-12-23 07:30:08.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    11967 2021-02-14 19:56:31.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/bluetooth.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    38790 2021-02-14 19:56:31.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/gateway3.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     7962 2021-02-14 19:56:31.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/mini_miio.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     5703 2021-02-14 19:56:31.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/shell.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     6239 2021-02-02 20:34:04.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/unqlite.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    20234 2021-02-14 19:56:31.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/utils.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     8064 2021-02-14 19:56:31.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/xiaomi_cloud.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       91 2020-12-22 22:51:37.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1855 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/miio_fix.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4848 2021-02-14 19:56:31.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/xiaomi_gateway3.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       31 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/__init__.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-26 20:05:39.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3513 2021-07-31 06:55:31.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/base.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2160 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/gateway.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1800 2021-02-10 20:33:08.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/sensor.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       61 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4080 2021-08-17 21:02:28.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/xiaomi_gateway3_device.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      805 2020-12-22 22:56:16.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       25 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       34 2020-12-09 20:57:30.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/manifest.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     6972 2021-02-14 19:56:31.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/xiaomi_tokens.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy.egg-info/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     9285 2021-08-27 17:39:17.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy.egg-info/PKG-INFO
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    11915 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy.egg-info/SOURCES.txt
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        1 2021-08-27 17:39:17.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy.egg-info/dependency_links.txt
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       79 2021-08-27 17:39:17.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy.egg-info/requires.txt
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       13 2021-08-27 17:39:17.000000 fhempy-0.1.99/FHEM/bindings/python/fhempy.egg-info/top_level.txt
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/tests/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-05 09:10:54.000000 fhempy-0.1.99/FHEM/bindings/python/tests/__init__.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/__init__.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/__init__.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/__init__.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      566 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_chime_health_attrs.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    10303 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_devices.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      882 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_ding_active.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      566 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_doorboot_health_attrs.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      566 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_doorboot_health_attrs_id987653.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      220 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_doorbots.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      214 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_oauth.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1248 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_session.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     5572 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/test_basics.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/__init__.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1095 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/device.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3518 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/devices.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1208 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/local_devices.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      234 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/token.json
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     3900 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/test_device_ctrl.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2356 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/test_setup.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     2246 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/test_modules_basic.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1049 2021-08-02 20:47:28.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/test_update.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     8731 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/tests/mocked/test_utils.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:22.000000 fhempy-0.1.99/FHEM/bindings/python/tests/reallife/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/reallife/__init__.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:23.000000 fhempy-0.1.99/FHEM/bindings/python/tests/reallife/modules/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/reallife/modules/__init__.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:23.000000 fhempy-0.1.99/FHEM/bindings/python/tests/reallife/modules/googlecast/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/reallife/modules/googlecast/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4598 2021-02-01 17:04:33.000000 fhempy-0.1.99/FHEM/bindings/python/tests/reallife/modules/googlecast/test_reallife_basics.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:23.000000 fhempy-0.1.99/FHEM/bindings/python/tests/reallife/modules/xiaomi_gateway3/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-02-14 19:56:31.000000 fhempy-0.1.99/FHEM/bindings/python/tests/reallife/modules/xiaomi_gateway3/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4547 2021-02-14 19:56:31.000000 fhempy-0.1.99/FHEM/bindings/python/tests/reallife/modules/xiaomi_gateway3/test_general.py
+drwxr-xr-x   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-08-27 17:39:23.000000 fhempy-0.1.99/FHEM/bindings/python/tests/utils/
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)        0 2021-01-20 20:58:13.000000 fhempy-0.1.99/FHEM/bindings/python/tests/utils/__init__.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     4224 2021-02-14 19:56:31.000000 fhempy-0.1.99/FHEM/bindings/python/tests/utils/mock_fhem.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1070 2020-12-04 22:15:54.000000 fhempy-0.1.99/LICENSE
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       94 2021-01-27 22:27:34.000000 fhempy-0.1.99/MANIFEST.in
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     9285 2021-08-27 17:39:23.000000 fhempy-0.1.99/PKG-INFO
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     7763 2021-08-25 20:02:45.000000 fhempy-0.1.99/README.md
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      359 2021-08-27 17:39:12.000000 fhempy-0.1.99/controls_pythonbinding.txt
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      463 2020-12-07 19:21:53.000000 fhempy-0.1.99/fhempy.service
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)    32747 2020-09-19 15:52:13.000000 fhempy-0.1.99/flowchart.png
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      536 2021-01-20 20:58:13.000000 fhempy-0.1.99/install_python.sh
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      234 2020-12-05 19:16:34.000000 fhempy-0.1.99/install_systemd_fhempy.sh
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      916 2021-01-05 09:11:25.000000 fhempy-0.1.99/prepare_update.pl
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      670 2021-01-30 19:42:20.000000 fhempy-0.1.99/release.sh
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       78 2021-02-17 20:10:58.000000 fhempy-0.1.99/requirements.txt
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      188 2021-03-01 21:14:39.000000 fhempy-0.1.99/requirements_dev.txt
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      164 2021-02-17 20:10:58.000000 fhempy-0.1.99/requirements_tests.txt
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)       38 2021-08-27 17:39:23.000000 fhempy-0.1.99/setup.cfg
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)     1161 2021-01-27 22:09:58.000000 fhempy-0.1.99/setup.py
+-rw-r--r--   0 dominikkarall  (1000) dominikkarall  (1000)      259 2021-01-29 20:43:25.000000 fhempy-0.1.99/tox.ini
```

### Comparing `fhempy-0.1.98/.github/workflows/release.yml` & `fhempy-0.1.99/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/.github/workflows/tests.yml` & `fhempy-0.1.99/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/.gitignore` & `fhempy-0.1.99/.gitignore`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/CHANGED` & `fhempy-0.1.99/CHANGED`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/CHANGELOG.md` & `fhempy-0.1.99/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.99 (2021-08-27)
+### Fix
+* **tuya_cloud:** Fix colour_data again ([`fd37524`](https://github.com/dominikkarall/fhempy/commit/fd37524f94bc30667b75849b1933e223d92df361))
+
 ## v0.1.98 (2021-08-27)
 ### Fix
 * **tuya_cloud:** Fix again colour_data ([`82998c7`](https://github.com/dominikkarall/fhempy/commit/82998c757357c9c9aee4fbc0b7c83ac8d9170cfb))
 
 ## v0.1.97 (2021-08-26)
 ### Fix
 * **tuya_cloud:** Handle exception on mqtt stop ([`de40876`](https://github.com/dominikkarall/fhempy/commit/de4087678f95429e9c86bf4ee3cd767f6836a326))
```

### Comparing `fhempy-0.1.98/FHEM/10_BindingsIo.pm` & `fhempy-0.1.99/FHEM/10_BindingsIo.pm`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/10_PythonBinding.pm` & `fhempy-0.1.99/FHEM/10_PythonBinding.pm`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/10_PythonModule.pm` & `fhempy-0.1.99/FHEM/10_PythonModule.pm`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/bin/fhempy` & `fhempy-0.1.99/FHEM/bindings/python/bin/fhempy`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_presence/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_presence/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_presence/ble_presence.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_presence/ble_presence.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_reset/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_reset/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ble_reset/ble_reset.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ble_reset/ble_reset.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/bt_presence/bt_presence.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/bt_presence/bt_presence.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/ble.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/ble.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/discover_fhempy/discover_fhempy.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/discover_fhempy/discover_fhempy.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/ssdp.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/ssdp.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/core/zeroconf.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/core/zeroconf.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_ble/discover_ble.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_ble/discover_ble.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_mdns/discover_mdns.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_mdns/discover_mdns.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/discover_upnp/discover_upnp.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/discover_upnp/discover_upnp.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/dlna_dmr/dlna_dmr.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/dlna_dmr/dlna_dmr.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/connection.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/connection.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/eq3bt.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/eq3bt.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/eq3btsmart.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/eq3btsmart.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/screenshot.png` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/screenshot.png`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/eq3bt/structures.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/eq3bt/structures.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/erelax_vaillant/erelax_vaillant.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/erelax_vaillant/erelax_vaillant.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/esphome/esphome.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/esphome/esphome.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/fhem.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/fhem.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/fhem_pythonbinding.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/fhem_pythonbinding.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/fusionsolar/const.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/fusionsolar/const.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/fusionsolar/fusionsolar_api.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/fusionsolar/fusionsolar_api.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/fusionsolar/fusiosolar.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/fusionsolar/fusiosolar.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/generic.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/generic.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/gfprobt/gfprobt.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/gfprobt/gfprobt.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/googlecast/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/googlecast/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/googlecast/googlecast.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/googlecast/googlecast.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/googlecast/screenshot.png` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/googlecast/screenshot.png`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/helloworld/helloworld.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miflora/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miflora/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miflora/miflora.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miflora/miflora.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miio/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miio/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/miio/miio.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/miio/miio.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp/mitemp.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp/mitemp.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp2/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp2/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/mitemp2/mitemp2.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/mitemp2/mitemp2.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/nespresso_ble/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/nespresso_ble/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/nespresso_ble/nespresso.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/nespresso_ble/nespresso.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/nespresso_ble/nespresso_ble.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/nespresso_ble/nespresso_ble.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/object_detection/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/object_detection/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/object_detection/detect.tflite` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/object_detection/detect.tflite`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/object_detection/labelmap.txt` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/object_detection/labelmap.txt`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/object_detection/object_detection.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/object_detection/object_detection.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/pkg_installer.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/pkg_installer.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/ring/ring.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/ring/ring.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/skodaconnect/skodaconnect.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/skodaconnect/skodaconnect.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/spotify/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/spotify/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/spotify/spotify.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/spotify/spotify.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/spotify_connect_player/spotify_connect_player.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/spotify_connect_player/spotify_connect_player.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya/const.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya/const.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya/mappings.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya/mappings.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya/tuya.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya/tuya.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya_cloud/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya_cloud/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya_cloud/tuya_cloud.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya_cloud/tuya_cloud.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya_cloud/tuya_cloud_device.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya_cloud/tuya_cloud_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,16 +309,16 @@
         else:
             rgb = colorsys.hsv_to_rgb(
                 int(hsv_json["h"]) / 360,
                 int(hsv_json["s"]) / 1000,
                 int(hsv_json["v"]) / 1000,
             )
 
-        red = rgb[0]
-        green = rgb[1]
-        blue = rgb[2]
+        red = int(rgb[0] * 255)
+        green = int(rgb[1] * 255)
+        blue = int(rgb[2] * 255)
         rgb_hex = f"{red:02x}{green:02x}{blue:02x}"
         await fhem.readingsBulkUpdate(
             self.hash,
             hsv_code,
             rgb_hex,
         )
```

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/tuya_cloud/tuya_cloud_setup.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/tuya_cloud/tuya_cloud_setup.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/utils.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/utils.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/volvooncall/volvooncall.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/volvooncall/volvooncall.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/warema/warema.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/warema/warema.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/wienerlinien/wienerlinien.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/wienerlinien/wienerlinien.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/bluetooth.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/bluetooth.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/gateway3.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/gateway3.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/mini_miio.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/mini_miio.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/shell.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/shell.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/unqlite.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/unqlite.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/utils.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/utils.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/xiaomi_cloud.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/core/xiaomi_cloud.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/miio_fix.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/miio_fix.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/xiaomi_gateway3.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3/xiaomi_gateway3.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/base.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/base.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/gateway.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/gateway.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/sensor.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/xiaomi_gateway3_device.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_gateway3_device/xiaomi_gateway3_device.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/README.md` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/xiaomi_tokens.py` & `fhempy-0.1.99/FHEM/bindings/python/fhempy/lib/xiaomi_tokens/xiaomi_tokens.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy.egg-info/PKG-INFO` & `fhempy-0.1.99/FHEM/bindings/python/fhempy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhempy
-Version: 0.1.98
+Version: 0.1.99
 Summary: Python binding for FHEM to support Python modules
 Home-page: https://github.com/dominikkarall/fhempy/
 Author: Dominik Karall
 Author-email: dominik.karall@gmail.com
 License: UNKNOWN
 Description: [![Download](https://img.shields.io/pypi/dm/fhempy)](https://pypistats.org/packages/fhempy)
         [![python](https://img.shields.io/badge/python-3.7+-critical)](https://github.com/dominikkarall/fhempy)
```

### Comparing `fhempy-0.1.98/FHEM/bindings/python/fhempy.egg-info/SOURCES.txt` & `fhempy-0.1.99/FHEM/bindings/python/fhempy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_chime_health_attrs.json` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_chime_health_attrs.json`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_devices.json` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_devices.json`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_ding_active.json` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_ding_active.json`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_doorboot_health_attrs.json` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_doorboot_health_attrs.json`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_doorboot_health_attrs_id987653.json` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_doorboot_health_attrs_id987653.json`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_session.json` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/fixtures/ring_session.json`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/ring/test_basics.py` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/ring/test_basics.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/device.json` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/device.json`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/devices.json` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/devices.json`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/local_devices.json` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/fixtures/local_devices.json`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/test_device_ctrl.py` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/test_device_ctrl.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/modules/tuya/test_setup.py` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/modules/tuya/test_setup.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/test_modules_basic.py` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/test_update.py` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/test_update.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/mocked/test_utils.py` & `fhempy-0.1.99/FHEM/bindings/python/tests/mocked/test_utils.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/reallife/modules/googlecast/test_reallife_basics.py` & `fhempy-0.1.99/FHEM/bindings/python/tests/reallife/modules/googlecast/test_reallife_basics.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/reallife/modules/xiaomi_gateway3/test_general.py` & `fhempy-0.1.99/FHEM/bindings/python/tests/reallife/modules/xiaomi_gateway3/test_general.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/FHEM/bindings/python/tests/utils/mock_fhem.py` & `fhempy-0.1.99/FHEM/bindings/python/tests/utils/mock_fhem.py`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/LICENSE` & `fhempy-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/PKG-INFO` & `fhempy-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhempy
-Version: 0.1.98
+Version: 0.1.99
 Summary: Python binding for FHEM to support Python modules
 Home-page: https://github.com/dominikkarall/fhempy/
 Author: Dominik Karall
 Author-email: dominik.karall@gmail.com
 License: UNKNOWN
 Description: [![Download](https://img.shields.io/pypi/dm/fhempy)](https://pypistats.org/packages/fhempy)
         [![python](https://img.shields.io/badge/python-3.7+-critical)](https://github.com/dominikkarall/fhempy)
```

### Comparing `fhempy-0.1.98/README.md` & `fhempy-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/flowchart.png` & `fhempy-0.1.99/flowchart.png`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/install_python.sh` & `fhempy-0.1.99/install_python.sh`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/prepare_update.pl` & `fhempy-0.1.99/prepare_update.pl`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/release.sh` & `fhempy-0.1.99/release.sh`

 * *Files identical despite different names*

### Comparing `fhempy-0.1.98/setup.py` & `fhempy-0.1.99/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/bosch-thermostat-client-0.9.8.tar.gz` & `tmp/bosch-thermostat-client-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bosch-thermostat-client-0.9.8.tar", last modified: Fri Dec 11 17:57:00 2020, max compression
+gzip compressed data, was "dist/bosch-thermostat-client-0.9.9.tar", last modified: Fri Dec 11 18:06:25 2020, max compression
```

## Comparing `bosch-thermostat-client-0.9.8.tar` & `bosch-thermostat-client-0.9.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 17:57:00.033896 bosch-thermostat-client-0.9.8/
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)    11357 2019-02-11 16:20:25.000000 bosch-thermostat-client-0.9.8/LICENSE.txt
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)       83 2020-04-25 18:28:05.000000 bosch-thermostat-client-0.9.8/MANIFEST.in
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     3208 2020-12-11 17:57:00.033896 bosch-thermostat-client-0.9.8/PKG-INFO
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1712 2020-04-27 09:41:41.000000 bosch-thermostat-client-0.9.8/README.md
-drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 17:57:00.027229 bosch-thermostat-client-0.9.8/bosch_thermostat_client/
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      464 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/__init__.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     7057 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/bosch_examples.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     4417 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/bosch_rawscan_cli.py
-drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 17:57:00.030562 bosch-thermostat-client-0.9.8/bosch_thermostat_client/circuits/
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)       55 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/circuits/__init__.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     8325 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/circuits/circuit.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     2702 2020-12-11 17:53:30.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/circuits/circuits.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     5833 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/circuits/ivt_circuit.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     2661 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/circuits/nefit_circuit.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1761 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/circuits/operation_mode.py
-drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 17:57:00.030562 bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      429 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/__init__.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     3425 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/http.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1603 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/ivt.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1244 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/nefit.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1463 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/nefit2.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     3547 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/nefitxmpp.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     4381 2020-12-11 13:27:06.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/xmpp.py
-drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 17:57:00.030562 bosch-thermostat-client-0.9.8/bosch_thermostat_client/const/
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1938 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/const/__init__.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      788 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/const/ivt.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      170 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/const/nefit.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      644 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/const_old.py
-drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 17:57:00.033896 bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1676 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/__init__.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     6913 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/can.json
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1285 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/db_IVT.json
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      624 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/db_NEFIT.json
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     8806 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/default.json
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)    95967 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/errorcodes_ivt.json
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     5372 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/nefit.json
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     9851 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/nsc_icom_gateway.json
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)    34751 2020-12-11 17:53:02.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/rc300.json
-drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 17:57:00.033896 bosch-thermostat-client-0.9.8/bosch_thermostat_client/encryption/
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      137 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/encryption/__init__.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     3006 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/encryption/base_encryption.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      235 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/encryption/ivt_encryption.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      242 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/encryption/nefit_encryption.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      496 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/errors.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1197 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/exceptions.py
-drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 17:57:00.033896 bosch-thermostat-client-0.9.8/bosch_thermostat_client/gateway/
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      228 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/gateway/__init__.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     8181 2020-12-11 17:54:42.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/gateway/base_gateway.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     3217 2020-12-07 06:55:18.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/gateway/ivt_gateway.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     2627 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/gateway/nefit_gateway.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     6644 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/helper.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     9556 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/schedule.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     4551 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/sensors.py
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)       37 2020-12-11 17:55:18.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client/version.py
-drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 17:57:00.030562 bosch-thermostat-client-0.9.8/bosch_thermostat_client.egg-info/
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     3208 2020-12-11 17:56:59.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client.egg-info/PKG-INFO
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     2185 2020-12-11 17:56:59.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client.egg-info/SOURCES.txt
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)        1 2020-12-11 17:56:59.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client.egg-info/dependency_links.txt
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      138 2020-12-11 17:56:59.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client.egg-info/entry_points.txt
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)       38 2020-12-11 17:56:59.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client.egg-info/requires.txt
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)       24 2020-12-11 17:56:59.000000 bosch-thermostat-client-0.9.8/bosch_thermostat_client.egg-info/top_level.txt
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)       38 2020-12-11 17:57:00.033896 bosch-thermostat-client-0.9.8/setup.cfg
--rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1782 2020-04-27 10:05:13.000000 bosch-thermostat-client-0.9.8/setup.py
+drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 18:06:25.225205 bosch-thermostat-client-0.9.9/
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)    11357 2019-02-11 16:20:25.000000 bosch-thermostat-client-0.9.9/LICENSE.txt
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)       83 2020-04-25 18:28:05.000000 bosch-thermostat-client-0.9.9/MANIFEST.in
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     3208 2020-12-11 18:06:25.225205 bosch-thermostat-client-0.9.9/PKG-INFO
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1712 2020-04-27 09:41:41.000000 bosch-thermostat-client-0.9.9/README.md
+drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 18:06:25.221872 bosch-thermostat-client-0.9.9/bosch_thermostat_client/
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      464 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/__init__.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     7057 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/bosch_examples.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     4417 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/bosch_rawscan_cli.py
+drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 18:06:25.221872 bosch-thermostat-client-0.9.9/bosch_thermostat_client/circuits/
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)       55 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/circuits/__init__.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     8325 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/circuits/circuit.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     2702 2020-12-11 17:53:30.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/circuits/circuits.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     5833 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/circuits/ivt_circuit.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     2661 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/circuits/nefit_circuit.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1761 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/circuits/operation_mode.py
+drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 18:06:25.221872 bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      429 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/__init__.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     3425 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/http.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1603 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/ivt.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1244 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/nefit.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1463 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/nefit2.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     3547 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/nefitxmpp.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     4381 2020-12-11 13:27:06.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/xmpp.py
+drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 18:06:25.221872 bosch-thermostat-client-0.9.9/bosch_thermostat_client/const/
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1938 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/const/__init__.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      788 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/const/ivt.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      170 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/const/nefit.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      644 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/const_old.py
+drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 18:06:25.221872 bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1676 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/__init__.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     6913 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/can.json
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1285 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/db_IVT.json
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      624 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/db_NEFIT.json
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     8806 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/default.json
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)    95967 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/errorcodes_ivt.json
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     5372 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/nefit.json
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     9851 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/nsc_icom_gateway.json
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)    34931 2020-12-11 18:05:33.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/rc300.json
+drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 18:06:25.225205 bosch-thermostat-client-0.9.9/bosch_thermostat_client/encryption/
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      137 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/encryption/__init__.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     3006 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/encryption/base_encryption.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      235 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/encryption/ivt_encryption.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      242 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/encryption/nefit_encryption.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      496 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/errors.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1197 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/exceptions.py
+drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 18:06:25.225205 bosch-thermostat-client-0.9.9/bosch_thermostat_client/gateway/
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      228 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/gateway/__init__.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     8181 2020-12-11 17:54:42.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/gateway/base_gateway.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     3217 2020-12-07 06:55:18.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/gateway/ivt_gateway.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     2627 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/gateway/nefit_gateway.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     6644 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/helper.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     9556 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/schedule.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     4551 2020-12-07 06:38:35.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/sensors.py
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)       37 2020-12-11 18:05:52.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client/version.py
+drwxr-xr-x   0 admin    (1175200500) użytkownicy domeny (1175200513)        0 2020-12-11 18:06:25.221872 bosch-thermostat-client-0.9.9/bosch_thermostat_client.egg-info/
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     3208 2020-12-11 18:06:25.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client.egg-info/PKG-INFO
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     2185 2020-12-11 18:06:25.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client.egg-info/SOURCES.txt
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)        1 2020-12-11 18:06:25.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client.egg-info/dependency_links.txt
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)      138 2020-12-11 18:06:25.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client.egg-info/entry_points.txt
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)       38 2020-12-11 18:06:25.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client.egg-info/requires.txt
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)       24 2020-12-11 18:06:25.000000 bosch-thermostat-client-0.9.9/bosch_thermostat_client.egg-info/top_level.txt
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)       38 2020-12-11 18:06:25.225205 bosch-thermostat-client-0.9.9/setup.cfg
+-rw-r--r--   0 admin    (1175200500) użytkownicy domeny (1175200513)     1782 2020-04-27 10:05:13.000000 bosch-thermostat-client-0.9.9/setup.py
```

### Comparing `bosch-thermostat-client-0.9.8/LICENSE.txt` & `bosch-thermostat-client-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/PKG-INFO` & `bosch-thermostat-client-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bosch-thermostat-client
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python API for talking to Bosch™ Heating gateway using HTTP or XMPP
 Home-page: https://github.com/bosch-thermostat/bosch-thermostat-client-python
 Author: Ludovic Laurent, Pawel Szafer
 Author-email: ludovic.laurent@gmail.com, pszafer@gmail.com
 License: Apache License 2.0
-Download-URL: https://github.com/bosch-thermostat/bosch-thermostat-client-python/archive/0.9.8.zip
+Download-URL: https://github.com/bosch-thermostat/bosch-thermostat-client-python/archive/0.9.9.zip
 Description: 
         
         # bosch-thermostat-client-python
         Python3 asyncio package to talk to Bosch Thermostats via their gateway.
         Suppored protocols are HTTP and XMPP.
         
         Both are still in development.
```

### Comparing `bosch-thermostat-client-0.9.8/README.md` & `bosch-thermostat-client-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/bosch_examples.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/bosch_examples.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/bosch_rawscan_cli.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/bosch_rawscan_cli.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/circuits/circuit.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/circuits/circuit.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/circuits/circuits.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/circuits/circuits.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/circuits/ivt_circuit.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/circuits/ivt_circuit.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/circuits/nefit_circuit.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/circuits/nefit_circuit.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/circuits/operation_mode.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/circuits/operation_mode.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/http.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/http.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/ivt.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/ivt.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/nefit.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/nefit.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/nefit2.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/nefit2.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/nefitxmpp.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/nefitxmpp.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/connectors/xmpp.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/connectors/xmpp.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/const/__init__.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/const/__init__.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/const/ivt.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/const/ivt.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/const_old.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/const_old.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/__init__.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/__init__.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/can.json` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/can.json`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/db_IVT.json` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/db_IVT.json`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/db_NEFIT.json` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/db_NEFIT.json`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/default.json` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/default.json`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/errorcodes_ivt.json` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/errorcodes_ivt.json`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/nefit.json` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/nefit.json`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/nsc_icom_gateway.json` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/nsc_icom_gateway.json`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/db/rc300.json` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/db/rc300.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998015873015872%*

 * *Differences: {"'04.07.05'": "{'heatingCircuits': {'sensors': {'actualSupplyTemperature': OrderedDict([('id', "*

 * *               "'actualSupplyTemperature'), ('name', 'Actual supply temperature for HC')])}}}"}*

```diff
@@ -893,14 +893,18 @@
                 "switchPrograms": {
                     "id": "switchPrograms",
                     "name": "Switch Programs",
                     "type": "regular"
                 }
             },
             "sensors": {
+                "actualSupplyTemperature": {
+                    "id": "actualSupplyTemperature",
+                    "name": "Actual supply temperature for HC"
+                },
                 "currentSuWiMode": {
                     "id": "currentSuWiMode",
                     "name": "Current Summer Winter Mode"
                 },
                 "pumpModulation": {
                     "id": "pumpModulation",
                     "name": "Pump Modulation"
```

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/encryption/base_encryption.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/encryption/base_encryption.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/exceptions.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/gateway/base_gateway.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/gateway/base_gateway.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/gateway/ivt_gateway.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/gateway/ivt_gateway.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/gateway/nefit_gateway.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/gateway/nefit_gateway.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/helper.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/helper.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/schedule.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/schedule.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client/sensors.py` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client/sensors.py`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client.egg-info/PKG-INFO` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bosch-thermostat-client
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python API for talking to Bosch™ Heating gateway using HTTP or XMPP
 Home-page: https://github.com/bosch-thermostat/bosch-thermostat-client-python
 Author: Ludovic Laurent, Pawel Szafer
 Author-email: ludovic.laurent@gmail.com, pszafer@gmail.com
 License: Apache License 2.0
-Download-URL: https://github.com/bosch-thermostat/bosch-thermostat-client-python/archive/0.9.8.zip
+Download-URL: https://github.com/bosch-thermostat/bosch-thermostat-client-python/archive/0.9.9.zip
 Description: 
         
         # bosch-thermostat-client-python
         Python3 asyncio package to talk to Bosch Thermostats via their gateway.
         Suppored protocols are HTTP and XMPP.
         
         Both are still in development.
```

### Comparing `bosch-thermostat-client-0.9.8/bosch_thermostat_client.egg-info/SOURCES.txt` & `bosch-thermostat-client-0.9.9/bosch_thermostat_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bosch-thermostat-client-0.9.8/setup.py` & `bosch-thermostat-client-0.9.9/setup.py`

 * *Files identical despite different names*


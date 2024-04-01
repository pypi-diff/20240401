# Comparing `tmp/alas-ce0-client-4.0.9.tar.gz` & `tmp/alas-ce0-client-5.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alas-ce0-client-4.0.9.tar", last modified: Thu Aug 18 00:04:33 2022, max compression
+gzip compressed data, was "alas-ce0-client-5.0.78.tar", last modified: Thu Mar 14 12:19:41 2024, max compression
```

## Comparing `alas-ce0-client-4.0.9.tar` & `alas-ce0-client-5.0.78.tar`

### file list

```diff
@@ -1,68 +1,71 @@
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/
--rw-r--r--   0 lzambra    (501) staff       (20)      950 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/PKG-INFO
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/clients/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/clients/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      748 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/clients/core.py
--rw-r--r--   0 lzambra    (501) staff       (20)     6223 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/clients/api_client.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/reporting/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/reporting/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      323 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/reporting/regional_partner_report.py
--rw-r--r--   0 lzambra    (501) staff       (20)      311 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/reporting/report_manager.py
--rw-r--r--   0 lzambra    (501) staff       (20)      495 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/reporting/report.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/scheduling/
--rw-r--r--   0 lzambra    (501) staff       (20)     2412 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/scheduling/route.py
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/scheduling/__init__.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/integration/
--rw-r--r--   0 lzambra    (501) staff       (20)      274 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/integration/shipper.py
--rw-r--r--   0 lzambra    (501) staff       (20)      283 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/integration/whatsapp.py
--rw-r--r--   0 lzambra    (501) staff       (20)      596 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/integration/device_magic.py
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/integration/__init__.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/management/
--rw-r--r--   0 lzambra    (501) staff       (20)      349 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/distribution_zone.py
--rw-r--r--   0 lzambra    (501) staff       (20)      462 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/geographic_coverage_active.py
--rw-r--r--   0 lzambra    (501) staff       (20)      531 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/configuration.py
--rw-r--r--   0 lzambra    (501) staff       (20)      584 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/user.py
--rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/task.py
--rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/shelf.py
--rw-r--r--   0 lzambra    (501) staff       (20)      336 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/service_level.py
--rw-r--r--   0 lzambra    (501) staff       (20)      160 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/roles_group.py
--rw-r--r--   0 lzambra    (501) staff       (20)     1130 2022-07-17 21:07:20.000000 alas-ce0-client-4.0.9/alas_ce0/management/bulk.py
--rw-r--r--   0 lzambra    (501) staff       (20)      337 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/maintenance.py
--rw-r--r--   0 lzambra    (501) staff       (20)      757 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/notification.py
--rw-r--r--   0 lzambra    (501) staff       (20)      316 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/vehicle.py
--rw-r--r--   0 lzambra    (501) staff       (20)      155 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/resource.py
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      169 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/product_template.py
--rw-r--r--   0 lzambra    (501) staff       (20)      147 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/role.py
--rw-r--r--   0 lzambra    (501) staff       (20)      153 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/feature.py
--rw-r--r--   0 lzambra    (501) staff       (20)      352 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/packaging.py
--rw-r--r--   0 lzambra    (501) staff       (20)      917 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/employee.py
--rw-r--r--   0 lzambra    (501) staff       (20)      609 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/barcode.py
--rw-r--r--   0 lzambra    (501) staff       (20)      362 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/cross_docking.py
--rw-r--r--   0 lzambra    (501) staff       (20)      298 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/package_template.py
--rw-r--r--   0 lzambra    (501) staff       (20)     1066 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/delivery_entity.py
--rw-r--r--   0 lzambra    (501) staff       (20)      492 2022-08-17 20:26:11.000000 alas-ce0-client-4.0.9/alas_ce0/management/geographic_coverage.py
--rw-r--r--   0 lzambra    (501) staff       (20)      152 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/management/contact.py
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/__init__.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/common/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/common/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)    12200 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/common/client_base.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/task/
--rw-r--r--   0 lzambra    (501) staff       (20)      289 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/task/data_job.py
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/task/__init__.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0/delivery/
--rw-r--r--   0 lzambra    (501) staff       (20)      307 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/delivery/b2c.py
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/alas_ce0/delivery/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)    34402 2022-08-18 00:03:42.000000 alas-ce0-client-4.0.9/alas_ce0/delivery/delivery_order.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0_client.egg-info/
--rw-r--r--   0 lzambra    (501) staff       (20)      950 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0_client.egg-info/PKG-INFO
--rw-r--r--   0 lzambra    (501) staff       (20)     1758 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0_client.egg-info/SOURCES.txt
--rw-r--r--   0 lzambra    (501) staff       (20)       55 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0_client.egg-info/requires.txt
--rw-r--r--   0 lzambra    (501) staff       (20)        9 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0_client.egg-info/top_level.txt
--rw-r--r--   0 lzambra    (501) staff       (20)        1 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/alas_ce0_client.egg-info/dependency_links.txt
--rw-r--r--   0 lzambra    (501) staff       (20)      238 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/MANIFEST.in
--rw-r--r--   0 lzambra    (501) staff       (20)     3892 2022-08-18 00:04:09.000000 alas-ce0-client-4.0.9/setup.py
--rw-r--r--   0 lzambra    (501) staff       (20)       67 2022-08-18 00:04:33.000000 alas-ce0-client-4.0.9/setup.cfg
--rw-r--r--   0 lzambra    (501) staff       (20)      260 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/README.rst
--rw-r--r--   0 lzambra    (501) staff       (20)       23 2022-07-06 21:05:07.000000 alas-ce0-client-4.0.9/LICENSE.txt
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.151336 alas-ce0-client-5.0.78/
+-rw-r--r--   0 lzambra    (501) staff       (20)       23 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/LICENSE.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)      238 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/MANIFEST.in
+-rw-r--r--   0 lzambra    (501) staff       (20)      955 2024-03-14 12:19:41.151047 alas-ce0-client-5.0.78/PKG-INFO
+-rw-r--r--   0 lzambra    (501) staff       (20)      260 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/README.rst
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.115693 alas-ce0-client-5.0.78/alas_ce0/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/__init__.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.117614 alas-ce0-client-5.0.78/alas_ce0/clients/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/clients/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     6223 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/clients/api_client.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      748 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/clients/core.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.118642 alas-ce0-client-5.0.78/alas_ce0/common/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/common/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)    12200 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/common/client_base.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.124001 alas-ce0-client-5.0.78/alas_ce0/delivery/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/delivery/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      307 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/delivery/b2c.py
+-rw-r--r--   0 lzambra    (501) staff       (20)    51736 2024-03-10 18:52:47.000000 alas-ce0-client-5.0.78/alas_ce0/delivery/delivery_order.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.129163 alas-ce0-client-5.0.78/alas_ce0/integration/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/integration/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      596 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/integration/device_magic.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      274 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/integration/shipper.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      283 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/integration/whatsapp.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.143556 alas-ce0-client-5.0.78/alas_ce0/management/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      609 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/barcode.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     1511 2024-02-12 13:05:56.000000 alas-ce0-client-5.0.78/alas_ce0/management/bulk.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      531 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/configuration.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      152 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/contact.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      362 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/cross_docking.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     1066 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/delivery_entity.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      349 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/distribution_zone.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      917 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/employee.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      153 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/feature.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      492 2022-08-17 20:26:11.000000 alas-ce0-client-5.0.78/alas_ce0/management/geographic_coverage.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      462 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/geographic_coverage_active.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      337 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/maintenance.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      757 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/notification.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      298 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/package_template.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      352 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/packaging.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      732 2024-02-12 13:05:56.000000 alas-ce0-client-5.0.78/alas_ce0/management/pallet.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      155 2024-02-12 13:10:27.000000 alas-ce0-client-5.0.78/alas_ce0/management/position.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      169 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/product_template.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      155 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/resource.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      147 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/role.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      160 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/roles_group.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      336 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/service_level.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/shelf.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/task.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      584 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/user.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      591 2024-02-12 13:05:56.000000 alas-ce0-client-5.0.78/alas_ce0/management/user_app.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      316 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/vehicle.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.145181 alas-ce0-client-5.0.78/alas_ce0/reporting/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/reporting/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      323 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/reporting/regional_partner_report.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      495 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/reporting/report.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      311 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/reporting/report_manager.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.145940 alas-ce0-client-5.0.78/alas_ce0/scheduling/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/scheduling/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     2412 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/scheduling/route.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.146869 alas-ce0-client-5.0.78/alas_ce0/task/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/task/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      289 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/task/data_job.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.150188 alas-ce0-client-5.0.78/alas_ce0_client.egg-info/
+-rw-r--r--   0 lzambra    (501) staff       (20)      955 2024-03-14 12:19:41.000000 alas-ce0-client-5.0.78/alas_ce0_client.egg-info/PKG-INFO
+-rw-r--r--   0 lzambra    (501) staff       (20)     1852 2024-03-14 12:19:41.000000 alas-ce0-client-5.0.78/alas_ce0_client.egg-info/SOURCES.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)        1 2024-03-14 12:19:41.000000 alas-ce0-client-5.0.78/alas_ce0_client.egg-info/dependency_links.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)       48 2024-03-14 12:19:41.000000 alas-ce0-client-5.0.78/alas_ce0_client.egg-info/requires.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)        9 2024-03-14 12:19:41.000000 alas-ce0-client-5.0.78/alas_ce0_client.egg-info/top_level.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)       67 2024-03-14 12:19:41.151950 alas-ce0-client-5.0.78/setup.cfg
+-rw-r--r--   0 lzambra    (501) staff       (20)     3807 2024-03-14 12:11:49.000000 alas-ce0-client-5.0.78/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `alas-ce0-client-4.0.9/alas_ce0/clients/core.py` & `alas-ce0-client-5.0.78/alas_ce0/clients/core.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.9/alas_ce0/clients/api_client.py` & `alas-ce0-client-5.0.78/alas_ce0/clients/api_client.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.9/alas_ce0/scheduling/route.py` & `alas-ce0-client-5.0.78/alas_ce0/scheduling/route.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.9/alas_ce0/integration/device_magic.py` & `alas-ce0-client-5.0.78/alas_ce0/integration/device_magic.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.9/alas_ce0/management/configuration.py` & `alas-ce0-client-5.0.78/alas_ce0/management/configuration.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.9/alas_ce0/management/user.py` & `alas-ce0-client-5.0.78/alas_ce0/management/user.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.9/alas_ce0/management/bulk.py` & `alas-ce0-client-5.0.78/alas_ce0/management/bulk.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,10 +16,18 @@
         return self.http_post_json(self.entity_endpoint_base_url + "_change-status", params)
 
     def ti_controlled_receive(self, code):
         return self.http_post_json(self.entity_endpoint_base_url + "_ti-controlled-receive", code)
 
     def ser_travelling_receive(self, code):
         return self.http_post_json(self.entity_endpoint_base_url + "_ser-travelling-receive", code)
+
+    def ser_travelling_receive_right(self, code, event_info):
+        return self.http_post_json(self.entity_endpoint_base_url + "{0}/_ser-travelling-receive-right".format(code), event_info)
     
     def cd_travelling_receive(self, id, event_info):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_cd-travelling-receive".format(id), event_info)
+
+    def get_attachment_content(self, id, att_file_name):
+        return self.http_get(
+            self.entity_endpoint_base_url + "{0}/attachment/{1}".format(id, att_file_name)
+        )
```

### Comparing `alas-ce0-client-4.0.9/alas_ce0/management/notification.py` & `alas-ce0-client-5.0.78/alas_ce0/management/notification.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.9/alas_ce0/management/employee.py` & `alas-ce0-client-5.0.78/alas_ce0/management/employee.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.9/alas_ce0/management/barcode.py` & `alas-ce0-client-5.0.78/alas_ce0/management/barcode.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.9/alas_ce0/management/delivery_entity.py` & `alas-ce0-client-5.0.78/alas_ce0/management/delivery_entity.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.9/alas_ce0/common/client_base.py` & `alas-ce0-client-5.0.78/alas_ce0/common/client_base.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-4.0.9/alas_ce0/delivery/delivery_order.py` & `alas-ce0-client-5.0.78/alas_ce0/delivery/delivery_order.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,15 +12,16 @@
         9: "Ingreso a Ce0",
         10: "Recepción Física TL (Nuevo Formato)",
     }
     
 def get_lob_order_dic():
     return {
         1: "Entrega",
-        2: "Retorno"        
+        2: "Retorno",
+        3: "Intercambio"
     }
     
 def get_delivery_order_status_description_dic():
     return {
         1: "En proceso de planificación",
         4: "En proceso de planificación",
         5: "Recibida por el tren logístico",
@@ -78,20 +79,45 @@
         37: "Robada",
         38: "Extraviada",
         39: "Retirada",
         40: "No Retirada",
         41: "No Retirable",
         42: "Viajando a CD",
         43: "Viajando B2B",
-        44: "Entregada B2B"
+        44: "Entregada B2B",
+        45: "Asignado Mensajero",
+        46: "Intercambiada",
+        47: "No Intercambiada",
+        48: "No Intercambiable",
+        49: "Recibido SER",
+        50: "Recibido Devoluciones",
+        51: "Cambio de Comuna",
+        52: "Cuarentena",
+        53: "PreAsignado Mensajero"
+    }
+
+def get_delivery_order_rejected_dic():
+    return {
+        1: "No hay quien reciba",
+        2: "Dirección Incompleta'",
+        3: "Problema de Documentación",
+        4: "Código Erróneo",
+        5: "Paso Automático",
+        6: "A pedido del B2B",
+        9: "Compra Anulada",
+        10: "Orden Duplicada",
+        11: "Paquete Dañado",
+        12: "Retiro Anulado",
+        14: "Sin Stock Para Remaquilar"
     }
 
 class LineOfBusinessType(Enum):
     Delivery = 1
     Pickup = 2
+    Exchange = 3
     
 LOB_TYPES = [e.value for e in LineOfBusinessType]
 
 class DeliveryOrderProcessType(Enum):
     B2bDelivery = 1
     B2bReception = 2
     Packaging = 3
@@ -164,29 +190,43 @@
     Missing  = 38    
     Withdrawn = 39 #Picking = 39
     NotWithdrawn = 40 #NotPicking = 40
     Nonwithdrable = 41 #NotPickingable = 41
     DistributionCenterTravelling = 42
     B2BTraveling = 43
     B2BDelivered = 44
+    DeliveryCourierAssigned = 45
+    Exchanged = 46
+    NotExchanged = 47
+    NotExchangable = 48
+    PickupSERReceived = 49
+    PickupDistributionCenterReceived = 50
+    WrongCrossDocking = 51
+    Quarantine = 52
+    DeliveryCourierPreAssigned = 53
+
+
     
 DELIVERY_ORDER_STATUS_TYPES = [e.value for e in DeliveryOrderStatusType]
 
 DELIVERY_ORDER_REJECTED_STATUSES = [
     DeliveryOrderStatusType.DeliveryRejected.value,
     DeliveryOrderStatusType.B2CRejected.value,
     DeliveryOrderStatusType.B2BReceptionRejected.value,
     DeliveryOrderStatusType.B2CReceptionRejected.value,
     DeliveryOrderStatusType.ALASRejected.value,
     DeliveryOrderStatusType.Steal.value,
-    DeliveryOrderStatusType.Missing.value
+    DeliveryOrderStatusType.Missing.value,
+    DeliveryOrderStatusType.WrongCrossDocking.value,
 ]
 DELIVERY_ORDER_FINAL_STATUSES = [
     DeliveryOrderStatusType.Delivered.value,
-    DeliveryOrderStatusType.NotDeliverable.value
+    DeliveryOrderStatusType.NotDeliverable.value,
+    DeliveryOrderStatusType.Exchanged.value,
+    DeliveryOrderStatusType.NotExchangable.value
 ] + DELIVERY_ORDER_REJECTED_STATUSES
 
 DELIVERY_ORDER_STATE_MACHINE = {
     DeliveryOrderStatusType.Planning.value: [
         DeliveryOrderStatusType.PlanningApproved.value,
         DeliveryOrderStatusType.PlanningChanged.value,
         DeliveryOrderStatusType.Planning.value,
@@ -203,25 +243,39 @@
         DeliveryOrderStatusType.DeliveryRejected.value, #entrega rechazada
     ],
     DeliveryOrderStatusType.PhysicallyReceived.value: [
         DeliveryOrderStatusType.DistributionCenterReceived.value,
         DeliveryOrderStatusType.DeliveryRejected.value, #entrega rechazada
     ],
     DeliveryOrderStatusType.DistributionCenterReceived.value: [
+        DeliveryOrderStatusType.DeliveryCourierPreAssigned.value,
         DeliveryOrderStatusType.SERTravelling.value,
         DeliveryOrderStatusType.DeliveryRejected.value, #entrega rechazada
         DeliveryOrderStatusType.PhysicallyReceived.value,
     ],
+    DeliveryOrderStatusType.DeliveryCourierPreAssigned.value: [
+        DeliveryOrderStatusType.DeliveryCourierAssigned.value,
+    ],
+    DeliveryOrderStatusType.DeliveryCourierAssigned.value: [
+        DeliveryOrderStatusType.SERTravelling.value,
+        DeliveryOrderStatusType.DeliveryCourierReceived.value,
+    ],
     DeliveryOrderStatusType.SERTravelling.value: [
         DeliveryOrderStatusType.SERReceived.value,
         DeliveryOrderStatusType.PhysicallyReceived.value,
     ],
     DeliveryOrderStatusType.SERReceived.value: [
         DeliveryOrderStatusType.DeliveryCourierReceived.value,
-        DeliveryOrderStatusType.PhysicallyReceived.value,
+        DeliveryOrderStatusType.PhysicallyReceived.value
+    ],
+    DeliveryOrderStatusType.PickupSERReceived.value: [
+        DeliveryOrderStatusType.DistributionCenterTravelling.value
+    ],
+    DeliveryOrderStatusType.DistributionCenterTravelling.value: [
+        DeliveryOrderStatusType.DistributionCenterReceived.value
     ],
     DeliveryOrderStatusType.DeliveryCourierReceived.value: [
         DeliveryOrderStatusType.DeliveryScheduled.value,
         DeliveryOrderStatusType.DeliveryRejected.value, #entrega rechazada
         DeliveryOrderStatusType.PhysicallyReceived.value,
         DeliveryOrderStatusType.DistributionCenterReceived.value,
         DeliveryOrderStatusType.SERReceived.value
@@ -260,31 +314,46 @@
         DeliveryOrderStatusType.SERReceived.value
     ],
     DeliveryOrderStatusType.Delivered.value: [
         DeliveryOrderStatusType.Recovered.value,
         DeliveryOrderStatusType.B2CEvaluated.value
     ],
     DeliveryOrderStatusType.B2CReceptionRejected.value: [ # rechazado cliente
+        DeliveryOrderStatusType.Quarantine.value,
+        DeliveryOrderStatusType.Recovered.value,
+    ],
+    DeliveryOrderStatusType.Quarantine.value: [
+        DeliveryOrderStatusType.PickupSERReceived.value,
         DeliveryOrderStatusType.Recovered.value
     ],
+    DeliveryOrderStatusType.PickupSERReceived.value: [
+        DeliveryOrderStatusType.DistributionCenterTravelling.value
+    ],
+    DeliveryOrderStatusType.DistributionCenterTravelling.value: [
+        DeliveryOrderStatusType.PickupDistributionCenterReceived.value
+    ],
     DeliveryOrderStatusType.ALASRejected.value: [ # rechazado alas
         DeliveryOrderStatusType.Recovered.value
     ],
     DeliveryOrderStatusType.Steal.value: [ # robada
         DeliveryOrderStatusType.Recovered.value
     ],
     DeliveryOrderStatusType.Missing.value: [ # extraviada
         DeliveryOrderStatusType.Recovered.value
     ],
     DeliveryOrderStatusType.B2CRejected.value: [ # rechazada en terreno
         DeliveryOrderStatusType.Recovered.value
     ],
-    DeliveryOrderStatusType.NotDeliverable.value: [
+    DeliveryOrderStatusType.WrongCrossDocking.value: [ # error de base
         DeliveryOrderStatusType.Recovered.value
     ],
+    DeliveryOrderStatusType.NotDeliverable.value: [
+        DeliveryOrderStatusType.Quarantine.value,
+        DeliveryOrderStatusType.Recovered.value,
+    ],
     DeliveryOrderStatusType.Recovered.value: [
         DeliveryOrderStatusType.DistributionCenterReceived.value,
         DeliveryOrderStatusType.SERReceived.value,
         DeliveryOrderStatusType.VirtuallyReceived.value,
         DeliveryOrderStatusType.Planning.value,
         DeliveryOrderStatusType.PhysicallyReceived.value
     ],
@@ -295,22 +364,22 @@
 
 PICKUP_ORDER_STATE_MACHINE = {
     DeliveryOrderStatusType.Planning.value: [
         DeliveryOrderStatusType.PlanningApproved.value,
         DeliveryOrderStatusType.Planning.value
     ],
     DeliveryOrderStatusType.PlanningApproved.value: [
-        DeliveryOrderStatusType.VirtuallyReceived.value,
+        DeliveryOrderStatusType.VirtuallyReceived.value
     ],
     DeliveryOrderStatusType.VirtuallyReceived.value: [
-        DeliveryOrderStatusType.DeliveryCourierReceived.value #Recibido Mensajero
+        DeliveryOrderStatusType.DeliveryCourierReceived.value
     ],
     DeliveryOrderStatusType.DeliveryCourierReceived.value: [
-        DeliveryOrderStatusType.Withdrawn.value, # Retirada
-        DeliveryOrderStatusType.NotWithdrawn.value # No Retirada 
+        DeliveryOrderStatusType.Withdrawn.value,
+        DeliveryOrderStatusType.NotWithdrawn.value
     ],
     DeliveryOrderStatusType.NotWithdrawn.value: [
         DeliveryOrderStatusType.DeliveryCourierReceived.value,
         DeliveryOrderStatusType.Nonwithdrable.value
     ],
     DeliveryOrderStatusType.Withdrawn.value: [
         DeliveryOrderStatusType.SERReceived.value
@@ -324,52 +393,253 @@
     DeliveryOrderStatusType.DistributionCenterReceived.value: [
         DeliveryOrderStatusType.B2BTraveling.value
     ],
     DeliveryOrderStatusType.B2BTraveling.value: [
         DeliveryOrderStatusType.B2BDelivered.value
     ],
     DeliveryOrderStatusType.B2BDelivered.value: [
-        
+
     ],
-    DeliveryOrderStatusType.B2CReceptionRejected.value: [ # rechazado cliente
+    DeliveryOrderStatusType.B2CReceptionRejected.value: [
         DeliveryOrderStatusType.Recovered.value
     ],
-    DeliveryOrderStatusType.ALASRejected.value: [ # rechazado alas
+    DeliveryOrderStatusType.ALASRejected.value: [
         DeliveryOrderStatusType.Recovered.value
     ],
-    DeliveryOrderStatusType.Steal.value: [ # robada
+    DeliveryOrderStatusType.Steal.value: [
         DeliveryOrderStatusType.Recovered.value
     ],
-    DeliveryOrderStatusType.Missing.value: [ # extraviada
+    DeliveryOrderStatusType.Missing.value: [
         DeliveryOrderStatusType.Recovered.value
     ],
     DeliveryOrderStatusType.Nonwithdrable.value: [
         DeliveryOrderStatusType.Recovered.value
     ],
     DeliveryOrderStatusType.Recovered.value: [
         DeliveryOrderStatusType.DistributionCenterReceived.value
     ],
-    DeliveryOrderStatusType.B2BReceptionRejected.value: [ #rechazado b2b
+    DeliveryOrderStatusType.B2BReceptionRejected.value: [
+        DeliveryOrderStatusType.Recovered.value
+    ]
+}
+
+PICKUP_ORDER_STATE_MACHINE_NEW = {
+    DeliveryOrderStatusType.Planning.value: [
+        DeliveryOrderStatusType.PlanningApproved.value,
+        DeliveryOrderStatusType.Planning.value
+    ],
+    DeliveryOrderStatusType.PlanningApproved.value: [
+        DeliveryOrderStatusType.VirtuallyReceived.value
+    ],
+    DeliveryOrderStatusType.VirtuallyReceived.value: [
+        DeliveryOrderStatusType.DeliveryCourierReceived.value
+    ],
+    DeliveryOrderStatusType.DeliveryCourierReceived.value: [
+        DeliveryOrderStatusType.Withdrawn.value,
+        DeliveryOrderStatusType.NotWithdrawn.value
+    ],
+    DeliveryOrderStatusType.NotWithdrawn.value: [
+        DeliveryOrderStatusType.DeliveryCourierReceived.value,
+        DeliveryOrderStatusType.Nonwithdrable.value
+    ],
+    DeliveryOrderStatusType.Withdrawn.value: [
+        DeliveryOrderStatusType.PickupSERReceived.value
+    ],
+    DeliveryOrderStatusType.PickupSERReceived.value: [
+        DeliveryOrderStatusType.DistributionCenterTravelling.value
+    ],
+    DeliveryOrderStatusType.DistributionCenterTravelling.value: [
+        DeliveryOrderStatusType.PickupDistributionCenterReceived.value
+    ],
+    DeliveryOrderStatusType.PickupDistributionCenterReceived.value: [
+        DeliveryOrderStatusType.B2BTraveling.value
+    ],
+    DeliveryOrderStatusType.B2BTraveling.value: [
+        DeliveryOrderStatusType.B2BDelivered.value
+    ],
+    # Rejected States
+    DeliveryOrderStatusType.B2CReceptionRejected.value: [
+        DeliveryOrderStatusType.Quarantine.value,
+        DeliveryOrderStatusType.Recovered.value
+    ],
+    DeliveryOrderStatusType.NotDeliverable.value: [
+        DeliveryOrderStatusType.Quarantine.value,
+        DeliveryOrderStatusType.Recovered.value,
+    ],
+    DeliveryOrderStatusType.Quarantine.value: [
+        DeliveryOrderStatusType.PickupSERReceived.value,
+        DeliveryOrderStatusType.Recovered.value
+    ],
+    DeliveryOrderStatusType.WrongCrossDocking.value: [
+        DeliveryOrderStatusType.PickupSERReceived.value
+    ],
+    DeliveryOrderStatusType.ALASRejected.value: [
+        DeliveryOrderStatusType.Recovered.value
+    ],
+    DeliveryOrderStatusType.Steal.value: [
+        DeliveryOrderStatusType.Recovered.value
+    ],
+    DeliveryOrderStatusType.Missing.value: [
+        DeliveryOrderStatusType.Recovered.value
+    ],
+    DeliveryOrderStatusType.Nonwithdrable.value: [
+        DeliveryOrderStatusType.Recovered.value
+    ],
+    DeliveryOrderStatusType.Recovered.value: [
+        DeliveryOrderStatusType.PickupDistributionCenterReceived.value
+    ],
+    DeliveryOrderStatusType.B2BReceptionRejected.value: [
         DeliveryOrderStatusType.Recovered.value
     ]
 }
 
+EXCHANGE_ORDER_STATE_MACHINE = {
+    DeliveryOrderStatusType.Planning.value: [
+        DeliveryOrderStatusType.PlanningApproved.value,
+        DeliveryOrderStatusType.Planning.value,
+    ],
+    DeliveryOrderStatusType.PlanningApproved.value: [
+        DeliveryOrderStatusType.VirtuallyReceived.value,
+    ],
+    DeliveryOrderStatusType.VirtuallyReceived.value: [
+        DeliveryOrderStatusType.PhysicallyReceived.value,
+    ],
+    DeliveryOrderStatusType.PhysicallyReceived.value: [
+        DeliveryOrderStatusType.DistributionCenterReceived.value,
+    ],
+    DeliveryOrderStatusType.DistributionCenterReceived.value: [
+        DeliveryOrderStatusType.DeliveryCourierPreAssigned.value,
+        DeliveryOrderStatusType.SERTravelling.value,
+        DeliveryOrderStatusType.PhysicallyReceived.value,
+    ],
+    DeliveryOrderStatusType.DeliveryCourierPreAssigned.value: [
+        DeliveryOrderStatusType.DeliveryCourierAssigned.value,
+    ],
+    DeliveryOrderStatusType.DeliveryCourierAssigned.value: [
+        DeliveryOrderStatusType.SERTravelling.value,
+        DeliveryOrderStatusType.DeliveryCourierReceived.value,
+    ],
+    DeliveryOrderStatusType.SERTravelling.value: [
+        DeliveryOrderStatusType.SERReceived.value,
+        DeliveryOrderStatusType.PhysicallyReceived.value,
+    ],
+    DeliveryOrderStatusType.SERReceived.value: [
+        DeliveryOrderStatusType.DeliveryCourierReceived.value,
+        DeliveryOrderStatusType.PhysicallyReceived.value,
+        DeliveryOrderStatusType.DeliveryCourierAssigned.value,
+    ],
+    DeliveryOrderStatusType.DeliveryCourierReceived.value: [
+        DeliveryOrderStatusType.DeliveryScheduled.value,
+        DeliveryOrderStatusType.PhysicallyReceived.value,
+        DeliveryOrderStatusType.DistributionCenterReceived.value,
+        DeliveryOrderStatusType.SERReceived.value
+    ],
+    DeliveryOrderStatusType.DeliveryScheduled.value: [
+        DeliveryOrderStatusType.B2CTraveling.value,
+        DeliveryOrderStatusType.DistributionCenterReceived.value,
+        DeliveryOrderStatusType.SERReceived.value
+    ],
+    DeliveryOrderStatusType.B2CTraveling.value: [
+        DeliveryOrderStatusType.Exchanged.value,
+        DeliveryOrderStatusType.NotExchanged.value,
+        DeliveryOrderStatusType.B2BReceptionRejected.value,
+        DeliveryOrderStatusType.B2CReceptionRejected.value,
+        DeliveryOrderStatusType.ALASRejected.value,
+        DeliveryOrderStatusType.Steal.value,
+        DeliveryOrderStatusType.Missing.value,
+        DeliveryOrderStatusType.DistributionCenterReceived.value,
+        DeliveryOrderStatusType.SERReceived.value
+    ],
+    DeliveryOrderStatusType.NotExchanged.value: [
+        DeliveryOrderStatusType.DeliveryCourierReceived.value,
+        DeliveryOrderStatusType.NotExchangable.value,
+        DeliveryOrderStatusType.Recovered.value,
+        DeliveryOrderStatusType.PhysicallyReceived.value,
+        DeliveryOrderStatusType.DistributionCenterReceived.value,
+        DeliveryOrderStatusType.SERReceived.value
+    ],
+    DeliveryOrderStatusType.Exchanged.value: [
+        DeliveryOrderStatusType.PickupSERReceived.value
+    ],
+    DeliveryOrderStatusType.PickupSERReceived.value: [
+        DeliveryOrderStatusType.DistributionCenterTravelling.value
+    ],
+    DeliveryOrderStatusType.DistributionCenterTravelling.value: [
+        DeliveryOrderStatusType.PickupDistributionCenterReceived.value
+    ],
+    DeliveryOrderStatusType.PickupDistributionCenterReceived.value: [
+        DeliveryOrderStatusType.B2BTraveling.value
+    ],
+    DeliveryOrderStatusType.B2BTraveling.value: [
+        DeliveryOrderStatusType.B2BDelivered.value
+    ],
+    # Rejected States
+    DeliveryOrderStatusType.B2CReceptionRejected.value: [
+        DeliveryOrderStatusType.Quarantine.value,
+        DeliveryOrderStatusType.Recovered.value
+    ],
+    DeliveryOrderStatusType.ALASRejected.value: [
+        DeliveryOrderStatusType.Recovered.value
+    ],
+    DeliveryOrderStatusType.Steal.value: [
+        DeliveryOrderStatusType.Recovered.value
+    ],
+    DeliveryOrderStatusType.Missing.value: [
+        DeliveryOrderStatusType.Recovered.value
+    ],
+    DeliveryOrderStatusType.NotExchangable.value: [
+        DeliveryOrderStatusType.Quarantine.value,
+        DeliveryOrderStatusType.Recovered.value
+    ],
+    DeliveryOrderStatusType.Quarantine.value: [
+        DeliveryOrderStatusType.PickupSERReceived.value,
+        DeliveryOrderStatusType.Recovered.value
+    ],
+    DeliveryOrderStatusType.Recovered.value: [
+        DeliveryOrderStatusType.DistributionCenterReceived.value,
+        DeliveryOrderStatusType.SERReceived.value,
+        DeliveryOrderStatusType.VirtuallyReceived.value,
+        DeliveryOrderStatusType.Planning.value,
+        DeliveryOrderStatusType.PhysicallyReceived.value
+    ],
+    DeliveryOrderStatusType.B2BReceptionRejected.value: [
+        DeliveryOrderStatusType.Recovered.value
+    ]
+}
+
+
+
 class BulkStatusType(Enum):
     Started = 1
     DCReceived = 2
     ITControlled = 3
     SERTravelling = 4
     Opened = 5
-    
+
+
+class PalletStatusType(Enum):
+    Started = 1
+    PreAssigned = 2
+    Assigned = 3
+
+
 class BulkOperationStatusType(Enum):
     Created = 1
     Packaged = 2
     Controlled = 3
     Travelling = 4
     Received = 5
+
+
+class PalletOperationStatusType(Enum):
+    Created = 1
+    Packaged = 2
+    Controlled = 3
+    Travelling = 4
+    Received = 5
     
 class PackageSerReceiveStatusType(Enum):
     Pending = 1
     Accepted = 2
     Damaged = 3
     
 def get_delivery_rejected_reason_dic():  
@@ -392,183 +662,262 @@
         return event_info['schedule_rejected_1_comments']
     if 'schedule_rejected_2_comments' in event_info and event_info['schedule_rejected_2_comments']:
         return event_info['schedule_rejected_2_comments']
     if 'schedule_rejected_3_comments' in event_info and event_info['schedule_rejected_3_comments']:
         return event_info['schedule_rejected_3_comments']
     return None
 
-def get_status_info(delivery_order):
+def get_status_info_wom(delivery_order):
+    events_info, status, last_event_timestamp = None, None, None
+
+    if delivery_order['status'] == DeliveryOrderStatusType.PhysicallyReceived.value:
+        events_info = filter(
+            lambda x: x['status'] == delivery_order['status'],
+            delivery_order['events_info']
+        )
+        status = 'Despacho recepcionado'
+
+    elif delivery_order['status'] == DeliveryOrderStatusType.B2BReceptionRejected.value:
+        events_info = filter(
+            lambda x: x['status'] == delivery_order['status'],
+            delivery_order['events_info']
+        )
+        status = 'Orden Cancelada por Logística'
+
+
+    elif delivery_order['status'] in [DeliveryOrderStatusType.B2CTraveling.value,
+                                      DeliveryOrderStatusType.DeliveryCourierReceived.value]:
+        events_info = filter(
+            lambda x: x['status'] == delivery_order['status'],
+            delivery_order['events_info']
+        )
+        status = 'Despacho en ruta'
+
+    elif delivery_order['status'] in [DeliveryOrderStatusType.NotDelivered.value, DeliveryOrderStatusType.NotDeliverable.value, DeliveryOrderStatusType.NotExchanged.value, DeliveryOrderStatusType.NotExchangable.value]:
+        events_info = filter(
+            lambda x: x['status'] == delivery_order['status'],
+            delivery_order['events_info']
+        )
+        status = "Intento {}".format( str(delivery_order['delivery_attemps']) )
+
+    elif delivery_order['status'] in [DeliveryOrderStatusType.Delivered.value, DeliveryOrderStatusType.Exchanged.value]:
+        events_info = filter(
+            lambda x: x['status'] == delivery_order['status'],
+            delivery_order['events_info']
+        )
+        status = 'Entregado'
+
+    #elif delivery_order['status'] == DeliveryOrderStatusType.NotDeliverable.value:
+    #    events_info = filter(
+    #        lambda x: x['status'] == delivery_order['status'],
+    #        delivery_order['events_info']
+    #    )
+    #    status = 'Orden Cancelada'
+
+    elif delivery_order['status'] == DeliveryOrderStatusType.B2CReceptionRejected.value:
+        events_info = filter(
+            lambda x: x['status'] == delivery_order['status'],
+            delivery_order['events_info']
+        )
+        status = 'Cliente desiste'
+
+    elif delivery_order['status'] == DeliveryOrderStatusType.ALASRejected.value:
+        events_info = filter(
+            lambda x: x['status'] == delivery_order['status'],
+            delivery_order['events_info']
+        )
+        status = 'No Entregado'
+
+    elif delivery_order['status'] in [DeliveryOrderStatusType.Steal.value, DeliveryOrderStatusType.Missing.value]:
+        events_info = filter(
+            lambda x: x['status'] == delivery_order['status'],
+            delivery_order['events_info']
+        )
+        status = 'Mermada'
+
+    else:
+        events_info = filter(
+            lambda x: x['status'] == delivery_order['status'],
+            delivery_order['events_info']
+        )
+
+        status_dic = get_delivery_order_status_dic()
+        status = status_dic[delivery_order['status']]
+
+    if events_info:
+        last_event_timestamp = events_info[len(events_info) - 1]['timestamp'].split('.')[0]
+
+    return status, last_event_timestamp
+
+def get_status_info(delivery_order, r_reason = False):
     events_info, status, description, last_event_timestamp = None, None, None, None
 
     if delivery_order['status'] == DeliveryOrderStatusType.Planning.value:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
+        description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.VirtuallyReceived.value:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status = 'Planificación'
 
         description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
+        description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.PhysicallyReceived.value:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status = 'Recepción Física'
 
         description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
+        description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.B2BReceptionRejected.value:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status = 'Rechazada B2B'
 
         description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
+        description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.DistributionCenterReceived.value:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
+        description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.SERTravelling.value:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status = 'Viajando SER'
 
         description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
+        description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.SERReceived.value:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
-
-    elif delivery_order['status'] == DeliveryOrderStatusType.DeliveryCourierReceived.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
-        status_dic = get_delivery_order_status_dic()
-        status = status_dic[delivery_order['status']]
-
-        description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
+        description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.DeliveryConfirmed.value:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status = 'Entrega Agendada'
 
         description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
+        description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.DeliveryNotConfirmed.value:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status = 'Entrega Agendada'
 
         description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
+        description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.DeliveryScheduled.value:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
+        description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
-    elif delivery_order['status'] == DeliveryOrderStatusType.B2CTraveling.value:
+    elif delivery_order['status'] in [DeliveryOrderStatusType.B2CTraveling.value, DeliveryOrderStatusType.DeliveryCourierReceived.value]:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status = 'En Ruta'
 
         description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
+        description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
-    elif delivery_order['status'] == DeliveryOrderStatusType.NotDelivered.value:
+    elif delivery_order['status'] in [DeliveryOrderStatusType.NotDelivered.value, DeliveryOrderStatusType.NotExchanged.value]:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
+        description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
-    elif DeliveryOrderStatusType.Delivered.value == DeliveryOrderStatusType.Delivered.value:
+    elif delivery_order['status'] == DeliveryOrderStatusType.Delivered.value:
         events_info = filter(
-            lambda x: x['status'] == DeliveryOrderStatusType.Delivered.value,
+            lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status = 'Entregado'
         description = 'Entrega realizada'
 
+    elif delivery_order['status'] == DeliveryOrderStatusType.Exchanged.value:
+        events_info = filter(
+            lambda x: x['status'] == delivery_order['status'],
+            delivery_order['events_info']
+        )
+        status = 'Intercambiada'
+        description = 'Intercambio realizada'
+
     elif delivery_order['status'] in DELIVERY_ORDER_REJECTED_STATUSES:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description = get_rejected_reason(events_info[len(events_info) - 1]['info'])
         if description is None:
             description = "Entrega Rechazada"
 
-    elif delivery_order['status'] == DeliveryOrderStatusType.NotDeliverable.value:
+    elif delivery_order['status'] in [DeliveryOrderStatusType.NotDeliverable.value, DeliveryOrderStatusType.NotExchangable.value]:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description_dic = get_delivery_order_status_description_dic()
-        description = description_dic[delivery_order['status']]
+        description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
     else:
         events_info = filter(
             lambda x: x['status'] == delivery_order['status'],
             delivery_order['events_info']
         )
 
         status_dic = get_delivery_order_status_dic()
@@ -579,51 +928,70 @@
             if delivery_order['status'] in description_dic \
                 else status
 
 
     if events_info:
         last_event_timestamp = events_info[len(events_info) - 1]['timestamp'].split('.')[0]
 
+    reason = None
+    if r_reason:
+        for key in events_info[-1]['info'].keys():
+            if 'reason' in key:
+                reason = events_info[-1]['info'][key]
+        if reason is not None:
+            reason_dic = get_delivery_order_rejected_dic()
+            reason = reason_dic[reason]
+
+        return status, description, last_event_timestamp, reason
+
     return status, description, last_event_timestamp
 
 def get_macro_status(delivery_order):
     in_route_amount = len(filter(lambda x: x == 17, delivery_order['statuses']))
+    in_quarantine_amount = len(filter(lambda x: x == 52, delivery_order['statuses']))
     status = get_delivery_order_status_dic()
 
     if delivery_order['status'] in [
-        DeliveryOrderStatusType.VirtuallyReceived.value,
-        DeliveryOrderStatusType.PhysicallyReceived.value,
-        DeliveryOrderStatusType.B2BReceptionRejected.value,
-        DeliveryOrderStatusType.Delivered.value] or delivery_order['status'] >= DeliveryOrderStatusType.ALASRejected.value:
-        return status[delivery_order['status']]
-    elif delivery_order['status'] in [
         DeliveryOrderStatusType.DeliveryRejected.value,
         DeliveryOrderStatusType.B2CRejected.value,
         DeliveryOrderStatusType.B2CReceptionRejected.value]:
         return 'Rechazado Cliente'
+
+    elif delivery_order['status'] == DeliveryOrderStatusType.Quarantine.value or (
+            delivery_order['status'] != DeliveryOrderStatusType.Quarantine.value and in_quarantine_amount > 0 and
+            delivery_order['lob'] == 1 and
+            delivery_order['lob'] != delivery_order['branch']
+    ):
+
+        statuses = delivery_order['statuses'][:]
+        statuses.reverse()
+        index = len(statuses) - statuses.index(52) - 1
+
+        value = delivery_order['statuses'][:index][-1]
+        return status[value]
+
     elif delivery_order['status'] == DeliveryOrderStatusType.B2CTraveling.value:
         return 'En Ruta {0}'.format(in_route_amount)
-    elif delivery_order['status'] == DeliveryOrderStatusType.NotDeliverable.value:
+
+    elif delivery_order['status'] in [DeliveryOrderStatusType.NotDeliverable.value, DeliveryOrderStatusType.NotWithdrawn.value, DeliveryOrderStatusType.NotExchangable.value]:
         return 'Rechazado 3 Intentos'
-    else:
-        if in_route_amount > 0:
-            return 'Pendiente Ruta {0}'.format(in_route_amount + 1)
-    return 'En Planta'
+
+    return status[delivery_order['status']]
 
 def get_b2c_delivery_events(delivery_order):
     return filter(
         lambda x: (x['status'] == 15 and 'b2c_delivery_actual' in x['info']) or
                     x['status'] == 18 or
                     x['status'] == 19 or
                     x['status'] in DELIVERY_ORDER_REJECTED_STATUSES,
         delivery_order['events_info']
     )
     
 def get_not_delivered_reason(event_info):
-    reasons = ['No hay quien reciba', 'Dirección Incompleta', 'Problema Documentación', 'Siniestro', 'Merma']
+    reasons = ['No hay quien reciba', 'Dirección Incompleta', 'Problema Documentación', 'Código Erróneo', 'Paso Automatico', 'Siniestro', 'Merma']
 
     if 'not_delivered_3_reason' in event_info and event_info['not_delivered_3_reason']:
         return reasons[event_info['not_delivered_3_reason'] - 1]
     if 'not_delivered_2_reason' in event_info and event_info['not_delivered_2_reason']:
         return reasons[event_info['not_delivered_2_reason'] - 1]
     if 'not_delivered_1_reason' in event_info and event_info['not_delivered_1_reason']:
         return reasons[event_info['not_delivered_1_reason'] - 1]
@@ -711,23 +1079,25 @@
 
     def change_status(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_change-status".format(id), params)
 
     def change_planning(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_change-planning".format(id), params)
 
-    def upload_file(self, user_name, sender_code, base64_content, file_format="txt", file_name=None, lob=1):
+    def upload_file(self, user_name, sender_code, base64_content, file_format="txt", file_name=None, lob=1, target_name=None):
         params = {
             'user_name': user_name,
             'sender_code': sender_code,
             'base64_content': base64_content,
             'format': file_format,
             'file_name': file_name,
             'lob': lob
         }
+        if target_name is not None:
+            params.update({'target_name': target_name})
         return self.http_post_json(self.entity_endpoint_base_url + "_upload-file", params)
 
     def validate_customer(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_validate-customer".format(id), params)
 
     def confirm_b2c_delivery(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_confirm-b2c-delivery".format(id), params)
@@ -746,17 +1116,26 @@
 
     def send_notification(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_send-notification".format(id), params)
 
     def change_b2c_delivery(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_change-b2c-delivery".format(id), params)
 
+    def change_b2b_delivery(self, id, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "{0}/_change-b2b-delivery".format(id), params)
+
     def masive_change_b2c_delivery(self, params):
         return self.http_post_json(self.entity_endpoint_base_url + "_masive_change-b2c-delivery", params)
 
+    def massive_change_b2c_delivery(self, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "_massive_change-b2c-delivery", params)
+
+    def polygons_list(self, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "_polygons-list", params)
+
     def change_destination(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_change-destination".format(id), params)
 
     def set_b2c_informed_geo_location(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_set-b2c-informed-geo-location".format(id), params)
 
     def route_now(self, id, params):
@@ -787,29 +1166,53 @@
 
     def validate_package(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_validate-package".format(id), params)
     
     def assign_package(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_assign-package".format(id), params)
 
+    def assign_simserial_package(self, id, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "{0}/_assign-simserial-package".format(id), params)
+
+    def assign_simserial_packages(self, id, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "{0}/_assign-simserial-packages".format(id), params)
+
     def process_create_labels_by_ids(self, params):
         return self.http_post_json(self.entity_endpoint_base_url + "_process-create-labels-by-ids", params)
     
     def process_create_generic_labels(self, params):
         return self.http_post_json(self.entity_endpoint_base_url + "_process-create-generic-labels", params)
 
     def create_label_sync(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_create-label-sync".format(id), params)
 
+    def create_label_zpl(self, id, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "{0}/_create-label-zpl".format(id), params)
+
+    def get_b2b_reception_expected(self, id, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "{0}/_get-b2b-reception-expected".format(id), params)
+
     def process_physical_reception(self, params):
         return self.http_post_json(self.entity_endpoint_base_url + "_process-physical-reception", params)
+
+    def process_b2b_receive_reception(self, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "_process-b2b-receive-reception", params)
     
     def slack_report_send(self, params):
         return self.http_post_json(self.entity_endpoint_base_url + "_slack-report-send", params)
 
+    def in_postgresql(self, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "_in-postgresql", params)
+
+    def set_packed_items(self, id, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "{0}/_set-packed_items".format(id), params)
+
+    def modify_package_quantity(self, id, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "{0}/_modify-package-quantity".format(id), params)
+
     def physically_receive(self, id, event_info, pasync=True):
         if pasync:
             return TaskClient(**self.args).enqueue('delivery-order-physically-receive', {
                 'delivery_order_id': id,
                 'event_info': event_info
             })
         else:
@@ -823,14 +1226,17 @@
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_ser-travelling-receive".format(id), event_info)
 
     def ser_received_receive(self, id, event_info, pasync=True):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_ser-received-receive".format(id), event_info)
 
     def delivery_courier_receive(self, id, event_info, pasync=True):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_delivery-courier-receive".format(id), event_info)
+
+    def delivery_courier_assigned(self, id, event_info, pasync=True):
+        return self.http_post_json(self.entity_endpoint_base_url + "{0}/_delivery-courier-assigned".format(id), event_info)
     
     def b2b_travelling(self, id, event_info):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_b2b-travelling".format(id), event_info)
     
     def b2b_receive(self, id, event_info):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_b2b-receive".format(id), event_info)
     # endregion
@@ -843,17 +1249,28 @@
 
     def recover(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_recover".format(id), params)
 
     def submit_form(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_submit-form".format(id), params)
 
+    def info_next_status(self, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "_info-next-status", params)
+
+    def next_status(self, id, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "{0}/_next-status".format(id), params)
+
+    def prev_status(self, id, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "{0}/_prev-status".format(id), params)
+
     def update_documents(self, id, params):
         return self.http_post_json(self.entity_endpoint_base_url + "{0}/_update-documents".format(id), params)
 
+    def assignment_courier(self, params):
+        return self.http_post_json(self.entity_endpoint_base_url + "_assignment-courier", params)
 
 class DeliveryOrderMessagingClient(EntityClientBase):
     entity_endpoint_base_url = '/delivery/delivery-orders-messaging/'
 
 
 class DeliveryOrdersForRouteClient(EntityClientBase):
     entity_endpoint_base_url = '/delivery/delivery-orders-for-route/'
```

### Comparing `alas-ce0-client-4.0.9/alas_ce0_client.egg-info/SOURCES.txt` & `alas-ce0-client-5.0.78/alas_ce0_client.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -28,22 +28,25 @@
 alas_ce0/management/feature.py
 alas_ce0/management/geographic_coverage.py
 alas_ce0/management/geographic_coverage_active.py
 alas_ce0/management/maintenance.py
 alas_ce0/management/notification.py
 alas_ce0/management/package_template.py
 alas_ce0/management/packaging.py
+alas_ce0/management/pallet.py
+alas_ce0/management/position.py
 alas_ce0/management/product_template.py
 alas_ce0/management/resource.py
 alas_ce0/management/role.py
 alas_ce0/management/roles_group.py
 alas_ce0/management/service_level.py
 alas_ce0/management/shelf.py
 alas_ce0/management/task.py
 alas_ce0/management/user.py
+alas_ce0/management/user_app.py
 alas_ce0/management/vehicle.py
 alas_ce0/reporting/__init__.py
 alas_ce0/reporting/regional_partner_report.py
 alas_ce0/reporting/report.py
 alas_ce0/reporting/report_manager.py
 alas_ce0/scheduling/__init__.py
 alas_ce0/scheduling/route.py
```

### Comparing `alas-ce0-client-4.0.9/setup.py` & `alas-ce0-client-5.0.78/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
-API_CLIENT_VERSION = '4.0.9'
+API_CLIENT_VERSION = '5.0.78'
 
 setup(
     name='alas-ce0-client',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
@@ -53,16 +53,16 @@
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: MIT License',
 
         # Specify the Python versions you support here. In particular, ensure
-        # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 2.7',
+        # that you indicate whether you support Python 3 or both.
+        'Programming Language :: Python :: 3.10',
     ],
 
     # What does your project relate to?
     keywords='alas-ce0 api client development',
 
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
@@ -72,16 +72,15 @@
     # this:
     #   py_modules=["my_module"],
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['enum34', 'httplib2'],
-    # install_requires=['enum34', 'httplib2', 'requests-toolbelt'],
+    install_requires=['httplib2'],\
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={
         'dev': ['check-manifest'],
```


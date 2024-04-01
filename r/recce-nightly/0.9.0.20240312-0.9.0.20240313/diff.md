# Comparing `tmp/recce-nightly-0.9.0.20240312.tar.gz` & `tmp/recce-nightly-0.9.0.20240313.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recce-nightly-0.9.0.20240312.tar", last modified: Tue Mar 12 18:06:23 2024, max compression
+gzip compressed data, was "recce-nightly-0.9.0.20240313.tar", last modified: Wed Mar 13 18:05:52 2024, max compression
```

## Comparing `recce-nightly-0.9.0.20240312.tar` & `recce-nightly-0.9.0.20240313.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.342224 recce-nightly-0.9.0.20240312/
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-03-12 18:06:23.342224 recce-nightly-0.9.0.20240312/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.330225 recce-nightly-0.9.0.20240312/recce/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-12 18:05:25.000000 recce-nightly-0.9.0.20240312/recce/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.330225 recce-nightly-0.9.0.20240312/recce/apis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/apis/check_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/apis/check_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/apis/run_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/apis/run_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.330225 recce-nightly-0.9.0.20240312/recce/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.326225 recce-nightly-0.9.0.20240312/recce/data/_next/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.326225 recce-nightly-0.9.0.20240312/recce/data/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.330225 recce-nightly-0.9.0.20240312/recce/data/_next/static/OSDAXs6UrZSM40dV34eY3/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/OSDAXs6UrZSM40dV34eY3/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/OSDAXs6UrZSM40dV34eY3/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.334225 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/030e0bea-59754f62ad2a287c.js
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/2d02f0f7-ed3b4e4daa7c5d22.js
--rw-r--r--   0 runner    (1001) docker     (127)  1128329 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/354-d94f5f7615bdde2d.js
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/49348413-7aacf235ca16afb9.js
--rw-r--r--   0 runner    (1001) docker     (127)    97409 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/4b89641d-a80e6024cd2468dc.js
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/526a6206-7ccbd30e159c1652.js
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/5e9a126f-da62af62011c0643.js
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/607285b2-dadd48144d45dbcf.js
--rw-r--r--   0 runner    (1001) docker     (127)   119202 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/62-fe89bcbd7de7edb6.js
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/6af6e714-6003aba9c53d2dcd.js
--rw-r--r--   0 runner    (1001) docker     (127)    88650 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/6dc81886-a3fa8efdc3652e8f.js
--rw-r--r--   0 runner    (1001) docker     (127)   159459 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/7c9ab469-732af37965d79ccf.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.334225 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/app/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/app/_not-found-51ab6491960b0490.js
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/app/layout-c159ba5715e8f184.js
--rw-r--r--   0 runner    (1001) docker     (127)   108374 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/app/page-11d757976ef71345.js
--rw-r--r--   0 runner    (1001) docker     (127)   213332 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/c132bf7d-fca1bc3c8aa231eb.js
--rw-r--r--   0 runner    (1001) docker     (127)   171779 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/f0cfc0e7-bb82a3d2a10fc463.js
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/f6be744d-5973a409ea097354.js
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/f78b7092-bf8a8853eef36a4c.js
--rw-r--r--   0 runner    (1001) docker     (127)    89940 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/fb2d5402-0ccc92fc728c2993.js
--rw-r--r--   0 runner    (1001) docker     (127)   140587 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/framework-f780fd9bae3b8c58.js
--rw-r--r--   0 runner    (1001) docker     (127)   116522 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/main-01494d5774218692.js
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/main-app-3297e27de57b3a96.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.338225 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/pages/_app-97b950e56cb06d37.js
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/pages/_error-53b6bd498e76608f.js
--rw-r--r--   0 runner    (1001) docker     (127)    91460 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/webpack-2d4823656eaa7d1c.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.338225 recce-nightly-0.9.0.20240312/recce/data/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/_next/static/css/6d0611c21a82d0bb.css
--rw-r--r--   0 runner    (1001) docker     (127)    25931 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    32593 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-12 18:06:12.000000 recce-nightly-0.9.0.20240312/recce/data/index.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/dbt.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.338225 recce-nightly-0.9.0.20240312/recce/event/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-12 18:05:25.000000 recce-nightly-0.9.0.20240312/recce/event/CONFIG
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/event/SENTRY_DNS
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/event/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/event/track.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.338225 recce-nightly-0.9.0.20240312/recce/models/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/models/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/models/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/models/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/models/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.338225 recce-nightly-0.9.0.20240312/recce/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/tasks/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/tasks/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/tasks/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/tasks/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/tasks/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/tasks/rowcount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/tasks/top_k.py
--rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/tasks/valuediff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.338225 recce-nightly-0.9.0.20240312/recce/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/util/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.338225 recce-nightly-0.9.0.20240312/recce/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/recce/yaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.338225 recce-nightly-0.9.0.20240312/recce_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-03-12 18:06:23.000000 recce-nightly-0.9.0.20240312/recce_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-03-12 18:06:23.000000 recce-nightly-0.9.0.20240312/recce_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 18:06:23.000000 recce-nightly-0.9.0.20240312/recce_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-12 18:06:23.000000 recce-nightly-0.9.0.20240312/recce_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-12 18:06:23.000000 recce-nightly-0.9.0.20240312/recce_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-12 18:06:23.000000 recce-nightly-0.9.0.20240312/recce_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 18:06:23.342224 recce-nightly-0.9.0.20240312/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-12 18:06:18.000000 recce-nightly-0.9.0.20240312/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:06:23.338225 recce-nightly-0.9.0.20240312/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-12 18:04:45.000000 recce-nightly-0.9.0.20240312/tests/test_dbt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.075754 recce-nightly-0.9.0.20240313/
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-03-13 18:05:52.075754 recce-nightly-0.9.0.20240313/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.063754 recce-nightly-0.9.0.20240313/recce/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-13 18:04:57.000000 recce-nightly-0.9.0.20240313/recce/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.063754 recce-nightly-0.9.0.20240313/recce/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/apis/check_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/apis/check_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/apis/run_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/apis/run_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.063754 recce-nightly-0.9.0.20240313/recce/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.059754 recce-nightly-0.9.0.20240313/recce/data/_next/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.063754 recce-nightly-0.9.0.20240313/recce/data/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.071754 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/030e0bea-59754f62ad2a287c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/2d02f0f7-ed3b4e4daa7c5d22.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1128329 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/354-d94f5f7615bdde2d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/49348413-7aacf235ca16afb9.js
+-rw-r--r--   0 runner    (1001) docker     (127)    97409 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/4b89641d-a80e6024cd2468dc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/526a6206-7ccbd30e159c1652.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/5e9a126f-da62af62011c0643.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/607285b2-dadd48144d45dbcf.js
+-rw-r--r--   0 runner    (1001) docker     (127)   119202 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/62-fe89bcbd7de7edb6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/6af6e714-6003aba9c53d2dcd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    88650 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/6dc81886-a3fa8efdc3652e8f.js
+-rw-r--r--   0 runner    (1001) docker     (127)   159459 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/7c9ab469-732af37965d79ccf.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.071754 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/app/_not-found-51ab6491960b0490.js
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/app/layout-c159ba5715e8f184.js
+-rw-r--r--   0 runner    (1001) docker     (127)   110506 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/app/page-2e986eecfb9156dd.js
+-rw-r--r--   0 runner    (1001) docker     (127)   213332 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/c132bf7d-fca1bc3c8aa231eb.js
+-rw-r--r--   0 runner    (1001) docker     (127)   171779 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/f0cfc0e7-bb82a3d2a10fc463.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/f6be744d-5973a409ea097354.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/f78b7092-bf8a8853eef36a4c.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89940 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/fb2d5402-0ccc92fc728c2993.js
+-rw-r--r--   0 runner    (1001) docker     (127)   140587 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/framework-f780fd9bae3b8c58.js
+-rw-r--r--   0 runner    (1001) docker     (127)   116522 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/main-01494d5774218692.js
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/main-app-3297e27de57b3a96.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.071754 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/pages/_app-97b950e56cb06d37.js
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/pages/_error-53b6bd498e76608f.js
+-rw-r--r--   0 runner    (1001) docker     (127)    91460 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/webpack-2d4823656eaa7d1c.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.071754 recce-nightly-0.9.0.20240313/recce/data/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/css/6d0611c21a82d0bb.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.071754 recce-nightly-0.9.0.20240313/recce/data/_next/static/k9hThvy5xnFYnWlSYKB0A/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/k9hThvy5xnFYnWlSYKB0A/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/_next/static/k9hThvy5xnFYnWlSYKB0A/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25931 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    32593 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-13 18:05:41.000000 recce-nightly-0.9.0.20240313/recce/data/index.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.071754 recce-nightly-0.9.0.20240313/recce/event/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-13 18:04:57.000000 recce-nightly-0.9.0.20240313/recce/event/CONFIG
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/event/SENTRY_DNS
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/event/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/event/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.071754 recce-nightly-0.9.0.20240313/recce/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/models/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/models/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.075754 recce-nightly-0.9.0.20240313/recce/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/tasks/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/tasks/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/tasks/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/tasks/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/tasks/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/tasks/rowcount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/tasks/top_k.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/tasks/valuediff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.075754 recce-nightly-0.9.0.20240313/recce/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/util/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.075754 recce-nightly-0.9.0.20240313/recce/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/recce/yaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.075754 recce-nightly-0.9.0.20240313/recce_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-03-13 18:05:52.000000 recce-nightly-0.9.0.20240313/recce_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-03-13 18:05:52.000000 recce-nightly-0.9.0.20240313/recce_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 18:05:52.000000 recce-nightly-0.9.0.20240313/recce_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-13 18:05:52.000000 recce-nightly-0.9.0.20240313/recce_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-13 18:05:52.000000 recce-nightly-0.9.0.20240313/recce_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-13 18:05:52.000000 recce-nightly-0.9.0.20240313/recce_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 18:05:52.075754 recce-nightly-0.9.0.20240313/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-13 18:05:47.000000 recce-nightly-0.9.0.20240313/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:05:52.075754 recce-nightly-0.9.0.20240313/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-13 18:04:25.000000 recce-nightly-0.9.0.20240313/tests/test_dbt.py
```

### Comparing `recce-nightly-0.9.0.20240312/LICENSE` & `recce-nightly-0.9.0.20240313/LICENSE`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/PKG-INFO` & `recce-nightly-0.9.0.20240313/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recce-nightly
-Version: 0.9.0.20240312
+Version: 0.9.0.20240313
 Summary: Environment diff tool for dbt
 Home-page: https://github.com/InfuseAI/recce
 Author: InfuseAI Dev Team
 Author-email: dev@infuseai.io
 Project-URL: Bug Tracker, https://github.com/InfuseAI/recce/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `recce-nightly-0.9.0.20240312/README.md` & `recce-nightly-0.9.0.20240313/README.md`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/__init__.py` & `recce-nightly-0.9.0.20240313/recce/__init__.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/apis/check_api.py` & `recce-nightly-0.9.0.20240313/recce/apis/check_api.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/apis/check_func.py` & `recce-nightly-0.9.0.20240313/recce/apis/check_func.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/apis/run_api.py` & `recce-nightly-0.9.0.20240313/recce/apis/run_api.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/apis/run_func.py` & `recce-nightly-0.9.0.20240313/recce/apis/run_func.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/cli.py` & `recce-nightly-0.9.0.20240313/recce/cli.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/404.html` & `recce-nightly-0.9.0.20240313/recce/data/404.html`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width, initial-scale=1"/><link rel="preload" as="script" fetchPriority="low" href="/_next/static/chunks/webpack-2d4823656eaa7d1c.js" crossorigin=""/><script src="/_next/static/chunks/f0cfc0e7-bb82a3d2a10fc463.js" async="" crossorigin=""></script><script src="/_next/static/chunks/62-fe89bcbd7de7edb6.js" async="" crossorigin=""></script><script src="/_next/static/chunks/main-app-3297e27de57b3a96.js" async="" crossorigin=""></script><title>404: This page could not be found.</title><title>recce</title><meta name="description" content="Recce: a dbt tool"/><script src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js" crossorigin="" noModule=""></script></head><body><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding:0 23px 0 0;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found.</h2></div></div></div><script src="/_next/static/chunks/webpack-2d4823656eaa7d1c.js" crossorigin="" async=""></script><script>(self.__next_f=self.__next_f||[]).push([0]);self.__next_f.push([2,null])</script><script>self.__next_f.push([1,"0:\"$L1\"\n"])</script><script>self.__next_f.push([1,"2:I[61886,[],\"\"]\n4:I[35774,[],\"\"]\n5:I[44813,[],\"\"]\n6:I[82593,[],\"\"]\n8:{\"fontFamily\":\"system-ui,\\\"Segoe UI\\\",Roboto,Helvetica,Arial,sans-serif,\\\"Apple Color Emoji\\\",\\\"Segoe UI Emoji\\\"\",\"height\":\"100vh\",\"textAlign\":\"center\",\"display\":\"flex\",\"flexDirection\":\"column\",\"alignItems\":\"center\",\"justifyContent\":\"center\"}\n9:{\"display\":\"inline-block\",\"margin\":\"0 20px 0 0\",\"padding\":\"0 23px 0 0\",\"fontSize\":24,\"fontWeight\":500,\"verticalAlign\":\"top\",\"lineHeight\":\"49px\"}\na:{\"display\":\"inline-block\"}\nb:{\"fontSize\":14,\"fontW"])</script><script>self.__next_f.push([1,"eight\":400,\"lineHeight\":\"49px\",\"margin\":0}\n"])</script><script>self.__next_f.push([1,"1:[null,[\"$\",\"$L2\",null,{\"buildId\":\"OSDAXs6UrZSM40dV34eY3\",\"assetPrefix\":\"\",\"initialCanonicalUrl\":\"/_not-found\",\"initialTree\":[\"\",{\"children\":[\"__PAGE__\",{}]},\"$undefined\",\"$undefined\",true],\"initialHead\":[false,\"$L3\"],\"globalErrorComponent\":\"$4\",\"children\":[null,[\"$\",\"html\",null,{\"lang\":\"en\",\"children\":[\"$\",\"body\",null,{\"suppressHydrationWarning\":true,\"children\":[\"$\",\"$L5\",null,{\"parallelRouterKey\":\"children\",\"segmentPath\":[\"children\"],\"loading\":\"$undefined\",\"loadingStyles\":\"$undefined\",\"loadingScripts\":\"$undefined\",\"hasLoading\":false,\"error\":\"$undefined\",\"errorStyles\":\"$undefined\",\"errorScripts\":\"$undefined\",\"template\":[\"$\",\"$L6\",null,{}],\"templateStyles\":\"$undefined\",\"templateScripts\":\"$undefined\",\"notFound\":[[\"$\",\"title\",null,{\"children\":\"404: This page could not be found.\"}],[\"$\",\"div\",null,{\"style\":{\"fontFamily\":\"system-ui,\\\"Segoe UI\\\",Roboto,Helvetica,Arial,sans-serif,\\\"Apple Color Emoji\\\",\\\"Segoe UI Emoji\\\"\",\"height\":\"100vh\",\"textAlign\":\"center\",\"display\":\"flex\",\"flexDirection\":\"column\",\"alignItems\":\"center\",\"justifyContent\":\"center\"},\"children\":[\"$\",\"div\",null,{\"children\":[[\"$\",\"style\",null,{\"dangerouslySetInnerHTML\":{\"__html\":\"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}\"}}],[\"$\",\"h1\",null,{\"className\":\"next-error-h1\",\"style\":{\"display\":\"inline-block\",\"margin\":\"0 20px 0 0\",\"padding\":\"0 23px 0 0\",\"fontSize\":24,\"fontWeight\":500,\"verticalAlign\":\"top\",\"lineHeight\":\"49px\"},\"children\":\"404\"}],[\"$\",\"div\",null,{\"style\":{\"display\":\"inline-block\"},\"children\":[\"$\",\"h2\",null,{\"style\":{\"fontSize\":14,\"fontWeight\":400,\"lineHeight\":\"49px\",\"margin\":0},\"children\":\"This page could not be found.\"}]}]]}]}]],\"notFoundStyles\":[],\"childProp\":{\"current\":[\"$L7\",[[\"$\",\"title\",null,{\"children\":\"404: This page could not be found.\"}],[\"$\",\"div\",null,{\"style\":\"$8\",\"children\":[\"$\",\"div\",null,{\"children\":[[\"$\",\"style\",null,{\"dangerouslySetInnerHTML\":{\"__html\":\"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}\"}}],[\"$\",\"h1\",null,{\"className\":\"next-error-h1\",\"style\":\"$9\",\"children\":\"404\"}],[\"$\",\"div\",null,{\"style\":\"$a\",\"children\":[\"$\",\"h2\",null,{\"style\":\"$b\",\"children\":\"This page could not be found.\"}]}]]}]}]],null],\"segment\":\"__PAGE__\"},\"styles\":null}]}]}],null]}]]\n"])</script><script>self.__next_f.push([1,"3:[[\"$\",\"meta\",\"0\",{\"name\":\"viewport\",\"content\":\"width=device-width, initial-scale=1\"}],[\"$\",\"meta\",\"1\",{\"charSet\":\"utf-8\"}],[\"$\",\"title\",\"2\",{\"children\":\"recce\"}],[\"$\",\"meta\",\"3\",{\"name\":\"description\",\"content\":\"Recce: a dbt tool\"}]]\n7:null\n"])</script><script>self.__next_f.push([1,""])</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width, initial-scale=1"/><link rel="preload" as="script" fetchPriority="low" href="/_next/static/chunks/webpack-2d4823656eaa7d1c.js" crossorigin=""/><script src="/_next/static/chunks/f0cfc0e7-bb82a3d2a10fc463.js" async="" crossorigin=""></script><script src="/_next/static/chunks/62-fe89bcbd7de7edb6.js" async="" crossorigin=""></script><script src="/_next/static/chunks/main-app-3297e27de57b3a96.js" async="" crossorigin=""></script><title>404: This page could not be found.</title><title>recce</title><meta name="description" content="Recce: a dbt tool"/><script src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js" crossorigin="" noModule=""></script></head><body><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding:0 23px 0 0;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found.</h2></div></div></div><script src="/_next/static/chunks/webpack-2d4823656eaa7d1c.js" crossorigin="" async=""></script><script>(self.__next_f=self.__next_f||[]).push([0]);self.__next_f.push([2,null])</script><script>self.__next_f.push([1,"0:\"$L1\"\n"])</script><script>self.__next_f.push([1,"2:I[61886,[],\"\"]\n4:I[35774,[],\"\"]\n5:I[44813,[],\"\"]\n6:I[82593,[],\"\"]\n8:{\"fontFamily\":\"system-ui,\\\"Segoe UI\\\",Roboto,Helvetica,Arial,sans-serif,\\\"Apple Color Emoji\\\",\\\"Segoe UI Emoji\\\"\",\"height\":\"100vh\",\"textAlign\":\"center\",\"display\":\"flex\",\"flexDirection\":\"column\",\"alignItems\":\"center\",\"justifyContent\":\"center\"}\n9:{\"display\":\"inline-block\",\"margin\":\"0 20px 0 0\",\"padding\":\"0 23px 0 0\",\"fontSize\":24,\"fontWeight\":500,\"verticalAlign\":\"top\",\"lineHeight\":\"49px\"}\na:{\"display\":\"inline-block\"}\nb:{\"fontSize\":14,\"fontW"])</script><script>self.__next_f.push([1,"eight\":400,\"lineHeight\":\"49px\",\"margin\":0}\n"])</script><script>self.__next_f.push([1,"1:[null,[\"$\",\"$L2\",null,{\"buildId\":\"k9hThvy5xnFYnWlSYKB0A\",\"assetPrefix\":\"\",\"initialCanonicalUrl\":\"/_not-found\",\"initialTree\":[\"\",{\"children\":[\"__PAGE__\",{}]},\"$undefined\",\"$undefined\",true],\"initialHead\":[false,\"$L3\"],\"globalErrorComponent\":\"$4\",\"children\":[null,[\"$\",\"html\",null,{\"lang\":\"en\",\"children\":[\"$\",\"body\",null,{\"suppressHydrationWarning\":true,\"children\":[\"$\",\"$L5\",null,{\"parallelRouterKey\":\"children\",\"segmentPath\":[\"children\"],\"loading\":\"$undefined\",\"loadingStyles\":\"$undefined\",\"loadingScripts\":\"$undefined\",\"hasLoading\":false,\"error\":\"$undefined\",\"errorStyles\":\"$undefined\",\"errorScripts\":\"$undefined\",\"template\":[\"$\",\"$L6\",null,{}],\"templateStyles\":\"$undefined\",\"templateScripts\":\"$undefined\",\"notFound\":[[\"$\",\"title\",null,{\"children\":\"404: This page could not be found.\"}],[\"$\",\"div\",null,{\"style\":{\"fontFamily\":\"system-ui,\\\"Segoe UI\\\",Roboto,Helvetica,Arial,sans-serif,\\\"Apple Color Emoji\\\",\\\"Segoe UI Emoji\\\"\",\"height\":\"100vh\",\"textAlign\":\"center\",\"display\":\"flex\",\"flexDirection\":\"column\",\"alignItems\":\"center\",\"justifyContent\":\"center\"},\"children\":[\"$\",\"div\",null,{\"children\":[[\"$\",\"style\",null,{\"dangerouslySetInnerHTML\":{\"__html\":\"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}\"}}],[\"$\",\"h1\",null,{\"className\":\"next-error-h1\",\"style\":{\"display\":\"inline-block\",\"margin\":\"0 20px 0 0\",\"padding\":\"0 23px 0 0\",\"fontSize\":24,\"fontWeight\":500,\"verticalAlign\":\"top\",\"lineHeight\":\"49px\"},\"children\":\"404\"}],[\"$\",\"div\",null,{\"style\":{\"display\":\"inline-block\"},\"children\":[\"$\",\"h2\",null,{\"style\":{\"fontSize\":14,\"fontWeight\":400,\"lineHeight\":\"49px\",\"margin\":0},\"children\":\"This page could not be found.\"}]}]]}]}]],\"notFoundStyles\":[],\"childProp\":{\"current\":[\"$L7\",[[\"$\",\"title\",null,{\"children\":\"404: This page could not be found.\"}],[\"$\",\"div\",null,{\"style\":\"$8\",\"children\":[\"$\",\"div\",null,{\"children\":[[\"$\",\"style\",null,{\"dangerouslySetInnerHTML\":{\"__html\":\"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}\"}}],[\"$\",\"h1\",null,{\"className\":\"next-error-h1\",\"style\":\"$9\",\"children\":\"404\"}],[\"$\",\"div\",null,{\"style\":\"$a\",\"children\":[\"$\",\"h2\",null,{\"style\":\"$b\",\"children\":\"This page could not be found.\"}]}]]}]}]],null],\"segment\":\"__PAGE__\"},\"styles\":null}]}]}],null]}]]\n"])</script><script>self.__next_f.push([1,"3:[[\"$\",\"meta\",\"0\",{\"name\":\"viewport\",\"content\":\"width=device-width, initial-scale=1\"}],[\"$\",\"meta\",\"1\",{\"charSet\":\"utf-8\"}],[\"$\",\"title\",\"2\",{\"children\":\"recce\"}],[\"$\",\"meta\",\"3\",{\"name\":\"description\",\"content\":\"Recce: a dbt tool\"}]]\n7:null\n"])</script><script>self.__next_f.push([1,""])</script></body></html>
```

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/030e0bea-59754f62ad2a287c.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/030e0bea-59754f62ad2a287c.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/2d02f0f7-ed3b4e4daa7c5d22.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/2d02f0f7-ed3b4e4daa7c5d22.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/354-d94f5f7615bdde2d.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/354-d94f5f7615bdde2d.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/49348413-7aacf235ca16afb9.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/49348413-7aacf235ca16afb9.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/4b89641d-a80e6024cd2468dc.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/4b89641d-a80e6024cd2468dc.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/526a6206-7ccbd30e159c1652.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/526a6206-7ccbd30e159c1652.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/5e9a126f-da62af62011c0643.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/5e9a126f-da62af62011c0643.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/607285b2-dadd48144d45dbcf.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/607285b2-dadd48144d45dbcf.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/62-fe89bcbd7de7edb6.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/62-fe89bcbd7de7edb6.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/6af6e714-6003aba9c53d2dcd.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/6af6e714-6003aba9c53d2dcd.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/6dc81886-a3fa8efdc3652e8f.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/6dc81886-a3fa8efdc3652e8f.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/7c9ab469-732af37965d79ccf.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/7c9ab469-732af37965d79ccf.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/app/_not-found-51ab6491960b0490.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/app/_not-found-51ab6491960b0490.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/app/page-11d757976ef71345.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/app/page-2e986eecfb9156dd.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,145 +1,145 @@
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
     [931], {
         99178: function(e, n, t) {
-            Promise.resolve().then(t.bind(t, 26331))
+            Promise.resolve().then(t.bind(t, 13512))
         },
-        26331: function(e, n, t) {
+        13512: function(e, n, t) {
             "use strict";
             t.r(n), t.d(n, {
                 default: function() {
                     return Home
                 }
             });
-            var i = t(757),
-                r = t(27869);
+            var r = t(757),
+                i = t(27869);
 
             function getNeighborSet(e, n) {
                 let t = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 1e3,
-                    i = new Set,
-                    r = {},
+                    r = new Set,
+                    i = {},
                     dfs = (e, t) => {
-                        if (t < 0 || void 0 !== r[e] && r[e] >= t) return;
-                        r[e] = t;
+                        if (t < 0 || void 0 !== i[e] && i[e] >= t) return;
+                        i[e] = t;
                         let l = n(e);
                         for (let e of l) dfs(e, t - 1);
-                        i.add(e)
+                        r.add(e)
                     };
                 for (let n of e) dfs(n, t);
-                return i
+                return r
             }
 
             function buildDefaultLineageGraphSets(e, n) {
                 function buildAllLineageGraph(e, n) {
                     let t = {},
-                        i = {},
+                        r = {},
                         buildNode = (e, n) => ({
                             id: e,
                             name: e,
                             data: {},
                             from: n,
                             parents: {},
                             children: {},
                             isSelected: !1
                         });
-                    for (let [n, i] of Object.entries(e.parent_map)) {
+                    for (let [n, r] of Object.entries(e.parent_map)) {
                         t[n] = buildNode(n, "base");
-                        let i = e.nodes && e.nodes[n];
-                        i && (t[n].data.base = i, t[n].name = null == i ? void 0 : i.name, t[n].resourceType = null == i ? void 0 : i.resource_type, t[n].packageName = null == i ? void 0 : i.package_name)
+                        let r = e.nodes && e.nodes[n];
+                        r && (t[n].data.base = r, t[n].name = null == r ? void 0 : r.name, t[n].resourceType = null == r ? void 0 : r.resource_type, t[n].packageName = null == r ? void 0 : r.package_name)
                     }
-                    for (let [e, i] of Object.entries(n.parent_map)) {
+                    for (let [e, r] of Object.entries(n.parent_map)) {
                         t[e] ? t[e].from = "both" : t[e] = buildNode(e, "current");
-                        let i = n.nodes && n.nodes[e];
-                        i && (t[e].data.current = n.nodes && n.nodes[e], t[e].name = null == i ? void 0 : i.name, t[e].resourceType = null == i ? void 0 : i.resource_type, t[e].packageName = null == i ? void 0 : i.package_name)
+                        let r = n.nodes && n.nodes[e];
+                        r && (t[e].data.current = n.nodes && n.nodes[e], t[e].name = null == r ? void 0 : r.name, t[e].resourceType = null == r ? void 0 : r.resource_type, t[e].packageName = null == r ? void 0 : r.package_name)
                     }
-                    for (let [n, r] of Object.entries(e.parent_map))
-                        for (let e of r) {
-                            let r = t[n],
+                    for (let [n, i] of Object.entries(e.parent_map))
+                        for (let e of i) {
+                            let i = t[n],
                                 l = t[e],
                                 o = "".concat(e, "_").concat(n);
-                            i[o] = {
+                            r[o] = {
                                 id: o,
                                 from: "base",
                                 parent: l,
-                                child: r
+                                child: i
                             };
-                            let a = i[o];
-                            r.parents[e] = a, l.children[n] = a
+                            let a = r[o];
+                            i.parents[e] = a, l.children[n] = a
                         }
-                    for (let [e, r] of Object.entries(n.parent_map))
-                        for (let n of r) {
-                            let r = t[e],
+                    for (let [e, i] of Object.entries(n.parent_map))
+                        for (let n of i) {
+                            let i = t[e],
                                 l = t[n],
                                 o = "".concat(n, "_").concat(e);
-                            i[o] ? i[o].from = "both" : i[o] = {
+                            r[o] ? r[o].from = "both" : r[o] = {
                                 id: o,
                                 from: "current",
                                 parent: l,
-                                child: r
+                                child: i
                             };
-                            let a = i[o];
-                            r.parents[n] = a, l.children[e] = a
+                            let a = r[o];
+                            i.parents[n] = a, l.children[e] = a
                         }
                     return {
-                        edges: i,
+                        edges: r,
                         nodes: t
                     }
                 }
 
                 function buildChangedOnlyLineageGraph(e, n) {
                     let t = {},
-                        i = {};
+                        r = {};
 
                     function union() {
                         for (var e = arguments.length, n = Array(e), t = 0; t < e; t++) n[t] = arguments[t];
-                        let i = new Set;
+                        let r = new Set;
                         return n.forEach(e => {
                             e.forEach(e => {
-                                i.add(e)
+                                r.add(e)
                             })
-                        }), i
+                        }), r
                     }
-                    let r = selectDownstream(e, n),
+                    let i = selectDownstream(e, n),
                         l = selectUpstream(e, n, 1),
-                        o = union(r, l);
+                        o = union(i, l);
                     return Object.entries(e.nodes).forEach(e => {
-                        let [n, i] = e;
-                        o.has(n) && (t[n] = i)
+                        let [n, r] = e;
+                        o.has(n) && (t[n] = r)
                     }), Object.entries(e.edges).forEach(e => {
                         let [n, t] = e;
-                        o.has(t.parent.id) && o.has(t.child.id) && (i[n] = t)
+                        o.has(t.parent.id) && o.has(t.child.id) && (r[n] = t)
                     }), {
                         nodes: t,
-                        edges: i
+                        edges: r
                     }
                 }
                 let {
                     nodes: t,
-                    edges: i
-                } = buildAllLineageGraph(e, n), r = [];
+                    edges: r
+                } = buildAllLineageGraph(e, n), i = [];
                 for (let [e, n] of Object.entries(t))
-                    if ("base" === n.from) n.changeStatus = "removed", r.push(n.id);
-                    else if ("current" === n.from) n.changeStatus = "added", r.push(n.id);
+                    if ("base" === n.from) n.changeStatus = "removed", i.push(n.id);
+                    else if ("current" === n.from) n.changeStatus = "added", i.push(n.id);
                 else {
                     var l, o, a, s, c, d;
                     let e = null == n ? void 0 : null === (a = n.data) || void 0 === a ? void 0 : null === (o = a.base) || void 0 === o ? void 0 : null === (l = o.checksum) || void 0 === l ? void 0 : l.checksum,
                         t = null == n ? void 0 : null === (d = n.data) || void 0 === d ? void 0 : null === (c = d.current) || void 0 === c ? void 0 : null === (s = c.checksum) || void 0 === s ? void 0 : s.checksum;
-                    e && t && e !== t && (n.changeStatus = "modified", r.push(n.id))
+                    e && t && e !== t && (n.changeStatus = "modified", i.push(n.id))
                 }
-                for (let [e, n] of Object.entries(i)) "base" === n.from ? n.changeStatus = "removed" : "current" === n.from && (n.changeStatus = "added");
+                for (let [e, n] of Object.entries(r)) "base" === n.from ? n.changeStatus = "removed" : "current" === n.from && (n.changeStatus = "added");
                 return {
                     all: {
                         nodes: t,
-                        edges: i
+                        edges: r
                     },
                     changed: buildChangedOnlyLineageGraph({
                         nodes: t,
-                        edges: i
-                    }, r),
-                    modifiedSet: r,
+                        edges: r
+                    }, i),
+                    modifiedSet: i,
                     catalogExistence: {
                         base: !!e.catalog_metadata,
                         current: !!n.catalog_metadata
                     }
                 }
             }
 
@@ -151,56 +151,56 @@
             function selectDownstream(e, n) {
                 let t = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 1e3;
                 return getNeighborSet(n, n => void 0 === e.nodes[n] ? [] : Object.keys(e.nodes[n].children), t)
             }
 
             function toReactflow(e, n) {
                 let t = [],
-                    i = [];
-                for (let [n, i] of Object.entries(e.nodes)) t.push({
-                    id: i.id,
+                    r = [];
+                for (let [n, r] of Object.entries(e.nodes)) t.push({
+                    id: r.id,
                     position: {
                         x: 0,
                         y: 0
                     },
-                    data: i,
+                    data: r,
                     type: "customNode",
-                    targetPosition: r.Ly.Left,
-                    sourcePosition: r.Ly.Right
+                    targetPosition: i.Ly.Left,
+                    sourcePosition: i.Ly.Right
                 });
-                for (let [n, t] of Object.entries(e.edges)) i.push({
+                for (let [n, t] of Object.entries(e.edges)) r.push({
                     id: t.id,
                     type: "customEdge",
                     source: t.parent.id,
                     target: t.child.id,
                     data: t
                 });
-                return highlightPath(e, n, t, i, null)
+                return highlightPath(e, n, t, r, null)
             }
 
-            function highlightPath(e, n, t, i, r) {
+            function highlightPath(e, n, t, r, i) {
                 function union() {
                     for (var e = arguments.length, n = Array(e), t = 0; t < e; t++) n[t] = arguments[t];
-                    let i = new Set;
+                    let r = new Set;
                     return n.forEach(e => {
                         e.forEach(e => {
-                            i.add(e)
+                            r.add(e)
                         })
-                    }), i
+                    }), r
                 }
-                let l = null !== r ? union(selectUpstream(e, [r]), selectDownstream(e, [r])) : getNeighborSet(n, n => void 0 === e.nodes[n] ? [] : Object.keys(e.nodes[n].children)),
-                    o = new Set(i.filter(e => l.has(e.source) && l.has(e.target)).map(e => e.id)),
+                let l = null !== i ? union(selectUpstream(e, [i]), selectDownstream(e, [i])) : getNeighborSet(n, n => void 0 === e.nodes[n] ? [] : Object.keys(e.nodes[n].children)),
+                    o = new Set(r.filter(e => l.has(e.source) && l.has(e.target)).map(e => e.id)),
                     a = t.map(e => ({
                         ...e,
                         data: {
                             ...e.data,
                             isHighlighted: l.has(e.id)
                         }
                     })),
-                    s = i.map(e => ({
+                    s = r.map(e => ({
                         ...e,
                         data: {
                             ...e.data,
                             isHighlighted: o.has(e.id)
                         }
                     }));
                 return [a, s]
@@ -268,62 +268,62 @@
                 u = t(76920),
                 h = t(39668),
                 m = t(83179),
                 x = t(62648),
                 f = t(43093),
                 p = t(40312),
                 g = t(7752),
-                v = t(94410),
-                j = t(23330),
-                y = t(29985),
+                j = t(94410),
+                y = t(23330),
+                v = t(29985),
                 C = t(42524),
                 b = t(36700),
                 k = t(10287),
                 w = t(48950),
                 S = t(27726),
                 _ = t(26187),
                 R = t(23704),
                 D = t(33710),
-                T = t(93864),
-                N = t.n(T);
+                N = t(93864),
+                T = t.n(N);
             t(94570);
             var E = t(90593),
                 L = t(11180),
                 I = t(63240),
                 z = t(54057);
-            let M = L.Nbv,
-                F = L.sFB,
+            let F = L.Nbv,
+                M = L.sFB,
                 O = L.UGs,
-                IconChanged = e => (0, i.jsxs)("svg", {
+                IconChanged = e => (0, r.jsxs)("svg", {
                     stroke: "currentColor",
                     fill: "currentColor",
                     strokeWidth: "0",
                     viewBox: "0 0 16 16",
                     height: "1em",
                     width: "1em",
                     xmlns: "http://www.w3.org/2000/svg",
                     ...e,
-                    children: [(0, i.jsx)("path", {
+                    children: [(0, r.jsx)("path", {
                         fillRule: "evenodd",
                         clipRule: "evenodd",
                         d: "M8 11 a3 3 0 1 0 0-6 3 3 0 0 0 0 6z"
-                    }), (0, i.jsx)("path", {
+                    }), (0, r.jsx)("path", {
                         fillRule: "evenodd",
                         clipRule: "evenodd",
                         d: ""
                     })]
                 });
 
             function getIconForChangeStatus(e) {
                 return "added" === e ? {
                     color: "#1dce00",
-                    icon: M
+                    icon: F
                 } : "removed" === e ? {
                     color: "#ff4444",
-                    icon: F
+                    icon: M
                 } : "modified" === e ? {
                     color: "#ffa502",
                     icon: O
                 } : {
                     color: "inherit",
                     icon: void 0
                 }
@@ -365,48 +365,48 @@
             let U = W.env.NEXT_PUBLIC_API_URL ? W.env.NEXT_PUBLIC_API_URL : window.location.origin;
             var G = t(27471);
             let Q = K.default.create({
                     baseURL: U
                 }),
                 J = new G.S;
             async function submitRun(e, n, t) {
-                let i = await Q.post("/api/runs", {
+                let r = await Q.post("/api/runs", {
                         type: e,
                         params: n,
                         nowait: null == t ? void 0 : t.nowait
                     }),
-                    r = i.data;
-                return r
+                    i = r.data;
+                return i
             }
             async function waitRun(e, n) {
                 let t = await Q.get("/api/runs/".concat(e, "/wait"), {
                         params: {
                             timeout: n
                         }
                     }),
-                    i = t.data;
-                return i
+                    r = t.data;
+                return r
             }
             async function cancelRun(e) {
                 return await Q.post("/api/runs/".concat(e, "/cancel"))
             }
             async function submitRunFromCheck(e, n) {
                 let t = await Q.post("/api/checks/".concat(e, "/run"), {
                         nowait: null == n ? void 0 : n.nowait
                     }),
-                    i = t.data;
-                return i
+                    r = t.data;
+                return r
             }
             async function searchRuns(e, n, t) {
-                let i = await Q.post("/api/runs/search", {
+                let r = await Q.post("/api/runs/search", {
                     type: e,
                     params: n,
                     limit: t
                 });
-                return i.data
+                return r.data
             }
             async function submitRowCountDiff(e, n) {
                 return await submitRun("row_count_diff", e, n)
             }
             let Z = {
                     allRowCount: () => ["row_count"],
                     rowCount: e => ["row_count", e],
@@ -420,37 +420,37 @@
                     sqlQuery: X,
                     setSqlQuery: () => {}
                 });
 
             function RecceQueryContextProvider(e) {
                 let {
                     children: n
-                } = e, [t, r] = S.useState(X);
-                return (0, i.jsx)(Y.Provider, {
+                } = e, [t, i] = S.useState(X);
+                return (0, r.jsx)(Y.Provider, {
                     value: {
-                        setSqlQuery: r,
+                        setSqlQuery: i,
                         sqlQuery: t
                     },
                     children: n
                 })
             }
             let useRecceQueryContext = () => (0, S.useContext)(Y),
                 $ = (0, S.createContext)({
                     isNodesFetching: [],
                     setIsNodesFetching: () => {}
                 });
 
             function RowCountStateContextProvider(e) {
                 let {
                     children: n
-                } = e, [t, r] = S.useState([]);
-                return (0, i.jsx)($.Provider, {
+                } = e, [t, i] = S.useState([]);
+                return (0, r.jsx)($.Provider, {
                     value: {
                         isNodesFetching: t,
-                        setIsNodesFetching: r
+                        setIsNodesFetching: i
                     },
                     children: n
                 })
             }
             let useRowCountStateContext = () => (0, S.useContext)($);
             async function models_queryModelRowCount(e) {
                 let {
@@ -470,25 +470,25 @@
                 return {
                     runId: n,
                     result: t.result
                 }
             }
 
             function models_useRowCountQueries(e) {
-                let [n, t] = (0, S.useState)(!1), i = (0, H.NL)(), {
-                    setIsNodesFetching: r
-                } = useRowCountStateContext(), l = i.getQueriesData({
+                let [n, t] = (0, S.useState)(!1), r = (0, H.NL)(), {
+                    setIsNodesFetching: i
+                } = useRowCountStateContext(), l = r.getQueriesData({
                     queryKey: Z.allRowCount()
                 }).filter(n => {
-                    let [t, i] = n, [r, l] = t;
+                    let [t, r] = n, [i, l] = t;
                     return e.includes(l)
                 }).map(e => {
-                    let [n, t] = e, [i, r] = n;
+                    let [n, t] = e, [r, i] = n;
                     return {
-                        modelName: r,
+                        modelName: i,
                         data: t
                     }
                 }), o = [];
                 return e.forEach(e => {
                     let {
                         data: n
                     } = l.find(n => n.modelName === e) || {
@@ -497,140 +497,140 @@
                     };
                     void 0 === n && o.push(e)
                 }), {
                     isLoading: n,
                     fetchFn: async function() {
                         let n = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                             l = n && n.skipCache ? e : o;
-                        t(!0), r(l);
+                        t(!0), i(l);
                         let {
                             runId: a,
                             result: s
                         } = await queryRowCount(l);
                         return Object.keys(s).forEach(e => {
                             let n = s[e];
-                            i.setQueryData(Z.rowCount(e), {
+                            r.setQueryData(Z.rowCount(e), {
                                 base: n.base,
                                 curr: n.curr
                             })
-                        }), t(!1), r([]), a
+                        }), t(!1), i([]), a
                     }
                 }
             }
             var ee = t(44903),
                 en = t(62516);
 
             function RowCountByCompare(e) {
                 let {
                     rowCount: n
-                } = e, t = null === n.base ? -1 : n.base, r = null === n.curr ? -1 : n.curr, l = null === t ? "N/A" : t, o = null === r ? "N/A" : r;
-                return t === r ? (0, i.jsx)(x.U, {
-                    children: (0, i.jsxs)(f.x, {
+                } = e, t = null === n.base ? -1 : n.base, i = null === n.curr ? -1 : n.curr, l = null === t ? "N/A" : t, o = null === i ? "N/A" : i;
+                return t === i ? (0, r.jsx)(x.U, {
+                    children: (0, r.jsxs)(f.x, {
                         children: [l, " == ", o, " rows"]
                     })
-                }) : t < r ? (0, i.jsxs)(x.U, {
-                    children: [(0, i.jsx)(f.x, {
+                }) : t < i ? (0, r.jsxs)(x.U, {
+                    children: [(0, r.jsx)(f.x, {
                         children: l
-                    }), (0, i.jsx)(s.J, {
+                    }), (0, r.jsx)(s.J, {
                         as: B.QqI,
                         color: "green.500"
-                    }), (0, i.jsxs)(f.x, {
+                    }), (0, r.jsxs)(f.x, {
                         children: [o, " rows"]
                     })]
-                }) : r > t ? (0, i.jsxs)(x.U, {
-                    children: [(0, i.jsx)(f.x, {
+                }) : i > t ? (0, r.jsxs)(x.U, {
+                    children: [(0, r.jsx)(f.x, {
                         children: l
-                    }), (0, i.jsx)(s.J, {
+                    }), (0, r.jsx)(s.J, {
                         as: B.ZBs,
                         color: "red.500"
-                    }), (0, i.jsxs)(f.x, {
+                    }), (0, r.jsxs)(f.x, {
                         children: [o, " row"]
                     })]
                 }) : void 0
             }
 
             function RowCountWiteRate(e) {
                 let {
                     rowCount: n
-                } = e, t = null === n.base ? -1 : n.base, r = null === n.curr ? -1 : n.curr;
-                return t <= 0 || r <= 0 ? (0, i.jsx)(RowCountByCompare, {
+                } = e, t = null === n.base ? -1 : n.base, i = null === n.curr ? -1 : n.curr;
+                return t <= 0 || i <= 0 ? (0, r.jsx)(RowCountByCompare, {
                     rowCount: n
-                }) : t === r ? (0, i.jsxs)(x.U, {
-                    children: [(0, i.jsxs)(f.x, {
-                        children: [r, " rows"]
-                    }), (0, i.jsx)(s.J, {
+                }) : t === i ? (0, r.jsxs)(x.U, {
+                    children: [(0, r.jsxs)(f.x, {
+                        children: [i, " rows"]
+                    }), (0, r.jsx)(s.J, {
                         as: en.lxc,
                         color: "gray.500"
-                    }), (0, i.jsx)(f.x, {
+                    }), (0, r.jsx)(f.x, {
                         color: "gray.500",
                         children: "No Change"
                     })]
-                }) : t < r ? (0, i.jsxs)(x.U, {
-                    children: [(0, i.jsxs)(f.x, {
-                        children: [r, " rows"]
-                    }), (0, i.jsx)(s.J, {
+                }) : t < i ? (0, r.jsxs)(x.U, {
+                    children: [(0, r.jsxs)(f.x, {
+                        children: [i, " rows"]
+                    }), (0, r.jsx)(s.J, {
                         as: en.Tvk,
                         color: "green.500"
-                    }), (0, i.jsxs)(f.x, {
+                    }), (0, r.jsxs)(f.x, {
                         color: "green.500",
-                        children: ["+ ", Math.round((r - t) / t * 100), "%"]
+                        children: ["+ ", Math.round((i - t) / t * 100), "%"]
                     })]
-                }) : (0, i.jsxs)(x.U, {
-                    children: [(0, i.jsxs)(f.x, {
-                        children: [r, " rows"]
-                    }), (0, i.jsx)(s.J, {
+                }) : (0, r.jsxs)(x.U, {
+                    children: [(0, r.jsxs)(f.x, {
+                        children: [i, " rows"]
+                    }), (0, r.jsx)(s.J, {
                         as: en.ebp,
                         color: "red.500"
-                    }), (0, i.jsxs)(f.x, {
+                    }), (0, r.jsxs)(f.x, {
                         color: "red.500",
-                        children: ["- ", Math.round((t - r) / t * 100), "%"]
+                        children: ["- ", Math.round((t - i) / t * 100), "%"]
                     })]
                 })
             }
 
             function ModelRowCount(e) {
                 let {
                     rowCount: n
                 } = e;
-                return n ? (0, i.jsx)(RowCountWiteRate, {
+                return n ? (0, r.jsx)(RowCountWiteRate, {
                     rowCount: n
-                }) : (0, i.jsxs)(x.U, {
-                    children: [(0, i.jsx)(f.x, {
+                }) : (0, r.jsxs)(x.U, {
+                    children: [(0, r.jsx)(f.x, {
                         children: "Failed to load"
-                    }), (0, i.jsx)(s.J, {
+                    }), (0, r.jsx)(s.J, {
                         as: B.KZt,
                         color: "red.500"
                     })]
                 })
             }
 
             function ResourceTypeTag(e) {
                 let {
                     node: n
                 } = e, {
                     icon: t
                 } = getIconForResourceType(n.resourceType);
-                return (0, i.jsx)(o.u, {
+                return (0, r.jsx)(o.u, {
                     hasArrow: !0,
                     label: "Type of resource",
-                    children: (0, i.jsxs)(A.Vp, {
-                        children: [(0, i.jsx)(A.AD, {
+                    children: (0, r.jsxs)(A.Vp, {
+                        children: [(0, r.jsx)(A.AD, {
                             as: t
-                        }), (0, i.jsx)(A.Sn, {
+                        }), (0, r.jsx)(A.Sn, {
                             children: n.resourceType
                         })]
                     })
                 })
             }
 
             function RowCountTag(e) {
                 let {
                     node: n,
                     isAutoFetching: t = !1,
-                    isInteractive: r = !0
+                    isInteractive: i = !0
                 } = e, {
                     isNodesFetching: l
                 } = useRowCountStateContext(), {
                     isLoading: a,
                     data: c,
                     refetch: d,
                     isFetched: u,
@@ -642,148 +642,148 @@
                 }), m = h || l.includes(n.name), x = a || l.includes(n.name);
 
                 function ProcessedRowCountTag(e) {
                     let {
                         isLoading: n,
                         rowCount: t
                     } = e;
-                    return (0, i.jsx)(A.Sn, {
-                        children: (0, i.jsx)(V.N, {
+                    return (0, r.jsx)(A.Sn, {
+                        children: (0, r.jsx)(V.N, {
                             isLoaded: !n,
                             noOfLines: 1,
                             skeletonHeight: 2,
                             minWidth: "30px",
-                            children: (0, i.jsx)(ModelRowCount, {
+                            children: (0, r.jsx)(ModelRowCount, {
                                 rowCount: t
                             })
                         })
                     })
                 }
 
                 function UnprocessedRowCountTag(e) {
                     let {
                         isInteractive: n,
                         invokeFunction: t
                     } = e;
-                    return n ? (0, i.jsx)(P.h, {
+                    return n ? (0, r.jsx)(P.h, {
                         "aria-label": "Query Row Count",
-                        icon: (0, i.jsx)(q.j3i, {}),
+                        icon: (0, r.jsx)(q.j3i, {}),
                         size: "xs",
                         onClick: () => {
                             t()
                         }
-                    }) : (0, i.jsx)(s.J, {
+                    }) : (0, r.jsx)(s.J, {
                         as: q.ebq
                     })
                 }
-                if (!1 === r && !1 === u && !1 === m) return null;
+                if (!1 === i && !1 === u && !1 === m) return null;
                 let f = "Query the number of row";
                 if (m) f = "Querying the number of row";
                 else if (u) {
                     let e = (null == c ? void 0 : c.base) === null ? "N/A" : null == c ? void 0 : c.base,
                         n = (null == c ? void 0 : c.curr) === null ? "N/A" : null == c ? void 0 : c.curr;
                     f = "".concat(e, " -> ").concat(n, " rows")
                 }
-                return (0, i.jsx)(o.u, {
+                return (0, r.jsx)(o.u, {
                     hasArrow: !0,
                     label: f,
                     openDelay: 500,
                     closeDelay: 200,
-                    children: (0, i.jsxs)(A.Vp, {
-                        children: [(0, i.jsx)(A.AD, {
+                    children: (0, r.jsxs)(A.Vp, {
+                        children: [(0, r.jsx)(A.AD, {
                             as: B.SwK
-                        }), u || m ? (0, i.jsx)(ProcessedRowCountTag, {
+                        }), u || m ? (0, r.jsx)(ProcessedRowCountTag, {
                             isLoading: x,
                             rowCount: c
-                        }) : (0, i.jsx)(UnprocessedRowCountTag, {
-                            isInteractive: r,
+                        }) : (0, r.jsx)(UnprocessedRowCountTag, {
+                            isInteractive: i,
                             invokeFunction: d
                         })]
                     })
                 })
             }
             var et = t(85036),
-                ei = t(49294),
-                er = t(46016);
+                er = t(49294),
+                ei = t(46016);
             let ActionTag = e => {
                 let {
                     node: n,
                     action: t
                 } = e, {
-                    status: r,
+                    status: i,
                     skipReason: s,
                     run: c
                 } = t;
-                if ("pending" === r) return (0, i.jsx)(er.D, {
+                if ("pending" === i) return (0, r.jsx)(ei.D, {
                     size: "20px",
                     value: 0
                 });
-                if ("skipped" === r) return (0, i.jsxs)(a.k, {
+                if ("skipped" === i) return (0, r.jsxs)(a.k, {
                     fontSize: "10pt",
                     color: "gray",
-                    children: [(0, i.jsx)(l.xu, {
+                    children: [(0, r.jsx)(l.xu, {
                         children: "Skipped"
-                    }), s && (0, i.jsx)(o.u, {
+                    }), s && (0, r.jsx)(o.u, {
                         label: s,
-                        children: (0, i.jsx)(et.s, {})
+                        children: (0, r.jsx)(et.s, {})
                     })]
                 });
-                if (!c) return (0, i.jsx)(er.D, {
+                if (!c) return (0, r.jsx)(ei.D, {
                     isIndeterminate: !0,
                     size: "20px"
                 });
                 let {
                     error: d,
                     result: u,
                     run_id: h,
                     progress: m
                 } = c;
-                if ("running" === r) return (null == m ? void 0 : m.percentage) === void 0 ? (0, i.jsx)(er.D, {
+                if ("running" === i) return (null == m ? void 0 : m.percentage) === void 0 ? (0, r.jsx)(ei.D, {
                     isIndeterminate: !0,
                     size: "20px"
-                }) : (0, i.jsx)(er.D, {
+                }) : (0, r.jsx)(ei.D, {
                     size: "20px",
                     value: (null == m ? void 0 : m.percentage) * 100
                 });
-                if (d) return (0, i.jsxs)(a.k, {
+                if (d) return (0, r.jsxs)(a.k, {
                     fontSize: "10pt",
                     color: "gray",
-                    children: [(0, i.jsx)(l.xu, {
+                    children: [(0, r.jsx)(l.xu, {
                         children: "Error"
-                    }), s && (0, i.jsx)(o.u, {
+                    }), s && (0, r.jsx)(o.u, {
                         label: d,
-                        children: (0, i.jsx)(ei.a, {})
+                        children: (0, r.jsx)(er.a, {})
                     })]
                 });
                 if ("value_diff" === c.type) {
                     let e = 0;
                     for (let n of u.data.data) n[2] < 1 && e++;
-                    return (0, i.jsx)(A.Vp, {
-                        children: (0, i.jsx)(A.Sn, {
-                            children: (0, i.jsx)(a.k, {
+                    return (0, r.jsx)(A.Vp, {
+                        children: (0, r.jsx)(A.Sn, {
+                            children: (0, r.jsx)(a.k, {
                                 fontSize: "10pt",
                                 color: e > 0 ? "red" : "green",
                                 alignItems: "center",
                                 gap: "3px",
                                 children: e > 0 ? "".concat(e, " columns mismatched") : "All columns match"
                             })
                         })
                     })
                 }
                 if ("row_count_diff" === c.type) {
                     let e = c.result;
-                    return (0, i.jsx)(A.Vp, {
-                        children: (0, i.jsx)(A.Sn, {
-                            children: (0, i.jsx)(ModelRowCount, {
+                    return (0, r.jsx)(A.Vp, {
+                        children: (0, r.jsx)(A.Sn, {
+                            children: (0, r.jsx)(ModelRowCount, {
                                 rowCount: e[n.name]
                             })
                         })
                     })
                 }
-                return (0, i.jsx)(i.Fragment, {
+                return (0, r.jsx)(r.Fragment, {
                     children: h
                 })
             };
 
             function GraphNode(e) {
                 var n, t;
                 let c, {
@@ -791,101 +791,101 @@
                     } = e,
                     {
                         isHighlighted: u,
                         isSelected: h,
                         resourceType: m,
                         changeStatus: f
                     } = d,
-                    p = (0, r.oR)(e => e.transform[2] > .3),
+                    p = (0, i.oR)(e => e.transform[2] > .3),
                     {
                         icon: g
                     } = getIconForResourceType(m),
-                    v = "gray.400",
-                    j = "solid";
-                f && (c = getIconForChangeStatus(f).icon, v = getIconForChangeStatus(f).color);
-                let y = v,
+                    j = "gray.400",
+                    y = "solid";
+                f && (c = getIconForChangeStatus(f).icon, j = getIconForChangeStatus(f).color);
+                let v = j,
                     C = d.isSelected ? "rgba(3, 102, 214, 0.5) 5px 5px 10px 3px" : "unset",
                     b = null == d ? void 0 : d.name;
-                return (0, i.jsx)(o.u, {
+                return (0, r.jsx)(o.u, {
                     label: "model" === m ? b : "".concat(b, " (").concat(m, ")"),
                     placement: "top",
-                    children: (0, i.jsxs)(a.k, {
+                    children: (0, r.jsxs)(a.k, {
                         width: "300px",
                         _hover: {
-                            backgroundColor: p ? "gray.100" : v
+                            backgroundColor: p ? "gray.100" : j
                         },
-                        borderColor: y,
+                        borderColor: v,
                         borderWidth: 1,
-                        borderStyle: j,
-                        backgroundColor: p ? "white" : v,
+                        borderStyle: y,
+                        backgroundColor: p ? "white" : j,
                         borderRadius: 3,
                         boxShadow: C,
                         transition: "box-shadow 0.2s ease-in-out",
                         padding: 0,
                         className: !0 === u ? "node-highlight" : !0 === h ? "node-highlight" : !1 === u ? "node-unhighlight" : void 0,
-                        children: [(0, i.jsx)(a.k, {
-                            backgroundColor: v,
+                        children: [(0, r.jsx)(a.k, {
+                            backgroundColor: j,
                             padding: 2,
                             borderRightWidth: 1,
-                            borderColor: y,
-                            borderStyle: j,
+                            borderColor: v,
+                            borderStyle: y,
                             alignItems: "top",
                             visibility: p ? "inherit" : "hidden",
-                            children: (0, i.jsx)(s.J, {
+                            children: (0, r.jsx)(s.J, {
                                 as: g
                             })
-                        }), (0, i.jsxs)(a.k, {
+                        }), (0, r.jsxs)(a.k, {
                             flex: "1 0 auto",
                             mx: "1",
                             width: "100px",
                             direction: "column",
-                            children: [(0, i.jsxs)(a.k, {
+                            children: [(0, r.jsxs)(a.k, {
                                 width: "100%",
                                 textAlign: "left",
                                 flex: "1",
                                 p: 1,
                                 alignItems: "center",
                                 visibility: p ? "inherit" : "hidden",
-                                children: [(0, i.jsx)(l.xu, {
+                                children: [(0, r.jsx)(l.xu, {
                                     flex: "1",
                                     overflow: "hidden",
                                     textOverflow: "ellipsis",
                                     whiteSpace: "nowrap",
                                     children: b
-                                }), c && (0, i.jsx)(a.k, {
-                                    children: (0, i.jsx)(s.J, {
-                                        color: v,
+                                }), c && (0, r.jsx)(a.k, {
+                                    children: (0, r.jsx)(s.J, {
+                                        color: j,
                                         as: c,
                                         flex: "0 0 20px"
                                     })
                                 })]
-                            }), (0, i.jsx)(a.k, {
+                            }), (0, r.jsx)(a.k, {
                                 flex: "1 0 auto",
                                 mx: "1",
                                 direction: "column",
                                 paddingBottom: "1",
                                 visibility: p ? "inherit" : "hidden",
-                                children: (0, i.jsxs)(x.U, {
+                                children: (0, r.jsxs)(x.U, {
                                     spacing: "8px",
-                                    children: [(0, i.jsx)(E.L, {}), d.action ? (0, i.jsx)(ActionTag, {
+                                    children: [(0, r.jsx)(E.L, {}), d.action ? (0, r.jsx)(ActionTag, {
                                         node: d,
                                         action: d.action
-                                    }) : "model" === d.resourceType ? (0, i.jsx)(RowCountTag, {
+                                    }) : "model" === d.resourceType ? (0, r.jsx)(RowCountTag, {
                                         node: d,
                                         isInteractive: !1
-                                    }) : (0, i.jsx)(i.Fragment, {})]
+                                    }) : (0, r.jsx)(r.Fragment, {})]
                                 })
                             })]
-                        }), Object.keys(null !== (n = null == d ? void 0 : d.parents) && void 0 !== n ? n : {}).length > 0 && (0, i.jsx)(r.HH, {
+                        }), Object.keys(null !== (n = null == d ? void 0 : d.parents) && void 0 !== n ? n : {}).length > 0 && (0, r.jsx)(i.HH, {
                             type: "target",
-                            position: r.Ly.Left,
+                            position: i.Ly.Left,
                             isConnectable: !1
-                        }), Object.keys(null !== (t = null == d ? void 0 : d.children) && void 0 !== t ? t : {}).length > 0 && (0, i.jsx)(r.HH, {
+                        }), Object.keys(null !== (t = null == d ? void 0 : d.children) && void 0 !== t ? t : {}).length > 0 && (0, r.jsx)(i.HH, {
                             type: "source",
-                            position: r.Ly.Right,
+                            position: i.Ly.Right,
                             isConnectable: !1
                         })]
                     })
                 })
             }
 
             function GraphEdge(e) {
@@ -899,24 +899,24 @@
                     style: c = {},
                     markerEnd: d,
                     data: u
                 } = e, h = {
                     ...c
                 };
                 (null == u ? void 0 : u.changeStatus) && (h.stroke = getIconForChangeStatus(null == u ? void 0 : u.changeStatus).color, h.strokeDasharray = "5"), (null == u ? void 0 : u.isHighlighted) === !1 && (h.filter = "opacity(0.2) grayscale(50%)");
-                let [m] = (0, r.OQ)({
+                let [m] = (0, i.OQ)({
                     sourceX: n,
                     sourceY: t,
                     sourcePosition: a,
                     targetX: l,
                     targetY: o,
                     targetPosition: s
                 });
-                return (0, i.jsx)(i.Fragment, {
-                    children: (0, i.jsx)(r.u5, {
+                return (0, r.jsx)(r.Fragment, {
+                    children: (0, r.jsx)(i.u5, {
                         path: m,
                         markerEnd: d,
                         style: {
                             ...h,
                             ...c
                         }
                     })
@@ -932,65 +932,65 @@
                 eh = t(83622),
                 em = t(21801),
                 ex = t(29731),
                 ef = t(18974);
 
             function mergeKeys(e, n) {
                 let t = [...e],
-                    i = [...n],
-                    r = [];
-                for (; t.length > 0 && i.length > 0;)
-                    if (r.includes(t[0])) t.shift();
-                    else if (r.includes(i[0])) i.shift();
-                else if (t[0] === i[0]) r.push(t[0]), t.shift(), i.shift();
-                else if (i.includes(t[0])) {
-                    let e = i.indexOf(t[0]);
-                    for (let n = 0; n < e; n++) r.includes(i[n]) || r.push(i[n]);
-                    r.push(t[0]), t.shift(), i.splice(0, e + 1)
-                } else r.push(t[0]), t.shift();
+                    r = [...n],
+                    i = [];
+                for (; t.length > 0 && r.length > 0;)
+                    if (i.includes(t[0])) t.shift();
+                    else if (i.includes(r[0])) r.shift();
+                else if (t[0] === r[0]) i.push(t[0]), t.shift(), r.shift();
+                else if (r.includes(t[0])) {
+                    let e = r.indexOf(t[0]);
+                    for (let n = 0; n < e; n++) i.includes(r[n]) || i.push(r[n]);
+                    i.push(t[0]), t.shift(), r.splice(0, e + 1)
+                } else i.push(t[0]), t.shift();
                 return t.forEach(e => {
-                    r.includes(e) || r.push(e)
-                }), i.forEach(e => {
-                    r.includes(e) || r.push(e)
-                }), r
+                    i.includes(e) || i.push(e)
+                }), r.forEach(e => {
+                    i.includes(e) || i.push(e)
+                }), i
             }
 
             function mergeKeysWithStatus(e, n) {
                 let t = mergeKeys(e, n),
-                    i = {};
-                for (let r of t) e.includes(r) ? n.includes(r) ? i[r] = void 0 : i[r] = "removed" : i[r] = "added";
-                let r = {};
+                    r = {};
+                for (let i of t) e.includes(i) ? n.includes(i) ? r[i] = void 0 : r[i] = "removed" : r[i] = "added";
+                let i = {};
                 e.forEach((e, n) => {
-                    r[e] = n
+                    i[e] = n
                 });
                 let l = -1;
                 for (let e of t) {
-                    let n = r[e];
-                    void 0 !== n && (n > l ? l = n : i[e] = "reordered")
+                    let n = i[e];
+                    void 0 !== n && (n > l ? l = n : r[e] = "reordered")
                 }
-                return i
+                return r
             }
 
             function mergeColumns() {
                 let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                     n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {},
                     t = {},
-                    i = mergeKeysWithStatus(Object.keys(e), Object.keys(n));
-                return Object.entries(i).forEach(e => {
-                    let [n, i] = e;
+                    r = mergeKeysWithStatus(Object.keys(e), Object.keys(n));
+                return Object.entries(r).forEach(e => {
+                    let [n, r] = e;
                     t[n] = {
                         name: n,
-                        reordered: "reordered" === i
+                        reordered: "reordered" === r
                     }
                 }), Object.entries(e).map((e, n) => {
-                    let [i, r] = e;
-                    t[i].baseIndex = n + 1, t[i].baseType = r.type
+                    let [r, i] = e;
+                    t[r].baseIndex = n + 1, t[r].baseType = i.type
                 }), Object.entries(n).map((e, n) => {
-                    let [i, r] = e;
-                    t[i].currentIndex = n + 1, t[i].currentType = r.type
+                    let [r, i] = e;
+                    t[r].currentIndex = n + 1, t[r].currentType = i.type
                 }), t
             }
 
             function toDataGrid(e) {
                 function columnIndexCellClass(e) {
                     return void 0 === e.baseIndex ? "column-index-added" : void 0 === e.currentIndex ? "column-index-removed" : !0 === e.reordered ? "column-index-reordered" : "column-index-normal"
                 }
@@ -1034,18 +1034,18 @@
                     }],
                     rows: n
                 }
             }
             t(75165), t(91702);
             var ep = t(93683),
                 eg = t(7873),
-                ev = t(52116),
-                ej = t(47367),
-                ey = t(55201),
-                eC = t.n(ey),
+                ej = t(52116),
+                ey = t(47367),
+                ev = t(55201),
+                eC = t.n(ev),
                 eb = t(15550);
 
             function useClipBoardToast() {
                 let e = (0, eb.p)();
                 return {
                     successToast: function(n) {
                         e({
@@ -1072,16 +1072,16 @@
             }
             let ek = "ignore-screenshot";
 
             function useToBlob(e) {
                 let {
                     imageType: n = "png",
                     backgroundColor: t = null,
-                    boardEffect: i = !0,
-                    shadowEffect: r = !1,
+                    boardEffect: r = !0,
+                    shadowEffect: i = !1,
                     borderStyle: l = "solid 1px #ccc",
                     borderRadius: o = "10px",
                     onSuccess: a,
                     onError: s,
                     ignoreElements: c
                 } = e, [d, u] = (0, S.useState)("idle"), h = (0, S.useRef)(null), toImage = async () => {
                     if (!h.current) {
@@ -1095,25 +1095,25 @@
                         f = e.style.backgroundColor;
 
                     function resetStyles() {
                         e.style.overflow = d, e.style.border = m, e.style.borderRadius = x, e.style.backgroundColor = f
                     }
                     try {
                         var p;
-                        e.style.overflow = "hidden", e.style.border = i ? l : "", e.style.borderRadius = i ? o : "", e.style.backgroundColor = t || "";
+                        e.style.overflow = "hidden", e.style.border = r ? l : "", e.style.borderRadius = r ? o : "", e.style.backgroundColor = t || "";
                         let d = document.createElement("style");
                         document.head.appendChild(d), null === (p = d.sheet) || void 0 === p || p.insertRule("body > div:last-child img { display: inline-block; }"), u("loading");
                         let h = await eC()(e, {
                             logging: !1,
                             backgroundColor: null,
                             ignoreElements: c
                         });
                         d.remove();
-                        let m = r ? document.createElement("canvas") : h;
-                        if (r) {
+                        let m = i ? document.createElement("canvas") : h;
+                        if (i) {
                             m.width = h.width + 80, m.height = h.height + 80;
                             let e = m.getContext("2d");
                             if (e) e.shadowColor = "rgba(0, 0, 0, 0.5)", e.shadowBlur = 20, e.shadowOffsetX = 10, e.shadowOffsetY = 10, e.drawImage(h, 40, 40);
                             else {
                                 console.error("Error getting canvas context"), u("error"), s && s(Error("Error getting canvas context to add shadow effect"));
                                 return
                             }
@@ -1149,15 +1149,15 @@
             }
 
             function useCopyToClipboardButton(e) {
                 let {
                     successToast: n,
                     failToast: t
                 } = useClipBoardToast(), {
-                    isLoading: r,
+                    isLoading: i,
                     toImage: l,
                     ref: o
                 } = useToBlob({
                     imageType: "png",
                     shadowEffect: !0,
                     backgroundColor: (null == e ? void 0 : e.backgroundColor) || null,
                     onSuccess: async e => {
@@ -1173,23 +1173,23 @@
                 });
 
                 function CopyToClipboardButton(e) {
                     let {
                         imageType: n = "png",
                         ...t
                     } = e;
-                    return (0, i.jsx)(m.z, {
+                    return (0, r.jsx)(m.z, {
                         size: "sm",
-                        leftIcon: (0, i.jsx)(ej.T, {}),
+                        leftIcon: (0, r.jsx)(ey.T, {}),
                         style: {
                             position: "absolute",
                             bottom: "16px",
                             right: "16px"
                         },
-                        isLoading: r,
+                        isLoading: i,
                         onMouseEnter: () => {
                             if (o.current) {
                                 let e = o.current.element || o.current;
                                 e.style.boxShadow = "rgba(0, 0, 0, 0.25) 0px 54px 55px, rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px, rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px", e.style.transition = "box-shadow 0.5s ease-in-out"
                             }
                         },
                         onMouseLeave: () => {
@@ -1211,26 +1211,43 @@
             }
 
             function ScreenshotDataGrid(e) {
                 let {
                     enableScreenshot: n = !0,
                     ...t
                 } = e, {
-                    ref: r,
+                    ref: i,
                     CopyToClipboardButton: l
                 } = useCopyToClipboardButton();
-                return (0, i.jsxs)(i.Fragment, {
-                    children: [(0, i.jsx)(ev.ZP, {
-                        ref: r,
+                return (0, r.jsxs)(r.Fragment, {
+                    children: [(0, r.jsx)(ej.ZP, {
+                        ref: i,
                         ...t
-                    }), n && (0, i.jsx)(l, {
+                    }), n && (0, r.jsx)(l, {
                         imageType: "png"
                     })]
                 })
             }
+
+            function EmptyRowsRenderer() {
+                return (0, r.jsx)(a.k, {
+                    h: "35px",
+                    alignItems: "center",
+                    justifyContent: "center",
+                    bg: "gray.100",
+                    style: {
+                        textAlign: "center",
+                        gridColumn: "1/-1"
+                    },
+                    children: (0, r.jsx)(f.x, {
+                        fontWeight: "600",
+                        children: " No rows"
+                    })
+                })
+            }
             var ew = t(99691);
             async function getLineage() {
                 let e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0],
                     n = await Q.get("/api/lineage?base=".concat(e));
                 return n.data
             }
             async function getLineageWithError() {
@@ -1242,17 +1259,17 @@
                     }
                 } catch (e) {
                     if (!(e instanceof ew.d7)) return {
                         error: null == e ? void 0 : e.message
                     };
                     {
                         var n, t;
-                        let i = null == e ? void 0 : null === (t = e.response) || void 0 === t ? void 0 : null === (n = t.data) || void 0 === n ? void 0 : n.detail;
-                        if (i) return {
-                            error: i
+                        let r = null == e ? void 0 : null === (t = e.response) || void 0 === t ? void 0 : null === (n = t.data) || void 0 === n ? void 0 : n.detail;
+                        if (r) return {
+                            error: r
                         };
                         return {
                             error: null == e ? void 0 : e.message
                         }
                     }
                 }
             }
@@ -1268,32 +1285,32 @@
             var eS = t(21123),
                 e_ = t.n(eS);
             let eR = (0, S.createContext)({});
 
             function LineageWatcher(e) {
                 let {
                     refetch: n
-                } = e, t = (0, eb.p)(), [r, l] = (0, S.useState)(), o = (0, H.NL)();
+                } = e, t = (0, eb.p)(), [i, l] = (0, S.useState)(), o = (0, H.NL)();
                 return (0, S.useEffect)(() => {
                     function httpUrlToWebSocketUrl(e) {
                         return e.replace(/(http)(s)?\:\/\//, "ws$2://")
                     }
                     let e = new WebSocket("".concat(httpUrlToWebSocketUrl(U), "/api/ws"));
                     return l(e), e.onopen = () => {
                         e.send("ping")
                     }, e.onmessage = e => {
                         if ("pong" !== e.data) try {
                             let n = JSON.parse(e.data);
                             if ("refresh" === n.command) {
                                 let {
                                     eventType: e,
-                                    srcPath: i
-                                } = n.event, [r, l] = i.split("/").slice(-2), a = e_().parse(l).name;
+                                    srcPath: r
+                                } = n.event, [i, l] = r.split("/").slice(-2), a = e_().parse(l).name;
                                 t({
-                                    description: "Detected ".concat(r, " ").concat(a, " ").concat(e),
+                                    description: "Detected ".concat(i, " ").concat(a, " ").concat(e),
                                     status: "info",
                                     variant: "left-accent",
                                     position: "bottom-right",
                                     duration: 5e3,
                                     isClosable: !0
                                 }), o.invalidateQueries({
                                     queryKey: Z.lineage()
@@ -1301,103 +1318,106 @@
                             }
                         } catch (e) {
                             console.error(e)
                         }
                     }, () => {
                         e && e.close()
                     }
-                }, [t, o]), (0, i.jsx)(i.Fragment, {})
+                }, [t, o]), (0, r.jsx)(r.Fragment, {})
             }
 
             function LineageGraphsContextProvider(e) {
                 let {
                     children: n
                 } = e, {
                     data: t,
-                    isLoading: r,
+                    isLoading: i,
                     error: l,
                     refetch: o
                 } = (0, ee.a)({
                     queryKey: Z.lineage(),
                     queryFn: getLineageDiff
                 }), a = (0, S.useMemo)(() => {
                     if (t) return buildDefaultLineageGraphSets(t.base, t.current)
                 }, [t]), s = (null == l ? void 0 : l.message) || (null == t ? void 0 : t.current_error) || (null == t ? void 0 : t.base_error);
-                return (0, i.jsxs)(i.Fragment, {
-                    children: [(0, i.jsx)(LineageWatcher, {
+                return (0, r.jsxs)(r.Fragment, {
+                    children: [(0, r.jsx)(LineageWatcher, {
                         refetch: o
-                    }), (0, i.jsx)(eR.Provider, {
+                    }), (0, r.jsx)(eR.Provider, {
                         value: {
                             lineageGraphSets: a,
                             metadata: null == t ? void 0 : t.current.metadata,
                             isDemoSite: !!(null == t ? void 0 : t.current.metadata.pr_url),
                             error: s,
-                            isLoading: r
+                            isLoading: i
                         },
                         children: n
                     })]
                 })
             }
             let useLineageGraphsContext = () => (0, S.useContext)(eR);
 
             function SchemaView(e) {
                 let n, t, {
-                        base: r,
+                        base: i,
                         current: l,
                         enableScreenshot: o = !1
                     } = e,
                     {
                         columns: s,
                         rows: c
-                    } = (0, S.useMemo)(() => toDataGrid(mergeColumns(null == r ? void 0 : r.columns, null == l ? void 0 : l.columns)), [r, l]),
+                    } = (0, S.useMemo)(() => toDataGrid(mergeColumns(null == i ? void 0 : i.columns, null == l ? void 0 : l.columns)), [i, l]),
                     {
                         lineageGraphSets: d
                     } = useLineageGraphsContext(),
                     u = (null == d ? void 0 : d.catalogExistence.base) === !1,
                     h = (null == d ? void 0 : d.catalogExistence.current) === !1;
                 u && h ? n = "catalog.json is missing on both current and base environments." : u ? n = "catalog.json is missing on base environment." : h && (n = "catalog.json is missing on current environment.");
-                let m = r && void 0 === r.columns,
+                let m = i && void 0 === i.columns,
                     x = l && void 0 === l.columns;
-                return m && x ? t = "Schema information is missing on both current and base environments." : m ? t = "Schema information is missing on base environment." : x && (t = "Schema information is missing on current environment."), (0, i.jsxs)(a.k, {
+                return m && x ? t = "Schema information is missing on both current and base environments." : m ? t = "Schema information is missing on base environment." : x && (t = "Schema information is missing on current environment."), (0, r.jsxs)(a.k, {
                     direction: "column",
-                    children: [n ? (0, i.jsxs)(ep.b, {
+                    children: [n ? (0, r.jsxs)(ep.b, {
                         status: "warning",
                         fontSize: "12px",
                         p: "8px",
-                        children: [(0, i.jsx)(eg.z, {}), n]
-                    }) : t ? (0, i.jsxs)(ep.b, {
+                        children: [(0, r.jsx)(eg.z, {}), n]
+                    }) : t ? (0, r.jsxs)(ep.b, {
                         status: "warning",
                         fontSize: "12px",
                         p: "8px",
-                        children: [(0, i.jsx)(eg.z, {}), t]
-                    }) : (0, i.jsx)(i.Fragment, {}), c.length > 0 && (0, i.jsx)(i.Fragment, {
-                        children: (0, i.jsx)(ScreenshotDataGrid, {
+                        children: [(0, r.jsx)(eg.z, {}), t]
+                    }) : (0, r.jsx)(r.Fragment, {}), c.length > 0 && (0, r.jsx)(r.Fragment, {
+                        children: (0, r.jsx)(ScreenshotDataGrid, {
                             style: {
                                 blockSize: "auto",
                                 maxHeight: "100%",
                                 overflow: "auto",
                                 fontSize: "10pt",
                                 borderWidth: 1
                             },
                             columns: s,
                             rows: c,
+                            renderers: {
+                                noRowsFallback: (0, r.jsx)(EmptyRowsRenderer, {})
+                            },
                             className: "rdg-light",
                             enableScreenshot: o
                         })
                     })]
                 })
             }
             var eD = t(29357);
 
             function SqlDiffView(e) {
                 let {
                     base: n,
                     current: t
                 } = e;
-                return (0, i.jsx)(eD.SV, {
+                return (0, r.jsx)(eD.SV, {
                     height: "500px",
                     language: "sql",
                     theme: "vs",
                     original: null == n ? void 0 : n.raw_code,
                     modified: null == t ? void 0 : t.raw_code,
                     options: {
                         readOnly: !0,
@@ -1408,15 +1428,15 @@
                             enabled: !1
                         },
                         wordWrap: "on",
                         wrappingIndent: "same"
                     }
                 })
             }
-            var eT = t(32865);
+            var eN = t(32865);
             async function createSimpleCheck() {
                 let e = await Q.post("/api/checks", {
                         type: "simple"
                     }),
                     n = e.data;
                 return n
             }
@@ -1424,16 +1444,16 @@
                 let t = await Q.post("/api/checks", {
                         type: "lineage_diff",
                         params: {
                             view_mode: e,
                             node_ids: n
                         }
                     }),
-                    i = t.data;
-                return i
+                    r = t.data;
+                return r
             }
             async function createCheckByNodeSchema(e) {
                 let n = await Q.post("/api/checks", {
                         type: "schema_diff",
                         params: {
                             node_id: e
                         }
@@ -1442,16 +1462,16 @@
                 return t
             }
             async function checks_createCheckByRun(e, n) {
                 let t = await Q.post("/api/checks", {
                         run_id: e,
                         view_options: n
                     }),
-                    i = t.data;
-                return i
+                    r = t.data;
+                return r
             }
             async function listChecks() {
                 let e = await Q.get("/api/checks");
                 return e.data
             }
             async function getCheck(e) {
                 let n = await Q.get("/api/checks/".concat(e));
@@ -1474,69 +1494,69 @@
             }
             async function loadChecks(e) {
                 let n = new FormData;
                 n.append("file", e);
                 let t = await Q.post("/api/checks/load", n);
                 return t.data
             }
-            var eN = t(78448),
+            var eT = t(78448),
                 eE = t(93573);
 
             function ColumnNameCell(e) {
                 let {
                     params: n,
                     column: t,
-                    containerRef: r
+                    containerRef: i
                 } = e, {
                     runAction: o
                 } = useRecceActionContext(), handleValueDiffDetail = (e, t) => {
-                    let i = {
+                    let r = {
                         ...n,
                         ...e
                     };
-                    o("value_diff_detail", i, t)
+                    o("value_diff_detail", r, t)
                 };
-                return (0, i.jsxs)(a.k, {
-                    children: [(0, i.jsx)(l.xu, {
+                return (0, r.jsxs)(a.k, {
+                    children: [(0, r.jsx)(l.xu, {
                         overflow: "hidden",
                         textOverflow: "ellipsis",
                         whiteSpace: "nowrap",
                         children: t
-                    }), (0, i.jsx)(E.L, {}), (0, i.jsx)(b.v, {
+                    }), (0, r.jsx)(E.L, {}), (0, r.jsx)(b.v, {
                         children: e => {
                             let {
                                 isOpen: n
                             } = e;
-                            return (0, i.jsxs)(i.Fragment, {
-                                children: [(0, i.jsx)(ef.j, {
+                            return (0, r.jsxs)(r.Fragment, {
+                                children: [(0, r.jsx)(ef.j, {
                                     className: "row-context-menu",
                                     visibility: n ? "visible" : "hidden",
                                     width: n ? "auto" : "0px",
                                     minWidth: n ? "auto" : "0px",
                                     as: P.h,
-                                    icon: (0, i.jsx)(s.J, {
+                                    icon: (0, r.jsx)(s.J, {
                                         as: L.D_A
                                     }),
                                     variant: "unstyled",
                                     size: "sm"
-                                }), (0, i.jsx)(eN.h, {
-                                    containerRef: r,
-                                    children: (0, i.jsx)(k.q, {
+                                }), (0, r.jsx)(eT.h, {
+                                    containerRef: i,
+                                    children: (0, r.jsx)(k.q, {
                                         lineHeight: "20px",
-                                        children: (0, i.jsxs)(eE.k, {
+                                        children: (0, r.jsxs)(eE.k, {
                                             title: "Action",
                                             as: l.xu,
                                             fontSize: "8pt",
-                                            children: [(0, i.jsx)(w.s, {
+                                            children: [(0, r.jsx)(w.s, {
                                                 fontSize: "10pt",
                                                 onClick: () => handleValueDiffDetail({}, {
                                                     showForm: !0
                                                 }),
                                                 children: "Show mismatched values..."
-                                            }), (0, i.jsxs)(w.s, {
+                                            }), (0, r.jsxs)(w.s, {
                                                 fontSize: "10pt",
                                                 onClick: () => handleValueDiffDetail({
                                                     columns: [t]
                                                 }, {
                                                     showForm: !1
                                                 }),
                                                 children: ["Show mismatched values for '", t, "'"]
@@ -1549,44 +1569,44 @@
                     })]
                 })
             }
 
             function ValueDiffResultView(e) {
                 let {
                     run: n
-                } = e, t = n.result, r = n.params, cellClass = e => {
+                } = e, t = n.result, i = n.params, cellClass = e => {
                     let n = e[2];
                     return null != n && n < 1 ? "diff-cell-modified" : ""
                 }, o = (0, S.useRef)(), c = [{
                     key: "__is_pk__",
                     name: "",
                     maxWidth: 30,
                     renderCell: e => {
                         let {
                             row: n
                         } = e;
-                        return (0, i.jsx)(u.M, {
+                        return (0, r.jsx)(u.M, {
                             height: "100%",
-                            children: n[0] === r.primary_key && (0, i.jsx)(s.J, {
+                            children: n[0] === i.primary_key && (0, r.jsx)(s.J, {
                                 as: L.MhP
                             })
                         })
                     }
                 }, {
                     key: "0",
                     name: "Column",
                     resizable: !0,
                     renderCell: e => {
                         let {
                             row: n,
                             column: t
                         } = e;
-                        return (0, i.jsx)(ColumnNameCell, {
+                        return (0, r.jsx)(ColumnNameCell, {
                             column: n[t.key],
-                            params: r,
+                            params: i,
                             containerRef: o
                         })
                     },
                     cellClass: "cell-show-context-menu"
                 }, {
                     key: "1",
                     name: "Matched",
@@ -1596,235 +1616,238 @@
                     key: "2",
                     name: "Matched %",
                     resizable: !0,
                     renderCell: e => {
                         let {
                             column: n,
                             row: t
-                        } = e, r = t[n.key];
-                        return (0, i.jsx)(l.xu, {
+                        } = e, i = t[n.key];
+                        return (0, r.jsx)(l.xu, {
                             textAlign: "end",
-                            children: void 0 != r && null !== r ? "".concat((100 * r).toFixed(2), " %") : "N/A"
+                            children: void 0 != i && null !== i ? "".concat((100 * i).toFixed(2), " %") : "N/A"
                         })
                     },
                     cellClass
                 }];
-                return (0, i.jsxs)(a.k, {
+                return (0, r.jsxs)(a.k, {
                     direction: "column",
                     gap: "5px",
                     pt: "5px",
                     height: "100%",
                     ref: o,
-                    children: [(0, i.jsxs)(l.xu, {
+                    children: [(0, r.jsxs)(l.xu, {
                         px: "16px",
-                        children: ["Model: ", r.model, ", ", t.summary.total, " total (", t.summary.total - t.summary.added - t.summary.removed, " ", "common, ", t.summary.added, " added, ", t.summary.removed, " removed)"]
-                    }), (0, i.jsx)(ScreenshotDataGrid, {
+                        children: ["Model: ", i.model, ", ", t.summary.total, " total (", t.summary.total - t.summary.added - t.summary.removed, " ", "common, ", t.summary.added, " added, ", t.summary.removed, " removed)"]
+                    }), (0, r.jsx)(ScreenshotDataGrid, {
                         style: {
                             blockSize: "auto",
                             maxHeight: "100%",
                             overflow: "auto",
                             borderBlock: "1px solid lightgray"
                         },
                         columns: c,
                         rows: t.data.data,
+                        renderers: {
+                            noRowsFallback: (0, r.jsx)(EmptyRowsRenderer, {})
+                        },
                         defaultColumnOptions: {
                             resizable: !0
                         },
                         className: "rdg-light",
                         enableScreenshot: !0
                     })]
                 })
             }
             var eL = t(41171),
                 eI = t(53930),
                 ez = t(25535),
-                eM = t(51348),
-                eF = t(11546),
+                eF = t(51348),
+                eM = t(11546),
                 eO = t(83978),
                 eA = t.n(eO);
 
             function extractColumns(e) {
                 function getColumns(e) {
                     return e && e.columns ? Object.values(e.columns) : []
                 }
                 let n = getColumns(e.data.base),
                     t = getColumns(e.data.current),
-                    i = [];
+                    r = [];
                 return n.forEach(e => {
-                    i.some(n => n.name === e.name) || i.push(e)
+                    r.some(n => n.name === e.name) || r.push(e)
                 }), t.forEach(e => {
-                    i.some(n => n.name === e.name) || i.push(e)
-                }), i
+                    r.some(n => n.name === e.name) || r.push(e)
+                }), r
             }
 
             function extractColumnNames(e) {
                 function getNames(e) {
                     return e && e.columns ? Object.values(e.columns).map(e => e.name) : []
                 }
                 let n = getNames(e.data.base),
                     t = getNames(e.data.current),
-                    i = [];
+                    r = [];
                 return n.forEach(e => {
-                    i.includes(e) || i.push(e)
+                    r.includes(e) || r.push(e)
                 }), t.forEach(e => {
-                    i.includes(e) || i.push(e)
-                }), i
+                    r.includes(e) || r.push(e)
+                }), r
             }
 
             function ValueDiffForm(e) {
                 var n, t;
                 let {
-                    params: r,
+                    params: i,
                     onParamsChanged: l,
                     setIsReadyToExecute: o
-                } = e, a = useLineageGraphsContext(), [s, c] = (0, S.useState)(!r.columns || 0 === r.columns.length), d = null == r ? void 0 : r.model, u = null == r ? void 0 : r.primary_key, m = eA().find(null === (n = a.lineageGraphSets) || void 0 === n ? void 0 : n.all.nodes, {
-                    name: null == r ? void 0 : r.model
+                } = e, a = useLineageGraphsContext(), [s, c] = (0, S.useState)(!i.columns || 0 === i.columns.length), d = null == i ? void 0 : i.model, u = null == i ? void 0 : i.primary_key, m = eA().find(null === (n = a.lineageGraphSets) || void 0 === n ? void 0 : n.all.nodes, {
+                    name: null == i ? void 0 : i.model
                 }), x = null == m ? void 0 : null === (t = m.data.current) || void 0 === t ? void 0 : t.primary_key;
                 (0, S.useEffect)(() => {
                     !u && x && l({
-                        ...r,
+                        ...i,
                         primary_key: x
                     })
-                }, [u, x, r, l]), (0, S.useEffect)(() => {
+                }, [u, x, i, l]), (0, S.useEffect)(() => {
                     o(!!u && !!d)
                 }, [u, d, o]);
                 let f = m ? extractColumnNames(m) : [];
-                return (0, i.jsxs)(h.g, {
+                return (0, r.jsxs)(h.g, {
                     gap: 5,
                     m: "8px 24px",
                     paddingBottom: "200px",
-                    children: [(0, i.jsxs)(eL.NI, {
-                        children: [(0, i.jsx)(eI.l, {
+                    children: [(0, r.jsxs)(eL.NI, {
+                        children: [(0, r.jsx)(eI.l, {
                             children: "Model"
-                        }), (0, i.jsx)(ez.I, {
+                        }), (0, r.jsx)(ez.I, {
                             isReadOnly: !0,
-                            value: null == r ? void 0 : r.model
+                            value: null == i ? void 0 : i.model
                         })]
-                    }), (0, i.jsxs)(eL.NI, {
-                        children: [(0, i.jsx)(eI.l, {
+                    }), (0, r.jsxs)(eL.NI, {
+                        children: [(0, r.jsx)(eI.l, {
                             children: "Primary key"
-                        }), (0, i.jsx)(eF.Z, {
+                        }), (0, r.jsx)(eM.Z, {
                             placeholder: "Select primary key",
                             value: u ? {
                                 label: u,
                                 value: u
                             } : void 0,
                             options: (f || []).map(e => ({
                                 label: e,
                                 value: e
                             })),
                             onChange: e => {
                                 c(!0), l({
-                                    ...r,
+                                    ...i,
                                     primary_key: (null == e ? void 0 : e.value) || "",
                                     columns: void 0
                                 })
                             }
                         })]
-                    }), (0, i.jsxs)(eL.NI, {
-                        children: [(0, i.jsx)(eI.l, {
+                    }), (0, r.jsxs)(eL.NI, {
+                        children: [(0, r.jsx)(eI.l, {
                             children: "Columns"
-                        }), (0, i.jsx)(eM.X, {
+                        }), (0, r.jsx)(eF.X, {
                             marginBottom: "10px",
                             isChecked: s,
                             onChange: e => {
                                 c(e.target.checked), l({
-                                    ...r,
+                                    ...i,
                                     columns: void 0
                                 })
                             },
                             children: "All columns"
-                        }), !s && (0, i.jsx)(eF.Z, {
+                        }), !s && (0, r.jsx)(eM.Z, {
                             isMulti: !0,
                             closeMenuOnSelect: !1,
                             options: (f || []).map(e => ({
                                 label: e,
                                 value: e
                             })),
-                            value: (r.columns || []).map(e => ({
+                            value: (i.columns || []).map(e => ({
                                 label: e,
                                 value: e
                             })),
                             onChange: e => {
                                 l({
-                                    ...r,
+                                    ...i,
                                     columns: (e || []).map(e => e.value)
                                 })
                             }
                         })]
                     })]
                 })
             }
 
             function _getColumnMap(e, n) {
                 let t = {},
-                    i = mergeKeysWithStatus(e.columns.map(e => e.name), n.columns.map(e => e.name));
-                return Object.entries(i).map(i => {
-                    let [r, l] = i;
-                    t[r] = {
+                    r = mergeKeysWithStatus(e.columns.map(e => e.name), n.columns.map(e => e.name));
+                return Object.entries(r).map(r => {
+                    let [i, l] = r;
+                    t[i] = {
                         status: l,
-                        baseColumnIndex: e.columns.findIndex(e => e.name === r),
-                        currentColumnIndex: n.columns.findIndex(e => e.name === r)
+                        baseColumnIndex: e.columns.findIndex(e => e.name === i),
+                        currentColumnIndex: n.columns.findIndex(e => e.name === i)
                     }
                 }), t
             }
 
             function _getPrimaryKeyIndexes(e, n) {
                 let t = [];
-                for (let i of n) {
-                    let n = e.findIndex(e => e.name === i);
-                    if (n < 0) throw Error("Column ".concat(i, " not found"));
+                for (let r of n) {
+                    let n = e.findIndex(e => e.name === r);
+                    if (n < 0) throw Error("Column ".concat(r, " not found"));
                     t.push(n)
                 }
                 return t
             }
 
             function _getPrimaryKeyValue(e, n, t) {
-                let i = {};
+                let r = {};
                 if (0 === n.length) return JSON.stringify({
                     _index: t._index
                 });
-                for (let r of n) {
-                    let n = e[r];
-                    i[n.name] = t[r]
+                for (let i of n) {
+                    let n = e[i];
+                    r[n.name] = t[i]
                 }
-                return JSON.stringify(i)
+                return JSON.stringify(r)
             }
 
             function DataFrameColumnGroupHeader(e) {
                 let {
                     name: n,
                     columnStatus: t,
-                    onPrimaryKeyChange: r,
+                    onPrimaryKeyChange: i,
                     onPinnedColumnsChange: o,
                     ...c
                 } = e, d = c.primaryKeys || [], u = c.pinnedColumns || [], h = d.includes(n), m = u.includes(n);
-                return "index" === n ? (0, i.jsx)(i.Fragment, {}) : (0, i.jsxs)(a.k, {
+                return "index" === n ? (0, r.jsx)(r.Fragment, {}) : (0, r.jsxs)(a.k, {
                     alignItems: "center",
                     gap: "10px",
                     className: "grid-header",
-                    children: [(0, i.jsx)(l.xu, {
+                    children: [(0, r.jsx)(l.xu, {
                         flex: 1,
                         overflow: "hidden",
                         textOverflow: "ellipsis",
                         whiteSpace: "nowrap",
                         children: n
-                    }), "added" !== t && "removed" !== t && r && (0, i.jsx)(s.J, {
+                    }), "added" !== t && "removed" !== t && i && (0, r.jsx)(s.J, {
                         className: h ? "close-icon" : "key-icon",
                         display: h ? "block" : "none",
                         cursor: "pointer",
                         as: h ? L.ven : L.MhP,
                         onClick: h ? () => {
                             let e = d.filter(e => e !== n);
-                            r && r(e)
+                            i && i(e)
                         } : () => {
                             let e = [...d.filter(e => "index" !== e), n];
-                            r && r(e)
+                            i && i(e)
                         }
-                    }), !h && o && (0, i.jsx)(s.J, {
+                    }), !h && o && (0, r.jsx)(s.J, {
                         className: m ? "unpin-icon" : "pin-icon",
                         display: m ? "block" : "none",
                         cursor: "pointer",
                         as: m ? L.$kI : L.oJP,
                         onClick: m ? () => {
                             let e = u.filter(e => e !== n);
                             o && o(e)
@@ -1836,166 +1859,166 @@
                 })
             }
             t(7866);
             let defaultRenderCell = e => {
                 let {
                     row: n,
                     column: t
-                } = e, r = n[t.key];
-                return (0, i.jsx)(i.Fragment, {
-                    children: "boolean" == typeof r ? r.toString() : r
+                } = e, i = n[t.key];
+                return (0, r.jsx)(r.Fragment, {
+                    children: "boolean" == typeof i ? i.toString() : i
                 })
             };
 
             function toDataDiffGrid(e, n, t) {
-                let r = e || {
+                let i = e || {
                         columns: [],
                         data: []
                     },
                     l = n || {
                         columns: [],
                         data: []
                     },
                     o = (null == t ? void 0 : t.primaryKeys) || [],
                     a = (null == t ? void 0 : t.pinnedColumns) || [],
                     s = (null == t ? void 0 : t.changedOnly) || !1,
                     c = [],
-                    d = _getColumnMap(r, l),
+                    d = _getColumnMap(i, l),
                     u = {},
                     h = {},
                     m = !1,
                     x = !1;
-                if (0 === o.length) r.data.forEach((e, n) => {
+                if (0 === o.length) i.data.forEach((e, n) => {
                     e._index = n + 1, u[JSON.stringify({
                         _index: n + 1
                     })] = e
                 }), l.data.forEach((e, n) => {
                     e._index = n + 1, h[JSON.stringify({
                         _index: n + 1
                     })] = e
                 });
                 else {
-                    let e = _getPrimaryKeyIndexes(r.columns, o);
-                    r.data.forEach((n, t) => {
-                        let i = _getPrimaryKeyValue(r.columns, e, n);
-                        i in u && (m = !0), u[i] = n
+                    let e = _getPrimaryKeyIndexes(i.columns, o);
+                    i.data.forEach((n, t) => {
+                        let r = _getPrimaryKeyValue(i.columns, e, n);
+                        r in u && (m = !0), u[r] = n
                     }), e = _getPrimaryKeyIndexes(l.columns, o), l.data.forEach((n, t) => {
-                        let i = _getPrimaryKeyValue(l.columns, e, n);
-                        i in h && (x = !0), h[i] = n
+                        let r = _getPrimaryKeyValue(l.columns, e, n);
+                        r in h && (x = !0), h[r] = n
                     })
                 }
                 let f = mergeKeysWithStatus(Object.keys(u), Object.keys(h)),
                     p = Object.entries(f).map(e => {
-                        let [n, t] = e, i = u[n], a = h[n], s = JSON.parse(n);
-                        if (i && r.columns.forEach((e, n) => {
-                                o.includes(e.name) || (s["base__".concat(e.name)] = i[n])
+                        let [n, t] = e, r = u[n], a = h[n], s = JSON.parse(n);
+                        if (r && i.columns.forEach((e, n) => {
+                                o.includes(e.name) || (s["base__".concat(e.name)] = r[n])
                             }), a && l.columns.forEach((e, n) => {
                                 o.includes(e.name) || (s["current__".concat(e.name)] = a[n])
-                            }), i) {
+                            }), r) {
                             if (a)
-                                for (let [e, n] of Object.entries(d)) "index" === e || o.includes(e) || n.baseColumnIndex < 0 || n.currentColumnIndex < 0 || eA().isEqual(i[n.baseColumnIndex], a[n.currentColumnIndex]) || (s.status = "modified", n.status = "modified");
+                                for (let [e, n] of Object.entries(d)) "index" === e || o.includes(e) || n.baseColumnIndex < 0 || n.currentColumnIndex < 0 || eA().isEqual(r[n.baseColumnIndex], a[n.currentColumnIndex]) || (s.status = "modified", n.status = "modified");
                             else s.status = "removed"
                         } else s.status = "added";
                         return s
                     });
                 s && (p = p.filter(e => "added" === e.status || "removed" === e.status || "modified" === e.status));
                 let toColumn = (e, n) => {
-                    let r = "added" === n ? "diff-header-added" : "removed" === n ? "diff-header-removed" : void 0,
+                    let i = "added" === n ? "diff-header-added" : "removed" === n ? "diff-header-removed" : void 0,
                         cellClass = t => {
-                            let i = t.status;
-                            if ("removed" === i) return "diff-cell-removed";
-                            if ("added" === i) return "diff-cell-added";
+                            let r = t.status;
+                            if ("removed" === r) return "diff-cell-removed";
+                            if ("added" === r) return "diff-cell-added";
                             if ("added" === n);
                             else if ("removed" === n);
                             else if (!eA().isEqual(t["base__".concat(e)], t["current__".concat(e)])) return "diff-cell-modified"
                         };
                     return {
-                        headerCellClass: r,
-                        name: (0, i.jsx)(DataFrameColumnGroupHeader, {
+                        headerCellClass: i,
+                        name: (0, r.jsx)(DataFrameColumnGroupHeader, {
                             name: e,
                             columnStatus: n,
                             ...t
                         }),
                         children: [{
                             key: "base__".concat(e),
                             name: "Base",
-                            renderEditCell: ev.Ug,
-                            headerCellClass: r,
+                            renderEditCell: ej.Ug,
+                            headerCellClass: i,
                             cellClass,
                             renderCell: defaultRenderCell,
                             size: "auto"
                         }, {
                             key: "current__".concat(e),
                             name: "Current",
-                            renderEditCell: ev.Ug,
-                            headerCellClass: r,
+                            renderEditCell: ej.Ug,
+                            headerCellClass: i,
                             cellClass,
                             renderCell: defaultRenderCell,
                             size: "auto"
                         }]
                     }
                 };
                 return 0 === o.length ? c.push({
                     key: "_index",
                     name: "",
                     cellClass: "index-column"
                 }) : o.forEach(e => {
                     let n = d[e].status || "";
                     c.push({
                         key: "".concat(e),
-                        name: (0, i.jsx)(DataFrameColumnGroupHeader, {
+                        name: (0, r.jsx)(DataFrameColumnGroupHeader, {
                             name: e,
                             columnStatus: n,
                             ...t
                         }),
                         frozen: !0,
                         cellClass: e => {
                             if (e.status) return "diff-header-".concat(e.status)
                         }
                     })
                 }), a.forEach(e => {
                     let n = d[e].status || "";
                     "index" === e || o.includes(e) || c.push(toColumn(e, n))
                 }), Object.entries(d).forEach(e => {
-                    let [n, t] = e, i = t.status || "";
-                    "index" === n || o.includes(n) || a.includes(n) || s && "added" !== i && "removed" !== i && "modified" !== i || c.push(toColumn(n, i))
+                    let [n, t] = e, r = t.status || "";
+                    "index" === n || o.includes(n) || a.includes(n) || s && "added" !== r && "removed" !== r && "modified" !== r || c.push(toColumn(n, r))
                 }), {
                     columns: c,
                     rows: p,
                     invalidPKeyBase: m,
                     invalidPKeyCurrent: x
                 }
             }
 
             function ProfileDiffResultView(e) {
                 var n;
                 let {
                     run: t,
-                    viewOptions: r,
+                    viewOptions: i,
                     onViewOptionsChanged: l
                 } = e, o = t.result;
                 t.params;
-                let a = (0, S.useMemo)(() => (null == r ? void 0 : r.pinned_columns) || [], [r]),
+                let a = (0, S.useMemo)(() => (null == i ? void 0 : i.pinned_columns) || [], [i]),
                     s = ((null == o ? void 0 : null === (n = o.current) || void 0 === n ? void 0 : n.columns) || []).find(e => "column_name" === e.name.toLowerCase()),
                     c = (null == s ? void 0 : s.name) || "column_name",
                     d = (0, S.useMemo)(() => toDataDiffGrid(null == o ? void 0 : o.base, null == o ? void 0 : o.current, {
                         primaryKeys: [c],
                         pinnedColumns: a,
                         onPinnedColumnsChange: e => {
                             l && l({
-                                ...r,
+                                ...i,
                                 pinned_columns: e
                             })
                         }
-                    }), [o, c, a, r, l]);
-                return 0 === d.columns.length ? (0, i.jsx)(u.M, {
+                    }), [o, c, a, i, l]);
+                return 0 === d.columns.length ? (0, r.jsx)(u.M, {
                     height: "100%",
                     children: "No data"
-                }) : (0, i.jsx)(i.Fragment, {
-                    children: (0, i.jsx)(ScreenshotDataGrid, {
+                }) : (0, r.jsx)(r.Fragment, {
+                    children: (0, r.jsx)(ScreenshotDataGrid, {
                         style: {
                             blockSize: "auto",
                             maxHeight: "100%",
                             overflow: "auto"
                         },
                         columns: d.columns,
                         rows: d.rows,
@@ -2010,208 +2033,208 @@
                 })
             }
             var eV = t(84680),
                 eP = t(70556);
             let RunView = e => {
                 var n, t;
                 let {
-                    isPending: r,
+                    isPending: i,
                     isAborting: o,
                     progress: s,
                     error: c,
                     run: d,
                     onCancel: x,
                     viewOptions: f,
                     onViewOptionsChanged: p,
                     RunResultView: g,
-                    children: v
+                    children: j
                 } = e;
-                if (v && g) throw Error("RunView requires either a children or a RunResultView prop, but not both.");
-                if (!v && !g) throw Error("RunView requires at least one of children or RunResultView prop.");
-                let j = (null == c ? void 0 : null === (t = c.response) || void 0 === t ? void 0 : null === (n = t.data) || void 0 === n ? void 0 : n.detail) || (null == d ? void 0 : d.error);
-                if (j) return (0, i.jsxs)(ep.b, {
+                if (j && g) throw Error("RunView requires either a children or a RunResultView prop, but not both.");
+                if (!j && !g) throw Error("RunView requires at least one of children or RunResultView prop.");
+                let y = (null == c ? void 0 : null === (t = c.response) || void 0 === t ? void 0 : null === (n = t.data) || void 0 === n ? void 0 : n.detail) || (null == d ? void 0 : d.error);
+                if (y) return (0, r.jsxs)(ep.b, {
                     status: "error",
-                    children: [(0, i.jsx)(eg.z, {}), "Error: ", j]
+                    children: [(0, r.jsx)(eg.z, {}), "Error: ", y]
                 });
-                if (r) {
+                if (i) {
                     let e = (null == s ? void 0 : s.message) ? null == s ? void 0 : s.message : "Loading...";
-                    return (0, i.jsx)(u.M, {
+                    return (0, r.jsx)(u.M, {
                         p: "16px",
                         height: "100%",
                         bg: "rgb(249,249,249)",
-                        children: (0, i.jsxs)(h.g, {
-                            children: [(0, i.jsxs)(a.k, {
+                        children: (0, r.jsxs)(h.g, {
+                            children: [(0, r.jsxs)(a.k, {
                                 alignItems: "center",
-                                children: [(null == s ? void 0 : s.percentage) === void 0 || (null == s ? void 0 : s.percentage) === null ? (0, i.jsx)(er.D, {
+                                children: [(null == s ? void 0 : s.percentage) === void 0 || (null == s ? void 0 : s.percentage) === null ? (0, r.jsx)(ei.D, {
                                     isIndeterminate: !0,
                                     size: "20px",
                                     mr: "8px"
-                                }) : (0, i.jsx)(er.D, {
+                                }) : (0, r.jsx)(ei.D, {
                                     size: "20px",
                                     value: 100 * s.percentage,
                                     mr: "8px"
-                                }), o ? (0, i.jsx)(i.Fragment, {
+                                }), o ? (0, r.jsx)(r.Fragment, {
                                     children: "Aborting..."
-                                }) : (0, i.jsx)(i.Fragment, {
+                                }) : (0, r.jsx)(r.Fragment, {
                                     children: e
                                 })]
-                            }), !o && (0, i.jsx)(m.z, {
+                            }), !o && (0, r.jsx)(m.z, {
                                 onClick: x,
                                 colorScheme: "blue",
                                 size: "sm",
                                 children: "Cancel"
                             })]
                         })
                     })
                 }
-                return d ? (0, i.jsxs)(l.xu, {
+                return d ? (0, r.jsxs)(l.xu, {
                     h: "100%",
                     style: {
                         contain: "size layout"
                     },
                     overflow: "auto",
-                    children: [g && (0, i.jsx)(g, {
+                    children: [g && (0, r.jsx)(g, {
                         run: d,
                         viewOptions: f,
                         onViewOptionsChanged: p
-                    }), v && v({
+                    }), j && j({
                         run: d,
                         viewOptions: f,
                         onViewOptionsChanged: p
                     })]
-                }) : (0, i.jsx)(u.M, {
+                }) : (0, r.jsx)(u.M, {
                     bg: "rgb(249,249,249)",
                     height: "100%",
                     children: "No data"
                 })
             };
             var eB = t(48689);
             let RunModal = e => {
                 let {
                     isOpen: n,
                     onClose: t,
-                    type: r,
+                    type: i,
                     title: o,
                     params: s,
                     initialRun: c,
                     RunForm: d,
                     RunResultView: u
-                } = e, [, h] = (0, eT.TH)(), [x, f] = (0, S.useState)(), [p, b] = (0, S.useState)(s), [k, w] = (0, S.useState)(!1), [_, R] = (0, S.useState)(!1), [D, T] = (0, S.useState)(), [N, E] = (0, S.useState)(), [L, I] = (0, S.useState)(c), submitRunFn = async () => {
+                } = e, [, h] = (0, eN.TH)(), [x, f] = (0, S.useState)(), [p, b] = (0, S.useState)(s), [k, w] = (0, S.useState)(!1), [_, R] = (0, S.useState)(!1), [D, N] = (0, S.useState)(), [T, E] = (0, S.useState)(), [L, I] = (0, S.useState)(c), submitRunFn = async () => {
                     let {
                         run_id: e
-                    } = await submitRun(r, p, {
+                    } = await submitRun(i, p, {
                         nowait: !0
                     });
                     for (f(e);;) {
                         let n = await waitRun(e, 2);
-                        if (T(n.progress), n.result || n.error) return w(!1), T(void 0), n
+                        if (N(n.progress), n.result || n.error) return w(!1), N(void 0), n
                     }
                 }, {
                     data: z,
-                    mutate: M,
-                    reset: F,
+                    mutate: F,
+                    reset: M,
                     error: O,
                     isPending: A
                 } = (0, eP.D)({
                     mutationFn: submitRunFn
                 });
                 (0, S.useEffect)(() => {
-                    n && void 0 === d && void 0 === L && M()
+                    n && void 0 === d && void 0 === L && F()
                 }, [n]);
                 let V = (0, H.NL)(),
                     P = (0, S.useCallback)(async () => {
                         if (w(!0), x) return await cancelRun(x)
                     }, [x]),
                     B = (0, S.useCallback)(() => {
-                        M()
-                    }, [M]),
+                        F()
+                    }, [F]),
                     q = (0, S.useCallback)(() => {
-                        M(), I(void 0)
-                    }, [M]),
+                        F(), I(void 0)
+                    }, [F]),
                     handleReset = () => {
-                        w(!1), b(s), T(void 0), I(void 0), F()
+                        w(!1), b(s), N(void 0), I(void 0), M()
                     },
                     K = (0, S.useCallback)(async () => {
                         let e = L ? L.run_id : null == z ? void 0 : z.run_id;
                         if (void 0 === e) return;
-                        let n = await checks_createCheckByRun(e, N);
+                        let n = await checks_createCheckByRun(e, T);
                         V.invalidateQueries({
                             queryKey: Z.checks()
                         }), h("/checks/".concat(n.check_id))
-                    }, [null == z ? void 0 : z.run_id, L, h, V, N]),
+                    }, [null == z ? void 0 : z.run_id, L, h, V, T]),
                     handleClose = async () => {
                         t(), A && x && await cancelRun(x), handleReset()
                     }, W = !!(null == L ? void 0 : L.result) || !!(null == z ? void 0 : z.result), U = (null == L ? void 0 : L.run_at) ? (0, eB.Z)(new Date(L.run_at), {
                         addSuffix: !0
                     }) : null;
-                return (0, i.jsxs)(g.u_, {
+                return (0, r.jsxs)(g.u_, {
                     isOpen: n,
                     onClose: handleClose,
                     size: "6xl",
                     scrollBehavior: "inside",
-                    children: [(0, i.jsx)(v.Z, {}), (0, i.jsxs)(j.h, {
+                    children: [(0, r.jsx)(j.Z, {}), (0, r.jsxs)(y.h, {
                         overflowY: "auto",
                         height: "75%",
-                        children: [(0, i.jsxs)(es.x, {
-                            children: [o, !z && !A && U && (0, i.jsx)(l.xu, {
+                        children: [(0, r.jsxs)(es.x, {
+                            children: [o, !z && !A && U && (0, r.jsx)(l.xu, {
                                 textOverflow: "ellipsis",
                                 whiteSpace: "nowrap",
                                 overflow: "hidden",
                                 fontSize: "10pt",
                                 children: U
                             })]
-                        }), (0, i.jsx)(y.o, {}), (0, i.jsx)(C.f, {
+                        }), (0, r.jsx)(v.o, {}), (0, r.jsx)(C.f, {
                             p: "0px",
                             h: "100%",
                             overflow: "auto",
                             borderY: "1px solid lightgray",
-                            children: A || z || O || L ? (0, i.jsx)(RunView, {
+                            children: A || z || O || L ? (0, r.jsx)(RunView, {
                                 isPending: A,
                                 isAborting: k,
                                 run: L || z,
                                 error: O,
                                 progress: D,
                                 onCancel: P,
-                                viewOptions: N,
+                                viewOptions: T,
                                 onViewOptionsChanged: E,
                                 RunResultView: u
-                            }) : (0, i.jsx)(l.xu, {
+                            }) : (0, r.jsx)(l.xu, {
                                 style: {
                                     contain: "layout"
                                 },
-                                children: d && (0, i.jsx)(d, {
+                                children: d && (0, r.jsx)(d, {
                                     params: p,
                                     onParamsChanged: b,
                                     setIsReadyToExecute: R
                                 })
                             })
-                        }), (0, i.jsx)(eV.m, {
-                            children: (0, i.jsxs)(a.k, {
+                        }), (0, r.jsx)(eV.m, {
+                            children: (0, r.jsxs)(a.k, {
                                 gap: "10px",
-                                children: [W && d && (0, i.jsx)(m.z, {
+                                children: [W && d && (0, r.jsx)(m.z, {
                                     colorScheme: "blue",
                                     onClick: handleReset,
                                     children: "Reset"
-                                }), W && (0, i.jsx)(i.Fragment, {
-                                    children: (0, i.jsx)(m.z, {
+                                }), W && (0, r.jsx)(r.Fragment, {
+                                    children: (0, r.jsx)(m.z, {
                                         colorScheme: "blue",
                                         onClick: K,
                                         children: "Add to checklist"
                                     })
-                                }), A && (0, i.jsx)(m.z, {
+                                }), A && (0, r.jsx)(m.z, {
                                     onClick: P,
                                     isDisabled: k,
                                     colorScheme: "blue",
                                     children: "Cancel"
-                                }), !W && !A && (0, i.jsx)(m.z, {
+                                }), !W && !A && (0, r.jsx)(m.z, {
                                     isDisabled: A || !_,
                                     colorScheme: "blue",
                                     onClick: B,
                                     children: "Execute"
-                                }), W && !d && (0, i.jsx)(m.z, {
+                                }), W && !d && (0, r.jsx)(m.z, {
                                     colorScheme: "blue",
                                     onClick: q,
                                     children: "Rerun"
                                 })]
                             })
                         })]
                     })]
@@ -2226,53 +2249,53 @@
                         index: t
                     }
                 }), n
             }
 
             function valuediff_getPrimaryKeyIndexes(e, n) {
                 let t = [];
-                for (let i of n) {
-                    let n = e.findIndex(e => e.name === i);
-                    if (n < 0) throw Error("Column ".concat(i, " not found"));
+                for (let r of n) {
+                    let n = e.findIndex(e => e.name === r);
+                    if (n < 0) throw Error("Column ".concat(r, " not found"));
                     t.push(n)
                 }
                 return t
             }
 
             function valuediff_getPrimaryKeyValue(e, n, t) {
-                let i = {};
+                let r = {};
                 if (0 === n.length) return JSON.stringify({
                     _index: t._index
                 });
-                for (let r of n) {
-                    let n = e[r];
-                    i[n.name] = t[r]
+                for (let i of n) {
+                    let n = e[i];
+                    r[n.name] = t[i]
                 }
-                return JSON.stringify(i)
+                return JSON.stringify(r)
             }
 
             function valuediff_DataFrameColumnGroupHeader(e) {
                 let {
                     name: n,
                     columnStatus: t,
-                    onPrimaryKeyChange: r,
+                    onPrimaryKeyChange: i,
                     onPinnedColumnsChange: o,
                     ...c
                 } = e, d = c.primaryKeys || [], u = c.pinnedColumns || [], h = d.includes(n), m = u.includes(n);
-                return "index" === n ? (0, i.jsx)(i.Fragment, {}) : (0, i.jsxs)(a.k, {
+                return "index" === n ? (0, r.jsx)(r.Fragment, {}) : (0, r.jsxs)(a.k, {
                     alignItems: "center",
                     gap: "10px",
                     className: "grid-header",
-                    children: [(0, i.jsx)(l.xu, {
+                    children: [(0, r.jsx)(l.xu, {
                         flex: 1,
                         overflow: "hidden",
                         textOverflow: "ellipsis",
                         whiteSpace: "nowrap",
                         children: n
-                    }), !h && o && (0, i.jsx)(s.J, {
+                    }), !h && o && (0, r.jsx)(s.J, {
                         className: m ? "unpin-icon" : "pin-icon",
                         display: m ? "block" : "none",
                         cursor: "pointer",
                         as: m ? L.$kI : L.oJP,
                         onClick: m ? () => {
                             let e = u.filter(e => e !== n);
                             o && o(e)
@@ -2283,213 +2306,215 @@
                     })]
                 })
             }
             let valuediff_defaultRenderCell = e => {
                 let {
                     row: n,
                     column: t
-                } = e, r = n[t.key];
-                return (0, i.jsx)(i.Fragment, {
-                    children: "boolean" == typeof r ? r.toString() : r
+                } = e, i = n[t.key];
+                return (0, r.jsx)(r.Fragment, {
+                    children: "boolean" == typeof i ? i.toString() : i
                 })
             };
 
             function toValueDiffGrid(e, n, t) {
-                let r = (null == t ? void 0 : t.pinnedColumns) || [],
+                let i = (null == t ? void 0 : t.pinnedColumns) || [],
                     l = (null == t ? void 0 : t.changedOnly) || !1,
                     o = [],
                     a = valuediff_getColumnMap(e),
                     s = {},
                     c = {};
                 if (0 === n.length) throw Error("Primary keys are required");
                 let d = valuediff_getPrimaryKeyIndexes(e.columns, n),
                     u = (a.in_a || a.IN_A).index,
                     h = (a.in_b || a.IN_B).index;
                 e.data.forEach((n, t) => {
-                    let i = valuediff_getPrimaryKeyValue(e.columns, d, n);
-                    n[u] && (s[i] = n), n[h] && (c[i] = n)
+                    let r = valuediff_getPrimaryKeyValue(e.columns, d, n);
+                    n[u] && (s[r] = n), n[h] && (c[r] = n)
                 });
                 let m = mergeKeysWithStatus(Object.keys(s), Object.keys(c)),
                     x = Object.entries(m).map(t => {
-                        let [i, r] = t, l = s[i], o = c[i], d = JSON.parse(i);
+                        let [r, i] = t, l = s[r], o = c[r], d = JSON.parse(r);
                         if (l && e.columns.forEach((e, t) => {
                                 n.includes(e.name) || (d["base__".concat(e.name)] = l[t])
                             }), o && e.columns.forEach((e, t) => {
                                 n.includes(e.name) || (d["current__".concat(e.name)] = o[t])
                             }), l) {
                             if (o)
                                 for (let [e, t] of Object.entries(a)) !("index" === e || n.includes(e)) && (eA().isEqual(l[t.index], o[t.index]) || (d.status = "modified", t.status = "modified"));
                             else d.status = "removed"
                         } else d.status = "added";
                         return d
                     });
                 l && (x = x.filter(e => "added" === e.status || "removed" === e.status || "modified" === e.status));
                 let toColumn = (e, n) => {
-                    let r = "added" === n ? "diff-header-added" : "removed" === n ? "diff-header-removed" : void 0,
+                    let i = "added" === n ? "diff-header-added" : "removed" === n ? "diff-header-removed" : void 0,
                         cellClass = t => {
-                            let i = t.status;
-                            if ("removed" === i) return "diff-cell-removed";
-                            if ("added" === i) return "diff-cell-added";
+                            let r = t.status;
+                            if ("removed" === r) return "diff-cell-removed";
+                            if ("added" === r) return "diff-cell-added";
                             if ("added" === n);
                             else if ("removed" === n);
                             else if (!eA().isEqual(t["base__".concat(e)], t["current__".concat(e)])) return "diff-cell-modified"
                         };
                     return {
-                        headerCellClass: r,
-                        name: (0, i.jsx)(valuediff_DataFrameColumnGroupHeader, {
+                        headerCellClass: i,
+                        name: (0, r.jsx)(valuediff_DataFrameColumnGroupHeader, {
                             name: e,
                             columnStatus: n,
                             ...t
                         }),
                         children: [{
                             key: "base__".concat(e),
                             name: "Base",
-                            renderEditCell: ev.Ug,
-                            headerCellClass: r,
+                            renderEditCell: ej.Ug,
+                            headerCellClass: i,
                             cellClass,
                             renderCell: valuediff_defaultRenderCell,
                             size: "auto"
                         }, {
                             key: "current__".concat(e),
                             name: "Current",
-                            renderEditCell: ev.Ug,
-                            headerCellClass: r,
+                            renderEditCell: ej.Ug,
+                            headerCellClass: i,
                             cellClass,
                             renderCell: valuediff_defaultRenderCell,
                             size: "auto"
                         }]
                     }
                 };
                 return n.forEach(e => {
                     let n = a[e].status || "";
                     o.push({
                         key: "".concat(e),
-                        name: (0, i.jsx)(valuediff_DataFrameColumnGroupHeader, {
+                        name: (0, r.jsx)(valuediff_DataFrameColumnGroupHeader, {
                             name: e,
                             columnStatus: n,
                             ...t
                         }),
                         frozen: !0,
                         cellClass: e => {
                             if (e.status) return "diff-header-".concat(e.status)
                         }
                     })
-                }), r.forEach(e => {
+                }), i.forEach(e => {
                     let t = a[e].status || "";
                     n.includes(e) || o.push(toColumn(e, t))
                 }), Object.entries(a).forEach(e => {
-                    let [t, i] = e, a = i.status || "";
-                    "in_a" === t || "in_b" === t || n.includes(t) || r.includes(t) || l && "added" !== a && "removed" !== a && "modified" !== a || o.push(toColumn(t, a))
+                    let [t, r] = e, a = r.status || "";
+                    "in_a" === t || "in_b" === t || n.includes(t) || i.includes(t) || l && "added" !== a && "removed" !== a && "modified" !== a || o.push(toColumn(t, a))
                 }), {
                     columns: o,
                     rows: x
                 }
             }
             let ValueDiffDetailResultView = e => {
                 var n, t;
                 let {
-                    run: r,
+                    run: i,
                     onAddToChecklist: s,
                     viewOptions: c,
                     onViewOptionsChanged: d
                 } = e, h = (0, S.useMemo)(() => (null == c ? void 0 : c.changed_only) || !1, [c]), m = (0, S.useMemo)(() => (null == c ? void 0 : c.pinned_columns) || [], [c]), x = (0, S.useMemo)(() => {
                     var e, n;
-                    if (!r.result) return {
+                    if (!i.result) return {
                         columns: [],
                         rows: []
                     };
-                    let t = (null == r ? void 0 : null === (e = r.params) || void 0 === e ? void 0 : e.primary_key) ? [null == r ? void 0 : null === (n = r.params) || void 0 === n ? void 0 : n.primary_key] : [];
-                    return toValueDiffGrid(null == r ? void 0 : r.result, t, {
+                    let t = (null == i ? void 0 : null === (e = i.params) || void 0 === e ? void 0 : e.primary_key) ? [null == i ? void 0 : null === (n = i.params) || void 0 === n ? void 0 : n.primary_key] : [];
+                    return toValueDiffGrid(null == i ? void 0 : i.result, t, {
                         changedOnly: h,
                         pinnedColumns: m,
                         onPinnedColumnsChange: e => {
                             d && d({
                                 ...c,
                                 pinned_columns: e
                             })
                         }
                     })
-                }, [r, c, h, m, d]);
-                if (0 === x.columns.length) return (0, i.jsx)(u.M, {
+                }, [i, c, h, m, d]);
+                if (0 === x.columns.length) return (0, r.jsx)(u.M, {
                     height: "100%",
                     children: "No data"
                 });
-                if (h && 0 === x.rows.length) return (0, i.jsx)(u.M, {
+                if (h && 0 === x.rows.length) return (0, r.jsx)(u.M, {
                     height: "100%",
                     children: "No change"
                 });
-                let f = (null === (n = r.result) || void 0 === n ? void 0 : n.limit) || 0,
-                    p = f > 0 && (null == r ? void 0 : null === (t = r.result) || void 0 === t ? void 0 : t.more) ? "Warning: Displayed results are limited to ".concat(f.toLocaleString(), " records. To ensure complete data retrieval, consider applying a LIMIT or WHERE clause to constrain the result set.") : null;
-                return (0, i.jsxs)(a.k, {
+                let f = (null === (n = i.result) || void 0 === n ? void 0 : n.limit) || 0,
+                    p = f > 0 && (null == i ? void 0 : null === (t = i.result) || void 0 === t ? void 0 : t.more) ? "Warning: Displayed results are limited to ".concat(f.toLocaleString(), " records. To ensure complete data retrieval, consider applying a LIMIT or WHERE clause to constrain the result set.") : null;
+                return (0, r.jsxs)(a.k, {
                     direction: "column",
                     backgroundColor: "rgb(249, 249, 249)",
                     height: "100%",
-                    children: [(0, i.jsxs)(a.k, {
+                    children: [(0, r.jsxs)(a.k, {
                         borderBottom: "1px solid lightgray",
                         justifyContent: "flex-end",
                         gap: "5px",
                         alignItems: "center",
                         px: "10px",
                         bg: p ? "orange.100" : "inherit",
-                        children: [p && (0, i.jsxs)(i.Fragment, {
-                            children: [(0, i.jsx)(ei.a, {
+                        children: [p && (0, r.jsxs)(r.Fragment, {
+                            children: [(0, r.jsx)(er.a, {
                                 color: "orange.600"
-                            }), " ", (0, i.jsx)(l.xu, {
+                            }), " ", (0, r.jsx)(l.xu, {
                                 children: p
                             })]
-                        }), (0, i.jsx)(E.L, {
+                        }), (0, r.jsx)(E.L, {
                             minHeight: "32px"
-                        }), (0, i.jsx)(eM.X, {
+                        }), (0, r.jsx)(eF.X, {
                             isChecked: null == c ? void 0 : c.changed_only,
                             onChange: () => {
                                 let e = !(null == c ? void 0 : c.changed_only);
                                 d && d({
                                     ...c,
                                     changed_only: e
                                 })
                             },
                             children: "Changed only"
-                        }), s && (0, i.jsx)(o.u, {
+                        }), s && (0, r.jsx)(o.u, {
                             label: "Add to Checklist",
-                            children: (0, i.jsx)(P.h, {
+                            children: (0, r.jsx)(P.h, {
                                 variant: "unstyled",
                                 size: "sm",
                                 "aria-label": "Add",
-                                icon: (0, i.jsx)(eq.d, {}),
-                                onClick: () => s(r)
+                                icon: (0, r.jsx)(eq.d, {}),
+                                onClick: () => s(i)
                             })
                         })]
-                    }), (0, i.jsx)(ScreenshotDataGrid, {
+                    }), (0, r.jsx)(ScreenshotDataGrid, {
                         style: {
                             blockSize: "auto",
                             maxHeight: "100%",
                             overflow: "auto"
                         },
                         columns: x.columns,
                         rows: x.rows,
+                        renderers: {
+                            noRowsFallback: (0, r.jsx)(EmptyRowsRenderer, {})
+                        },
                         defaultColumnOptions: {
                             resizable: !0,
                             maxWidth: 800,
                             minWidth: 35
                         },
                         className: "rdg-light",
                         enableScreenshot: !0
                     })]
                 })
             };
-            var eH = t(17180),
-                eK = t(34030);
+            var eH = t(34030);
 
             function formatNumber(e) {
                 let n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "en-US",
                     t = arguments.length > 2 ? arguments[2] : void 0;
                 return "number" != typeof e ? e : new Intl.NumberFormat(n, t).format(e)
             }
 
-            function formatIntervalMinMax(e) {
+            function formatters_formatIntervalMinMax(e) {
                 let n = e > 0 && e <= .001,
                     t = e < 1 && e >= .999,
                     formatter = function() {
                         let n = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : e;
                         return formatNumber(n, "en-US", {
                             style: "percent",
                             minimumFractionDigits: 1
@@ -2502,32 +2527,32 @@
                 if (t) {
                     let e = formatter(.999);
                     return ">".concat(e)
                 }
                 return formatter()
             }
 
-            function formatAsAbbreviatedNumber(e) {
+            function formatters_formatAsAbbreviatedNumber(e) {
                 if ("number" != typeof e) return e;
                 {
                     let n = Math.abs(e),
                         t = n >= .01,
-                        i = n >= 1e6,
-                        r = n >= 1e9,
+                        r = n >= 1e6,
+                        i = n >= 1e9,
                         l = n >= 1e15;
                     if (l || n >= 1e12) return new Intl.NumberFormat("en-US", {
                         style: "unit",
                         unit: "liter",
                         unitDisplay: "narrow",
                         maximumFractionDigits: l ? 0 : 2
                     }).format(e / 1e12).replace("L", "T");
-                    if (r || i || n >= 1e3) {
+                    if (i || r || n >= 1e3) {
                         let n = {
-                            base: r ? 1e9 : i ? 1e6 : 1e3,
-                            unit: r ? "B" : i ? "M" : "K"
+                            base: i ? 1e9 : r ? 1e6 : 1e3,
+                            unit: i ? "B" : r ? "M" : "K"
                         };
                         return new Intl.NumberFormat("en-US", {
                             style: "unit",
                             unit: "liter",
                             unitDisplay: "narrow",
                             maximumFractionDigits: 1
                         }).format(e / n.base).replace("L", n.unit)
@@ -2536,105 +2561,197 @@
                         maximumFractionDigits: 2
                     }).format(e) : new Intl.NumberFormat("en-US", {
                         maximumFractionDigits: t ? 3 : 2,
                         notation: t || 0 === n ? "standard" : "scientific"
                     }).format(e)
                 }
             }
-            var eW = t(85670),
+            var eK = t(17180),
+                eW = t(85670),
                 eU = t(84021);
+            let eG = "#63B3ED",
+                eQ = "#F6AD55",
+                eJ = "".concat(eG, "A5"),
+                eZ = "".concat(eQ, "A5");
 
-            function TopKSummaryList(e) {
+            function SquareIcon(e) {
                 let {
-                    topk: n,
-                    valids: t,
-                    isDisplayTopTen: r
-                } = e, s = r ? 10 : n.counts.length, c = n.counts.slice(0, s), d = t - c.reduce((e, n) => e + n, 0);
-                return (0, i.jsx)(l.xu, {
+                    color: n
+                } = e;
+                return (0, r.jsx)(l.xu, {
+                    display: "inline-block",
+                    w: "10px",
+                    h: "10px",
+                    bgColor: n,
+                    mr: "2",
+                    borderRadius: "sm"
+                })
+            }
+            let eX = "#63B3ED";
+
+            function prepareSummaryList(e, n) {
+                let t = n ? 10 : e.counts.length,
+                    r = e.counts.slice(0, t),
+                    i = e.valids - r.reduce((e, n) => e + n, 0),
+                    l = e.values.slice(0, t);
+                return l.concat([i]).map((n, t) => {
+                    let l = t === r.length,
+                        o = l ? i : r[t];
+                    return {
+                        isLastItemOthers: l,
+                        label: l ? "(others)" : String(n) || "(empty)",
+                        count: o,
+                        displayCount: formatters_formatAsAbbreviatedNumber(o),
+                        displayRatio: formatters_formatIntervalMinMax(o / e.valids) || "N/A"
+                    }
+                })
+            }
+
+            function TopKChartTooltip(e) {
+                let {
+                    base: n,
+                    current: t,
+                    children: i
+                } = e;
+                return (0, r.jsx)(o.u, {
+                    label: (0, r.jsxs)(l.xu, {
+                        children: [(0, r.jsxs)(f.x, {
+                            children: [(0, r.jsx)(SquareIcon, {
+                                color: eG
+                            }), "Current: ", t.count, " (", t.displayRatio, ")"]
+                        }), (0, r.jsxs)(f.x, {
+                            children: [(0, r.jsx)(SquareIcon, {
+                                color: eQ
+                            }), "Base: ", n.count, " (", n.displayRatio, ")"]
+                        })]
+                    }),
+                    placement: "auto",
+                    hasArrow: !0,
+                    children: i
+                })
+            }
+
+            function TopKSummaryBarChart(e) {
+                let {
+                    topKDiff: n,
+                    isDisplayTopTen: t
+                } = e, i = prepareSummaryList(n.current, t), o = prepareSummaryList(n.base, t);
+                return (0, r.jsxs)(l.xu, {
                     w: "100%",
-                    children: c.concat([d]).map((e, r) => {
-                        let l = r === c.length,
-                            s = l ? d : e,
-                            u = String(n.values[r]),
-                            h = l ? "(others)" : u || "(empty)",
-                            m = formatAsAbbreviatedNumber(s),
-                            x = formatIntervalMinMax(s / t);
-                        return (0, i.jsx)(S.Fragment, {
-                            children: !l || l && s > 0 ? (0, i.jsxs)(i.Fragment, {
-                                children: [(0, i.jsxs)(a.k, {
+                    px: 20,
+                    py: 4,
+                    children: [(0, r.jsxs)(a.k, {
+                        alignItems: "center",
+                        direction: "row",
+                        children: [(0, r.jsx)(E.L, {}), (0, r.jsxs)(f.x, {
+                            as: "h3",
+                            size: "sm",
+                            p: "2",
+                            color: "gray",
+                            children: [(0, r.jsx)(SquareIcon, {
+                                color: eQ
+                            }), " Base"]
+                        }), (0, r.jsxs)(f.x, {
+                            as: "h3",
+                            size: "sm",
+                            p: "2",
+                            color: "gray",
+                            children: [(0, r.jsx)(SquareIcon, {
+                                color: eG
+                            }), " Current"]
+                        }), (0, r.jsx)(E.L, {})]
+                    }), i.map((e, t) => {
+                        let i = o[t];
+                        return e.isLastItemOthers && 0 === e.count && 0 === i.count ? (0, r.jsx)(r.Fragment, {}) : (0, r.jsxs)(S.Fragment, {
+                            children: [(0, r.jsx)(TopKChartTooltip, {
+                                base: i,
+                                current: e,
+                                children: (0, r.jsxs)(a.k, {
                                     alignItems: "center",
                                     width: "100%",
                                     _hover: {
                                         bg: "blackAlpha.300"
                                     },
-                                    px: 3,
-                                    children: [(0, i.jsx)(o.u, {
-                                        label: h,
-                                        placement: "start",
-                                        children: (0, i.jsx)(f.x, {
-                                            noOfLines: 1,
-                                            width: "14em",
-                                            fontSize: "sm",
-                                            color: l || 0 === u.length ? "gray.400" : "inherit",
-                                            children: h
-                                        })
-                                    }), (0, i.jsx)(a.k, {
-                                        height: "2em",
+                                    px: 4,
+                                    children: [(0, r.jsx)(f.x, {
+                                        noOfLines: 1,
                                         width: "10em",
-                                        children: (0, i.jsx)(CategoricalBarChart, {
-                                            topkCount: s,
-                                            topkLabel: h,
-                                            valids: t
-                                        })
-                                    }), (0, i.jsx)(o.u, {
-                                        label: m,
-                                        placement: "start",
-                                        children: (0, i.jsx)(f.x, {
-                                            ml: 5,
-                                            mr: 2,
-                                            fontSize: "sm",
-                                            width: "4em",
-                                            noOfLines: 1,
-                                            children: m
-                                        })
-                                    }), (0, i.jsx)(o.u, {
-                                        label: x,
-                                        placement: "start",
-                                        children: (0, i.jsx)(f.x, {
-                                            color: "gray.400",
-                                            fontSize: "sm",
-                                            width: "4em",
-                                            children: x
-                                        })
+                                        fontSize: "sm",
+                                        color: e.isLastItemOthers || 0 === e.label.length ? "gray.400" : "inherit",
+                                        children: e.label
+                                    }), (0, r.jsxs)(a.k, {
+                                        width: "70%",
+                                        direction: "column",
+                                        children: [(0, r.jsxs)(a.k, {
+                                            height: "1em",
+                                            children: [(0, r.jsx)(CategoricalBarChart, {
+                                                topkCount: e.count,
+                                                topkLabel: e.label,
+                                                valids: n.current.valids,
+                                                color: eG
+                                            }), (0, r.jsx)(f.x, {
+                                                ml: 5,
+                                                mr: 2,
+                                                fontSize: "sm",
+                                                width: "6em",
+                                                children: e.displayCount
+                                            }), (0, r.jsx)(f.x, {
+                                                color: "gray.400",
+                                                fontSize: "sm",
+                                                width: "4em",
+                                                children: e.displayRatio
+                                            })]
+                                        }), (0, r.jsxs)(a.k, {
+                                            height: "1em",
+                                            children: [(0, r.jsx)(CategoricalBarChart, {
+                                                topkCount: i.count,
+                                                topkLabel: i.label,
+                                                valids: n.base.valids,
+                                                color: eQ
+                                            }), (0, r.jsx)(f.x, {
+                                                ml: 5,
+                                                mr: 2,
+                                                fontSize: "sm",
+                                                width: "6em",
+                                                children: i.displayCount
+                                            }), (0, r.jsx)(f.x, {
+                                                color: "gray.400",
+                                                fontSize: "sm",
+                                                width: "4em",
+                                                children: i.displayRatio
+                                            })]
+                                        })]
                                     })]
-                                }), (0, i.jsx)(eH.i, {})]
-                            }) : (0, i.jsx)(i.Fragment, {})
-                        }, r)
-                    })
+                                })
+                            }), (0, r.jsx)(eK.i, {})]
+                        }, t)
+                    })]
                 })
             }
 
             function CategoricalBarChart(e) {
                 let {
                     topkCount: n,
                     topkLabel: t,
-                    valids: r,
-                    animation: l = !1
+                    valids: i,
+                    animation: l = !1,
+                    color: o = eX
                 } = e;
                 eW.kL.register(eW.uw, eW.ZL, eW.f$);
-                let o = getCatBarChartOptions(n, r, {
+                let a = getCatBarChartOptions(n, i, {
                         animation: l
                     }),
-                    a = getCatBarChartData({
+                    s = getCatBarChartData({
                         topkCount: n,
-                        topkLabel: t
+                        topkLabel: t,
+                        color: o
                     });
-                return (0, i.jsx)(eU.$Q, {
-                    data: a,
-                    options: o,
+                return (0, r.jsx)(eU.$Q, {
+                    data: s,
+                    options: a,
                     plugins: []
                 })
             }
 
             function getCatBarChartOptions(e, n) {
                 let {
                     ...t
@@ -2663,249 +2780,263 @@
                     ...t
                 }
             }
 
             function getCatBarChartData(e) {
                 let {
                     topkLabel: n,
-                    topkCount: t
+                    topkCount: t,
+                    color: r = eX
                 } = e;
                 return {
                     labels: [n],
                     datasets: [{
                         indexAxis: "y",
                         data: [t],
-                        backgroundColor: "#63B3ED",
-                        hoverBackgroundColor: "#002a53",
-                        borderWidth: 1,
-                        borderColor: "#002a53",
+                        backgroundColor: r,
+                        hoverBackgroundColor: r,
+                        borderWidth: 0,
+                        borderColor: r,
                         barPercentage: 1,
                         categoryPercentage: .6
                     }]
                 }
             }
             let ScreenshotBox = e => {
                 let {
                     backgroundColor: n = "white",
                     blockSize: t,
-                    children: r,
+                    children: i,
                     ...o
                 } = e, {
                     ref: a,
                     CopyToClipboardButton: s
                 } = useCopyToClipboardButton({
                     backgroundColor: n
                 });
-                return (0, i.jsxs)(i.Fragment, {
-                    children: [(0, i.jsx)(l.xu, {
+                return (0, r.jsxs)(r.Fragment, {
+                    children: [(0, r.jsx)(l.xu, {
                         ref: a,
                         ...o,
                         overflow: "auto",
-                        children: (0, i.jsx)(l.xu, {
+                        children: (0, r.jsx)(l.xu, {
                             backgroundColor: n,
                             height: "100%",
                             blockSize: t,
-                            children: r
+                            children: i
                         })
-                    }), (0, i.jsx)(s, {
+                    }), (0, r.jsx)(s, {
                         imageType: "png"
                     })]
                 })
             };
 
             function TopKDiffResultView(e) {
                 let {
                     run: n
-                } = e, [t, r] = (0, S.useState)(!0), o = n.result, s = n.params, c = o.base, d = o.current;
-                return (0, i.jsxs)(a.k, {
+                } = e, [t, i] = (0, S.useState)(!0), l = n.result, o = n.params, s = l.base, c = l.current;
+                return (0, r.jsxs)(a.k, {
                     direction: "column",
                     height: "100%",
-                    children: [(0, i.jsxs)(ScreenshotBox, {
+                    children: [(0, r.jsxs)(ScreenshotBox, {
                         blockSize: "auto",
-                        children: [(0, i.jsxs)(ea.X, {
+                        children: [(0, r.jsxs)(ea.X, {
                             as: "h1",
                             size: "md",
                             paddingTop: 4,
                             textAlign: "center",
-                            children: ["Model ", s.model, ".", s.column_name]
-                        }), (0, i.jsxs)(x.U, {
-                            children: [(0, i.jsx)(E.L, {}), (0, i.jsxs)(l.xu, {
-                                children: [(0, i.jsx)(ea.X, {
-                                    as: "h3",
-                                    size: "sm",
-                                    m: "2",
-                                    color: "gray",
-                                    children: "Base"
-                                }), (0, i.jsx)(eH.i, {}), (0, i.jsx)(TopKSummaryList, {
-                                    topk: c,
-                                    valids: c.valids || 0,
-                                    isDisplayTopTen: t
-                                })]
-                            }), (0, i.jsxs)(l.xu, {
-                                children: [(0, i.jsx)(ea.X, {
-                                    as: "h3",
-                                    size: "sm",
-                                    m: "2",
-                                    color: "gray",
-                                    children: "Current"
-                                }), (0, i.jsx)(eH.i, {}), (0, i.jsx)(TopKSummaryList, {
-                                    topk: d,
-                                    valids: d.valids || 0,
-                                    isDisplayTopTen: t
-                                })]
-                            }), (0, i.jsx)(E.L, {})]
+                            children: ["Model ", o.model, ".", o.column_name]
+                        }), (0, r.jsxs)(x.U, {
+                            children: [(0, r.jsx)(E.L, {}), (0, r.jsx)(TopKSummaryBarChart, {
+                                topKDiff: l,
+                                valids: c.valids || 0,
+                                isDisplayTopTen: t
+                            }), (0, r.jsx)(E.L, {})]
                         })]
-                    }), (0, i.jsx)(E.L, {}), (c.values.length > 10 || d.values.length > 10) && (0, i.jsx)(a.k, {
+                    }), (0, r.jsx)(E.L, {}), (s.values.length > 10 || c.values.length > 10) && (0, r.jsx)(a.k, {
                         p: 5,
                         justify: "start",
-                        children: (0, i.jsx)(eK.r, {
-                            onClick: () => r(e => !e),
+                        children: (0, r.jsx)(eH.r, {
+                            onClick: () => i(e => !e),
                             textColor: "blue.500",
                             children: t ? "View More Items" : "View Only Top-10"
                         })
                     })]
                 })
             }
-            var eG = t(68665);
+            var eY = t(68665);
 
             function TopKDiffForm(e) {
                 var n;
                 let {
                     params: t,
-                    onParamsChanged: r,
+                    onParamsChanged: i,
                     setIsReadyToExecute: o
                 } = e, a = useLineageGraphsContext(), s = eA().find(null === (n = a.lineageGraphSets) || void 0 === n ? void 0 : n.all.nodes, {
                     name: null == t ? void 0 : t.model
                 }), c = s ? extractColumnNames(s) : [];
                 return (0, S.useEffect)(() => {
                     o(!!t.column_name)
-                }, [t, o]), (0, i.jsx)(l.xu, {
+                }, [t, o]), (0, r.jsx)(l.xu, {
                     m: "16px",
-                    children: (0, i.jsxs)(eL.NI, {
-                        children: [(0, i.jsx)(eI.l, {
+                    children: (0, r.jsxs)(eL.NI, {
+                        children: [(0, r.jsx)(eI.l, {
                             children: "Pick a column to show top-k"
-                        }), (0, i.jsx)(eG.P, {
+                        }), (0, r.jsx)(eY.P, {
                             placeholder: "Select column",
                             value: null == t ? void 0 : t.column_name,
                             onChange: e => {
                                 let n = e.target.value;
-                                r({
+                                i({
                                     ...t,
                                     column_name: n
                                 })
                             },
-                            children: c.map(e => (0, i.jsx)("option", {
+                            children: c.map(e => (0, r.jsx)("option", {
                                 value: e,
                                 children: e
                             }, e))
                         })]
                     })
                 })
             }
 
             function HistogramChart(e) {
                 let {
                     data: n,
                     hideAxis: t = !1,
-                    animation: r = !1
+                    animation: i = !1
                 } = e;
                 eW.kL.register(eW.ZL, eW.RM, eW.f$, eW.uw, eW.u);
                 let l = getHistogramChartOptions(n, t, {
-                        animation: r
+                        animation: i
                     }),
                     o = getHistogramChartData(n);
-                return (0, i.jsx)(eU.kL, {
-                    type: "bar",
-                    options: l,
-                    data: o,
-                    plugins: []
+                return (0, r.jsxs)(r.Fragment, {
+                    children: [(0, r.jsxs)(a.k, {
+                        alignItems: "center",
+                        direction: "row",
+                        children: [(0, r.jsx)(E.L, {}), (0, r.jsxs)(f.x, {
+                            as: "h3",
+                            size: "sm",
+                            p: "2",
+                            color: "gray",
+                            children: [(0, r.jsx)(SquareIcon, {
+                                color: eZ
+                            }), " Base"]
+                        }), (0, r.jsxs)(f.x, {
+                            as: "h3",
+                            size: "sm",
+                            p: "2",
+                            color: "gray",
+                            children: [(0, r.jsx)(SquareIcon, {
+                                color: eJ
+                            }), " Current"]
+                        }), (0, r.jsx)(E.L, {})]
+                    }), (0, r.jsx)(eU.kL, {
+                        type: "bar",
+                        options: l,
+                        data: o,
+                        plugins: []
+                    })]
                 })
             }
 
+            function getHistogramChartDataset(e, n, t, r, i) {
+                let {
+                    counts: l = []
+                } = i, o = "datetime" === e ? l.map((e, t) => ({
+                    x: n[t],
+                    y: e
+                })) : l;
+                return {
+                    label: t,
+                    data: o,
+                    backgroundColor: r,
+                    borderColor: r,
+                    hoverBackgroundColor: r,
+                    borderWidth: 0,
+                    categoryPercentage: 1,
+                    barPercentage: 1,
+                    xAxisID: "x"
+                }
+            }
+
             function getHistogramChartData(e) {
                 let {
-                    histogram: n,
+                    datasets: n,
                     type: t,
-                    binEdges: i
-                } = e, {
-                    counts: r = []
-                } = n || {}, l = "datetime" === t ? r.map((e, n) => ({
-                    x: i[n],
-                    y: e
-                })) : r, o = i.map((e, n) => formatDisplayedBinItem(i, n)).slice(0, -1);
+                    binEdges: r
+                } = e, [i, l] = n, o = getHistogramChartDataset(t, r, "Current", eJ, l), a = getHistogramChartDataset(t, r, "Base", eZ, i), s = r.map((e, n) => formatDisplayedBinItem(r, n)).slice(0, -1);
                 return {
-                    labels: o,
-                    datasets: [{
-                        label: "counts",
-                        data: l,
-                        backgroundColor: "#63B3ED",
-                        borderColor: "#4299E1",
-                        hoverBackgroundColor: "#002A53",
-                        borderWidth: 1,
-                        categoryPercentage: 1,
-                        barPercentage: 1,
-                        xAxisID: "x"
-                    }]
+                    labels: s,
+                    datasets: [o, a]
                 }
             }
 
             function getHistogramChartOptions(e) {
                 let n = arguments.length > 1 && void 0 !== arguments[1] && arguments[1],
                     {
                         ...t
                     } = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {},
                     {
-                        histogram: i,
-                        type: r,
+                        datasets: r,
+                        type: i,
                         samples: l = 0,
                         binEdges: o
                     } = e,
-                    {
-                        counts: a = []
-                    } = i || {},
-                    s = "datetime" === r;
+                    [a, s] = r,
+                    c = "datetime" === i;
                 return {
                     responsive: !0,
                     maintainAspectRatio: !1,
                     plugins: {
                         tooltip: {
                             mode: "index",
-                            position: "nearest",
                             intersect: !1,
                             callbacks: {
                                 title(e) {
                                     let [{
-                                        dataIndex: n
-                                    }] = e, t = formatDisplayedBinItem(o, n), i = formatIntervalMinMax(a[n] / l);
-                                    return "".concat(s ? "Date Range" : "string" === r ? "Text Length" : "Value Range", "\n").concat(t, "\n(").concat(i, ")")
+                                        dataIndex: n,
+                                        datasetIndex: t
+                                    }] = e, r = formatDisplayedBinItem(o, n);
+                                    return "".concat(c ? "Date Range" : "string" === i ? "Text Length" : "Value Range", "\n").concat(r)
+                                },
+                                label(e) {
+                                    let {
+                                        datasetIndex: n,
+                                        dataIndex: t,
+                                        dataset: {
+                                            label: r
+                                        }
+                                    } = e, i = 0 === n ? s.counts : a.counts, o = formatters_formatIntervalMinMax(i[t] / l), c = i[t];
+                                    return "".concat(r, ": ").concat(c, " (").concat(o, ")")
                                 }
                             }
                         }
                     },
                     scales: getScales(e, n),
                     ...t
                 }
             }
 
             function getScales(e) {
                 let {
-                    histogram: n,
+                    datasets: n,
                     min: t = 0,
-                    max: i = 0,
-                    type: r,
+                    max: r = 0,
+                    type: i,
                     binEdges: l
-                } = e, o = arguments.length > 1 && void 0 !== arguments[1] && arguments[1], {
-                    counts: a = []
-                } = n || {}, s = l.map((e, n) => formatDisplayedBinItem(l, n)).slice(0, -1);
+                } = e, o = arguments.length > 1 && void 0 !== arguments[1] && arguments[1], [a, s] = n, c = Math.max(...s.counts, ...a.counts), d = l.map((e, n) => formatDisplayedBinItem(l, n)).slice(0, -1);
                 return {
-                    x: "datetime" === r ? {
+                    x: "datetime" === i ? {
                         display: !o,
                         type: "timeseries",
                         min: t,
-                        max: i,
+                        max: r,
                         adapters: {
                             date: {}
                         },
                         time: {
                             minUnit: "day"
                         },
                         grid: {
@@ -2919,107 +3050,83 @@
                     } : {
                         display: !o,
                         type: "category",
                         grid: {
                             display: !1
                         },
                         ticks: {
-                            callback: (e, n) => s[n]
-                        }
+                            callback: (e, n) => d[n]
+                        },
+                        stacked: !0
                     },
                     y: {
                         display: !o,
                         type: "linear",
-                        max: Math.max(...a),
+                        max: c,
                         border: {
                             dash: [2, 2]
                         },
                         grid: {
                             color: "lightgray"
                         },
                         ticks: {
                             maxTicksLimit: 8,
                             callback: function(e, n) {
-                                return formatAsAbbreviatedNumber(e)
+                                return formatters_formatAsAbbreviatedNumber(e)
                             }
-                        }
+                        },
+                        beginAtZero: !0
                     }
                 }
             }
 
             function formatDisplayedBinItem(e, n) {
                 let t = e[n],
-                    i = e[n + 1],
-                    r = formatAsAbbreviatedNumber(t),
-                    l = formatAsAbbreviatedNumber(i),
-                    o = "".concat(r, " - ").concat(l);
+                    r = e[n + 1],
+                    i = formatters_formatAsAbbreviatedNumber(t),
+                    l = formatters_formatAsAbbreviatedNumber(r),
+                    o = "".concat(i, " - ").concat(l);
                 return o
             }
 
             function HistogramDiffResultView(e) {
-                var n, t, r, o, s, c, d;
+                var n, t, i, o, s, c;
                 let {
-                    run: u
-                } = e, h = u.params, m = null === (n = u.result) || void 0 === n ? void 0 : n.base, f = null === (t = u.result) || void 0 === t ? void 0 : t.current, p = null === (r = u.result) || void 0 === r ? void 0 : r.min, g = null === (o = u.result) || void 0 === o ? void 0 : o.max, v = null === (s = u.result) || void 0 === s ? void 0 : s.bin_edges;
-                return m && f ? (0, i.jsx)(a.k, {
+                    run: d
+                } = e, u = d.params, h = null === (n = d.result) || void 0 === n ? void 0 : n.base, m = null === (t = d.result) || void 0 === t ? void 0 : t.current, f = null === (i = d.result) || void 0 === i ? void 0 : i.min, p = null === (o = d.result) || void 0 === o ? void 0 : o.max, g = null === (s = d.result) || void 0 === s ? void 0 : s.bin_edges;
+                return h && m ? (0, r.jsx)(a.k, {
                     direction: "column",
                     height: "500px",
-                    children: (0, i.jsxs)(ScreenshotBox, {
+                    children: (0, r.jsxs)(ScreenshotBox, {
                         height: "100%",
-                        children: [(0, i.jsxs)(ea.X, {
+                        children: [(0, r.jsxs)(ea.X, {
                             as: "h1",
                             size: "md",
                             paddingTop: "4",
                             textAlign: "center",
-                            children: ["Model ", h.model, ".", h.column_name]
-                        }), (0, i.jsxs)(x.U, {
-                            children: [(0, i.jsx)(E.L, {}), (0, i.jsxs)(l.xu, {
-                                w: "40%",
+                            children: ["Model ", u.model, ".", u.column_name]
+                        }), (0, r.jsxs)(x.U, {
+                            children: [(0, r.jsx)(E.L, {}), (0, r.jsx)(l.xu, {
+                                w: "80%",
                                 h: "300px",
                                 m: "4",
-                                children: [(0, i.jsx)(ea.X, {
-                                    as: "h3",
-                                    size: "sm",
-                                    m: "2",
-                                    color: "gray",
-                                    children: "Base"
-                                }), (0, i.jsx)(HistogramChart, {
+                                children: (0, r.jsx)(HistogramChart, {
                                     data: {
-                                        type: (null === (c = u.params) || void 0 === c ? void 0 : c.column_type) || "",
-                                        histogram: m,
-                                        min: p,
-                                        max: g,
-                                        samples: m.total,
-                                        binEdges: v
+                                        type: (null === (c = d.params) || void 0 === c ? void 0 : c.column_type) || "",
+                                        datasets: [m, h],
+                                        min: f,
+                                        max: p,
+                                        samples: h.total,
+                                        binEdges: g
                                     }
-                                })]
-                            }), (0, i.jsxs)(l.xu, {
-                                w: "40%",
-                                h: "300px",
-                                m: "4",
-                                children: [(0, i.jsx)(ea.X, {
-                                    as: "h3",
-                                    size: "sm",
-                                    m: "2",
-                                    color: "gray",
-                                    children: "Current"
-                                }), (0, i.jsx)(HistogramChart, {
-                                    data: {
-                                        type: (null === (d = u.params) || void 0 === d ? void 0 : d.column_type) || "",
-                                        histogram: f,
-                                        min: p,
-                                        max: g,
-                                        samples: f.total,
-                                        binEdges: v
-                                    }
-                                })]
-                            }), (0, i.jsx)(E.L, {})]
+                                })
+                            }), (0, r.jsx)(E.L, {})]
                         })]
                     })
-                }) : (0, i.jsx)("div", {
+                }) : (0, r.jsx)("div", {
                     children: "Loading..."
                 })
             }
 
             function isStringDataType(e) {
                 return ["CHAR", "VARCHAR", "TINYTEXT", "TEXT", "MEDIUMTEXT", "LONGTEXT", "NCHAR", "NVARCHAR", "VARCHAR2", "NVARCHAR2", "CLOB", "NCLOB", "VARCHAR(MAX)", "XML", "JSON", "BOOLEAN", "TINYINT(1)", "BIT", "NUMBER(1)", "BOOL"].includes(e.toUpperCase())
             }
@@ -3028,50 +3135,50 @@
                 return ["DATE", "DATETIME", "TIMESTAMP", "TIME", "YEAR", "DATETIME2", "SMALLDATETIME", "DATETIMEOFFSET", "INTERVAL", "TIMESTAMPTZ", "TIMETZ", "TIMESTAMP WITH TIME ZONE", "TIMESTAMP WITH LOCAL TIME ZONE", "TIMESTAMP_LTZ", "TIMESTAMP_NTZ", "TIMESTAMP_TZ"].includes(e.toUpperCase())
             }
 
             function HistogramDiffForm(e) {
                 var n;
                 let {
                     params: t,
-                    onParamsChanged: r,
+                    onParamsChanged: i,
                     setIsReadyToExecute: o
                 } = e, a = useLineageGraphsContext(), s = eA().find(null === (n = a.lineageGraphSets) || void 0 === n ? void 0 : n.all.nodes, {
                     name: null == t ? void 0 : t.model
                 }), c = s ? extractColumns(s).filter(e => !isStringDataType(e.type) && !isDateTimeType(e.type)) : [];
-                return (0, i.jsx)(l.xu, {
+                return (0, r.jsx)(l.xu, {
                     m: "16px",
-                    children: (0, i.jsxs)(eL.NI, {
-                        children: [(0, i.jsx)(eI.l, {
+                    children: (0, r.jsxs)(eL.NI, {
+                        children: [(0, r.jsx)(eI.l, {
                             children: "Pick a column to show Histogram Diff"
-                        }), (0, i.jsx)(eG.P, {
+                        }), (0, r.jsx)(eY.P, {
                             placeholder: "Select column",
                             value: null == t ? void 0 : t.column_name,
                             onChange: e => {
                                 var n;
-                                let i = e.target.value;
-                                o(!!i);
-                                let l = (null === (n = c.find(e => e.name === i)) || void 0 === n ? void 0 : n.type) || "";
-                                r({
+                                let r = e.target.value;
+                                o(!!r);
+                                let l = (null === (n = c.find(e => e.name === r)) || void 0 === n ? void 0 : n.type) || "";
+                                i({
                                     ...t,
-                                    column_name: i,
+                                    column_name: r,
                                     column_type: l
                                 })
                             },
-                            children: c.map(e => (0, i.jsxs)("option", {
+                            children: c.map(e => (0, r.jsxs)("option", {
                                 value: e.name,
                                 children: [e.name, " : ", e.type]
                             }, e.name))
                         })]
                     })
                 })
             }
-            let eQ = (0, S.createContext)({
+            let e$ = (0, S.createContext)({
                     runAction: () => {}
                 }),
-                eJ = {
+                e0 = {
                     profile_diff: {
                         title: "Profile Diff",
                         RunResultView: ProfileDiffResultView
                     },
                     value_diff: {
                         title: "Value Diff",
                         RunResultView: ValueDiffResultView,
@@ -3090,274 +3197,274 @@
                     histogram_diff: {
                         title: "Histogram Diff",
                         RunResultView: HistogramDiffResultView,
                         RunForm: HistogramDiffForm
                     }
                 },
                 useCloseModalEffect = e => {
-                    let [n] = (0, eT.TH)();
+                    let [n] = (0, eN.TH)();
                     (0, S.useEffect)(() => {
                         e()
                     }, [e, n])
                 };
 
             function RecceActionContextProvider(e) {
                 var n;
                 let {
                     children: t
-                } = e, [r, l] = (0, S.useState)(), {
+                } = e, [i, l] = (0, S.useState)(), {
                     isOpen: o,
                     onOpen: a,
                     onClose: s
                 } = (0, c.q)(), d = (0, S.useCallback)(async (e, n, t) => {
-                    let i;
-                    let r = new Date().getTime().toString();
+                    let r;
+                    let i = new Date().getTime().toString();
                     if (null == t ? void 0 : t.showLast) {
                         let t = await searchRuns(e, n, 1);
-                        1 === t.length && (i = t[0])
+                        1 === t.length && (r = t[0])
                     }
                     l({
-                        session: r,
+                        session: i,
                         type: e,
                         params: n,
-                        lastRun: i,
+                        lastRun: r,
                         options: t
                     }), a()
                 }, [l, a]);
-                return useCloseModalEffect(s), (0, i.jsxs)(eQ.Provider, {
+                return useCloseModalEffect(s), (0, r.jsxs)(e$.Provider, {
                     value: {
                         runAction: d
                     },
-                    children: [r && eJ[r.type] && (0, i.jsx)(RunModal, {
+                    children: [i && e0[i.type] && (0, r.jsx)(RunModal, {
                         isOpen: o,
                         onClose: s,
-                        title: eJ[r.type].title,
-                        type: r.type,
-                        params: r.params,
-                        initialRun: r.lastRun,
-                        RunResultView: eJ[r.type].RunResultView,
-                        RunForm: (null === (n = r.options) || void 0 === n ? void 0 : n.showForm) ? eJ[r.type].RunForm : void 0
-                    }, r.session), t]
+                        title: e0[i.type].title,
+                        type: i.type,
+                        params: i.params,
+                        initialRun: i.lastRun,
+                        RunResultView: e0[i.type].RunResultView,
+                        RunForm: (null === (n = i.options) || void 0 === n ? void 0 : n.showForm) ? e0[i.type].RunForm : void 0
+                    }, i.session), t]
                 })
             }
-            let useRecceActionContext = () => (0, S.useContext)(eQ);
+            let useRecceActionContext = () => (0, S.useContext)(e$);
 
             function NodeView(e) {
                 let {
                     node: n,
                     onCloseNode: t
-                } = e, [, r] = (0, eT.TH)(), {
+                } = e, [, i] = (0, eN.TH)(), {
                     setSqlQuery: o
                 } = useRecceQueryContext(), {
                     fetchFn: s
                 } = models_useRowCountQueries([n.name]), d = "model" === n.resourceType || "seed" === n.resourceType || "source" === n.resourceType, {
                     isOpen: u,
                     onOpen: h,
                     onClose: f
                 } = (0, c.q)(), {
                     runAction: p
                 } = useRecceActionContext(), _ = (0, S.useCallback)(async () => {
                     let e = n.id,
                         t = await createCheckByNodeSchema(e);
-                    r("/checks/".concat(t.check_id))
-                }, [n, r]), R = (0, S.useCallback)(async () => {
+                    i("/checks/".concat(t.check_id))
+                }, [n, i]), R = (0, S.useCallback)(async () => {
                     let e = await s({
                             skipCache: !0
                         }),
                         n = await checks_createCheckByRun(e);
-                    r("/checks/".concat(n.check_id))
-                }, [r, s]);
-                return (0, i.jsxs)(eo.r, {
+                    i("/checks/".concat(n.check_id))
+                }, [i, s]);
+                return (0, r.jsxs)(eo.r, {
                     height: "100%",
                     templateRows: "auto auto 1fr",
-                    children: [(0, i.jsxs)(x.U, {
-                        children: [(0, i.jsx)(l.xu, {
+                    children: [(0, r.jsxs)(x.U, {
+                        children: [(0, r.jsx)(l.xu, {
                             flex: "0 1 20%",
                             p: "16px",
-                            children: (0, i.jsx)(ea.X, {
+                            children: (0, r.jsx)(ea.X, {
                                 size: "sm",
                                 children: n.name
                             })
-                        }), (0, i.jsx)(E.L, {}), "modified" === n.changeStatus && (0, i.jsxs)(l.xu, {
-                            children: [(0, i.jsx)(m.z, {
+                        }), (0, r.jsx)(E.L, {}), "modified" === n.changeStatus && (0, r.jsxs)(l.xu, {
+                            children: [(0, r.jsx)(m.z, {
                                 onClick: h,
-                                leftIcon: (0, i.jsx)(I.tvD, {}),
+                                leftIcon: (0, r.jsx)(I.tvD, {}),
                                 colorScheme: "orange",
                                 variant: "solid",
                                 children: "Diff"
-                            }), (0, i.jsxs)(g.u_, {
+                            }), (0, r.jsxs)(g.u_, {
                                 isOpen: u,
                                 onClose: f,
                                 size: "6xl",
-                                children: [(0, i.jsx)(v.Z, {}), (0, i.jsxs)(j.h, {
+                                children: [(0, r.jsx)(j.Z, {}), (0, r.jsxs)(y.h, {
                                     overflowY: "auto",
                                     height: "75%",
-                                    children: [(0, i.jsx)(es.x, {
+                                    children: [(0, r.jsx)(es.x, {
                                         children: "Model Raw Code Diff"
-                                    }), (0, i.jsx)(y.o, {}), (0, i.jsx)(C.f, {
-                                        children: (0, i.jsx)(SqlDiffView, {
+                                    }), (0, r.jsx)(v.o, {}), (0, r.jsx)(C.f, {
+                                        children: (0, r.jsx)(SqlDiffView, {
                                             base: n.data.base,
                                             current: n.data.current
                                         })
                                     })]
                                 })]
                             })]
-                        }), (0, i.jsx)(l.xu, {
+                        }), (0, r.jsx)(l.xu, {
                             flex: "0 1 1%",
                             p: "16px",
-                            children: (0, i.jsx)(ec.P, {
+                            children: (0, r.jsx)(ec.P, {
                                 onClick: t
                             })
                         })]
-                    }), (0, i.jsx)(l.xu, {
+                    }), (0, r.jsx)(l.xu, {
                         color: "gray",
                         paddingLeft: "16px",
-                        children: (0, i.jsxs)(x.U, {
+                        children: (0, r.jsxs)(x.U, {
                             spacing: "8px",
-                            children: [(0, i.jsx)(ResourceTypeTag, {
+                            children: [(0, r.jsx)(ResourceTypeTag, {
                                 node: n
-                            }), "model" === n.resourceType && (0, i.jsx)(RowCountTag, {
+                            }), "model" === n.resourceType && (0, r.jsx)(RowCountTag, {
                                 node: n
                             })]
                         })
-                    }), d && (0, i.jsxs)(i.Fragment, {
-                        children: [(0, i.jsxs)(ed.m, {
+                    }), d && (0, r.jsxs)(r.Fragment, {
+                        children: [(0, r.jsxs)(ed.m, {
                             overflow: "auto",
                             as: a.k,
-                            children: [(0, i.jsx)(eu.t, {
-                                children: (0, i.jsx)(eh.O, {
+                            children: [(0, r.jsx)(eu.t, {
+                                children: (0, r.jsx)(eh.O, {
                                     children: "Columns"
                                 })
-                            }), (0, i.jsx)(em.n, {
+                            }), (0, r.jsx)(em.n, {
                                 overflow: "auto",
                                 height: "calc(100% - 42px)",
-                                children: (0, i.jsx)(ex.x, {
+                                children: (0, r.jsx)(ex.x, {
                                     p: 0,
                                     overflowY: "auto",
                                     height: "100%",
-                                    children: (0, i.jsx)(SchemaView, {
+                                    children: (0, r.jsx)(SchemaView, {
                                         base: n.data.base,
                                         current: n.data.current
                                     })
                                 })
                             })]
-                        }), (0, i.jsxs)(x.U, {
+                        }), (0, r.jsxs)(x.U, {
                             p: "16px",
-                            children: [(0, i.jsxs)(b.v, {
-                                children: [(0, i.jsx)(ef.j, {
+                            children: [(0, r.jsxs)(b.v, {
+                                children: [(0, r.jsx)(ef.j, {
                                     as: m.z,
                                     size: "sm",
                                     colorScheme: "blue",
                                     children: "Add check"
-                                }), (0, i.jsxs)(k.q, {
-                                    children: [(0, i.jsx)(w.s, {
+                                }), (0, r.jsxs)(k.q, {
+                                    children: [(0, r.jsx)(w.s, {
                                         onClick: _,
                                         children: "Schema Check"
-                                    }), (0, i.jsx)(w.s, {
+                                    }), (0, r.jsx)(w.s, {
                                         onClick: R,
                                         children: "Row Count Check"
                                     })]
                                 })]
-                            }), (0, i.jsx)(E.L, {}), "model" === n.resourceType && (0, i.jsxs)(i.Fragment, {
-                                children: ["added" !== n.changeStatus && "removed" !== n.changeStatus && (0, i.jsx)(i.Fragment, {
-                                    children: (0, i.jsxs)(b.v, {
-                                        children: [(0, i.jsx)(ef.j, {
+                            }), (0, r.jsx)(E.L, {}), "model" === n.resourceType && (0, r.jsxs)(r.Fragment, {
+                                children: ["added" !== n.changeStatus && "removed" !== n.changeStatus && (0, r.jsx)(r.Fragment, {
+                                    children: (0, r.jsxs)(b.v, {
+                                        children: [(0, r.jsx)(ef.j, {
                                             as: m.z,
                                             size: "sm",
                                             colorScheme: "blue",
                                             children: "Advanced Diffs"
-                                        }), (0, i.jsxs)(k.q, {
-                                            children: [(0, i.jsx)(w.s, {
+                                        }), (0, r.jsxs)(k.q, {
+                                            children: [(0, r.jsx)(w.s, {
                                                 onClick: () => {
                                                     p("profile_diff", {
                                                         model: n.name
                                                     }, {
                                                         showForm: !1,
                                                         showLast: !0
                                                     })
                                                 },
                                                 children: "Profile Diff"
-                                            }), (0, i.jsx)(w.s, {
+                                            }), (0, r.jsx)(w.s, {
                                                 onClick: () => {
                                                     p("value_diff", {
                                                         model: n.name
                                                     }, {
                                                         showForm: !0,
                                                         showLast: !0
                                                     })
                                                 },
                                                 children: "Value Diff"
-                                            }), (0, i.jsx)(w.s, {
+                                            }), (0, r.jsx)(w.s, {
                                                 onClick: () => {
                                                     p("top_k_diff", {
                                                         model: n.name,
                                                         column_name: "",
                                                         k: 50
                                                     }, {
                                                         showForm: !0
                                                     })
                                                 },
                                                 children: "Top-K Diff"
-                                            }), (0, i.jsx)(w.s, {
+                                            }), (0, r.jsx)(w.s, {
                                                 onClick: () => {
                                                     p("histogram_diff", {
                                                         model: n.name,
                                                         column_name: "",
                                                         column_type: ""
                                                     }, {
                                                         showForm: !0
                                                     })
                                                 },
                                                 children: "Histogram Diff"
                                             })]
                                         })]
                                     })
-                                }), (0, i.jsx)(m.z, {
+                                }), (0, r.jsx)(m.z, {
                                     colorScheme: "blue",
                                     size: "sm",
                                     onClick: () => {
-                                        o('select * from {{ ref("'.concat(n.name, '") }}')), r("/query")
+                                        o('select * from {{ ref("'.concat(n.name, '") }}')), i("/query")
                                     },
                                     children: "Query"
                                 })]
                             })]
                         })]
                     })]
                 })
             }
-            let eZ = {
+            let e1 = {
                 added: ["Model Added", "Added resource"],
                 removed: ["Model Removed", "Removed resource"],
                 modified: ["Model Modified", "Modified resource"],
                 col_added: ["Column Added", "Added column"],
                 col_removed: ["Column Removed", "Removed column"],
                 col_changed: ["Column Modified", "Modified column"],
                 folder_changed: ["Modified", "Modified folder"]
             };
 
             function ChangeSummary_getIconForChangeStatus(e) {
                 if ("added" === e) return {
                     color: "#1dce00",
-                    icon: M
+                    icon: F
                 };
                 if ("removed" === e) return {
                     color: "#ff067e",
-                    icon: F
+                    icon: M
                 };
                 if ("modified" === e) return {
                     color: "#ffa502",
                     icon: O
                 };
                 if ("col_added" === e) return {
                     color: "#1dce00",
-                    icon: M
+                    icon: F
                 };
                 if ("col_removed" === e) return {
                     color: "#ff067e",
-                    icon: F
+                    icon: M
                 };
                 if ("col_changed" === e) return {
                     color: "#ffa502",
                     icon: O
                 };
                 if ("folder_changed" === e) return {
                     color: "#ffa502",
@@ -3369,378 +3476,378 @@
                 }
             }
 
             function SummaryText(e) {
                 let {
                     name: n,
                     value: t,
-                    tip: r
+                    tip: i
                 } = e;
-                return (0, i.jsxs)(h.g, {
+                return (0, r.jsxs)(h.g, {
                     alignItems: "stretch",
-                    children: [(0, i.jsxs)(f.x, {
+                    children: [(0, r.jsxs)(f.x, {
                         fontSize: "sm",
                         color: "gray",
-                        children: [n, r && (0, i.jsx)(o.u, {
-                            label: r,
-                            children: (0, i.jsx)(l.xu, {
+                        children: [n, i && (0, r.jsx)(o.u, {
+                            label: i,
+                            children: (0, r.jsx)(l.xu, {
                                 display: "inline-block",
-                                children: (0, i.jsx)(s.J, {
+                                children: (0, r.jsx)(s.J, {
                                     mx: "2px",
                                     as: B.H33,
                                     boxSize: 3
                                 })
                             })
                         })]
                     }), t]
                 })
             }
 
             function ChangeStatusCountLabel(e) {
                 let {
                     changeStatus: n,
                     value: t
-                } = e, [r] = n ? eZ[n] : [""], {
+                } = e, [i] = n ? e1[n] : [""], {
                     icon: l,
                     color: o
                 } = ChangeSummary_getIconForChangeStatus(n);
-                return (0, i.jsxs)(h.g, {
+                return (0, r.jsxs)(h.g, {
                     alignItems: "stretch",
-                    children: [(0, i.jsxs)(a.k, {
+                    children: [(0, r.jsxs)(a.k, {
                         alignItems: "center",
                         fontSize: "sm",
                         color: "gray",
-                        children: [(0, i.jsx)(s.J, {
+                        children: [(0, r.jsx)(s.J, {
                             mr: "5px",
                             as: l,
                             color: o
-                        }), r]
-                    }), (0, i.jsx)(f.x, {
+                        }), i]
+                    }), (0, r.jsx)(f.x, {
                         fontSize: "sm",
                         children: t
                     })]
                 })
             }
 
             function calculateColumnChange(e, n) {
                 let t = 0,
-                    i = 0,
-                    r = 0;
+                    r = 0,
+                    i = 0;
                 return (e || n) && (n && Object.keys(n.columns || {}).forEach(n => {
                     (!e || !e.columns || !e.columns[n]) && t++
                 }), e && Object.keys(e.columns || {}).forEach(e => {
-                    (!n || !n.columns || !n.columns[e]) && i++
+                    (!n || !n.columns || !n.columns[e]) && r++
                 }), n && e && Object.keys(n.columns || {}).forEach(t => {
-                    e.columns && n.columns && e.columns[t] && e.columns[t].type !== n.columns[t].type && r++
+                    e.columns && n.columns && e.columns[t] && e.columns[t].type !== n.columns[t].type && i++
                 })), {
                     adds: t,
-                    removes: i,
-                    modifies: r
+                    removes: r,
+                    modifies: i
                 }
             }
 
             function calculateChangeSummary(e, n) {
                 let t = 0,
-                    i = 0,
                     r = 0,
+                    i = 0,
                     l = 0,
                     o = 0,
                     a = 0;
                 return n.forEach(n => {
-                    "added" === e.nodes[n].changeStatus ? t++ : "removed" === e.nodes[n].changeStatus ? i++ : "modified" === e.nodes[n].changeStatus && r++;
+                    "added" === e.nodes[n].changeStatus ? t++ : "removed" === e.nodes[n].changeStatus ? r++ : "modified" === e.nodes[n].changeStatus && i++;
                     let s = e.nodes[n].data.base,
                         c = e.nodes[n].data.current,
                         d = calculateColumnChange(s, c);
                     l += d.adds, o += d.removes, a += d.modifies
                 }), {
                     adds: t,
-                    removes: i,
-                    modifies: r,
+                    removes: r,
+                    modifies: i,
                     col_added: l,
                     col_removed: o,
                     col_changed: a
                 }
             }
 
             function ChangeSummary(e) {
                 let {
                     lineageGraphSets: n
                 } = e, {
                     adds: t,
-                    removes: r,
+                    removes: i,
                     modifies: o,
                     col_added: a,
                     col_removed: s,
                     col_changed: c
                 } = calculateChangeSummary(n.all, n.modifiedSet);
-                return (0, i.jsxs)(eo.r, {
+                return (0, r.jsxs)(eo.r, {
                     templateColumns: "1fr 1fr",
                     mb: "10px",
                     borderTop: "1px solid lightgray",
                     padding: "2.5vw",
-                    children: [(0, i.jsx)(l.xu, {
+                    children: [(0, r.jsx)(l.xu, {
                         borderColor: "lightgray",
-                        children: (0, i.jsx)(SummaryText, {
+                        children: (0, r.jsx)(SummaryText, {
                             name: "Code Changes",
-                            value: (0, i.jsx)(i.Fragment, {
-                                children: (0, i.jsxs)(eo.r, {
+                            value: (0, r.jsx)(r.Fragment, {
+                                children: (0, r.jsxs)(eo.r, {
                                     templateColumns: "1fr 1fr 1fr",
                                     width: "100%",
-                                    children: [(0, i.jsx)(ChangeStatusCountLabel, {
+                                    children: [(0, r.jsx)(ChangeStatusCountLabel, {
                                         changeStatus: "added",
                                         value: t
-                                    }), (0, i.jsx)(ChangeStatusCountLabel, {
+                                    }), (0, r.jsx)(ChangeStatusCountLabel, {
                                         changeStatus: "removed",
-                                        value: r
-                                    }), (0, i.jsx)(ChangeStatusCountLabel, {
+                                        value: i
+                                    }), (0, r.jsx)(ChangeStatusCountLabel, {
                                         changeStatus: "modified",
                                         value: o
                                     })]
                                 })
                             })
                         })
-                    }), (0, i.jsx)(l.xu, {
+                    }), (0, r.jsx)(l.xu, {
                         borderLeft: "1px",
                         paddingLeft: "12px",
                         borderColor: "lightgray",
-                        children: (0, i.jsx)(SummaryText, {
+                        children: (0, r.jsx)(SummaryText, {
                             name: "Column Changes",
-                            value: (0, i.jsx)(i.Fragment, {
-                                children: (0, i.jsxs)(eo.r, {
+                            value: (0, r.jsx)(r.Fragment, {
+                                children: (0, r.jsxs)(eo.r, {
                                     templateColumns: "1fr 1fr 1fr",
                                     width: "100%",
-                                    children: [(0, i.jsx)(ChangeStatusCountLabel, {
+                                    children: [(0, r.jsx)(ChangeStatusCountLabel, {
                                         changeStatus: "col_added",
                                         value: a
-                                    }), (0, i.jsx)(ChangeStatusCountLabel, {
+                                    }), (0, r.jsx)(ChangeStatusCountLabel, {
                                         changeStatus: "col_removed",
                                         value: s
-                                    }), (0, i.jsx)(ChangeStatusCountLabel, {
+                                    }), (0, r.jsx)(ChangeStatusCountLabel, {
                                         changeStatus: "col_changed",
                                         value: c
                                     })]
                                 })
                             })
                         })
                     })]
                 })
             }
-            var eX = t(76353),
-                eY = t(53248),
-                e$ = t(9763),
-                e0 = t(95853);
+            var e2 = t(76353),
+                e5 = t(53248),
+                e3 = t(9763),
+                e6 = t(95853);
 
             function SchemaDiffCard(e) {
                 let {
                     node: n,
                     ...t
                 } = e;
-                return (0, i.jsxs)(eX.Z, {
+                return (0, r.jsxs)(e2.Z, {
                     maxWidth: "500px",
-                    children: [(0, i.jsxs)(eY.O, {
-                        children: [(0, i.jsx)(ea.X, {
+                    children: [(0, r.jsxs)(e5.O, {
+                        children: [(0, r.jsx)(ea.X, {
                             fontSize: 18,
                             children: t.title
-                        }), (0, i.jsxs)(x.U, {
+                        }), (0, r.jsxs)(x.U, {
                             spacing: "8px",
                             p: "16px",
-                            children: [(0, i.jsx)(ResourceTypeTag, {
+                            children: [(0, r.jsx)(ResourceTypeTag, {
                                 node: n
-                            }), "model" === n.resourceType && (0, i.jsx)(RowCountTag, {
+                            }), "model" === n.resourceType && (0, r.jsx)(RowCountTag, {
                                 node: n,
                                 isAutoFetching: !0
                             })]
                         })]
-                    }), (0, i.jsx)(e$.e, {
-                        children: (0, i.jsx)(a.k, {
-                            children: (0, i.jsx)(SchemaView, {
+                    }), (0, r.jsx)(e3.e, {
+                        children: (0, r.jsx)(a.k, {
+                            children: (0, r.jsx)(SchemaView, {
                                 base: n.data.base,
                                 current: n.data.current
                             })
                         })
                     })]
                 })
             }
 
             function listChangedNodes(e) {
                 let n = [],
                     t = e.all.nodes;
                 return e.modifiedSet.forEach(e => {
-                    var i, r;
+                    var r, i;
                     let l = t[e],
-                        o = mergeKeysWithStatus(Object.keys((null === (i = l.data.base) || void 0 === i ? void 0 : i.columns) || {}), Object.keys((null === (r = l.data.current) || void 0 === r ? void 0 : r.columns) || {})),
+                        o = mergeKeysWithStatus(Object.keys((null === (r = l.data.base) || void 0 === r ? void 0 : r.columns) || {}), Object.keys((null === (i = l.data.current) || void 0 === i ? void 0 : i.columns) || {})),
                         a = !Object.values(o).every(e => void 0 === e);
                     a && l.data.base && l.data.current && n.push(l)
                 }), n
             }
 
             function SchemaSummary(e) {
                 let {
                     lineageGraphSets: n
-                } = e, [t, r] = (0, S.useState)([]);
+                } = e, [t, i] = (0, S.useState)([]);
                 return (0, S.useEffect)(() => {
-                    r(listChangedNodes(n))
-                }, [n]), (0, i.jsxs)(i.Fragment, {
-                    children: [(0, i.jsx)(a.k, {
+                    i(listChangedNodes(n))
+                }, [n]), (0, r.jsxs)(r.Fragment, {
+                    children: [(0, r.jsx)(a.k, {
                         w: "100%",
                         paddingBottom: "10px",
                         marginBottom: "20px",
                         marginTop: "20px",
-                        children: (0, i.jsx)(ea.X, {
+                        children: (0, r.jsx)(ea.X, {
                             fontSize: 24,
                             children: "Schema Summary"
                         })
-                    }), (0, i.jsx)(a.k, {
+                    }), (0, r.jsx)(a.k, {
                         w: "100%",
                         paddingBottom: "10px",
                         marginBottom: "20px",
-                        children: 0 === t.length ? (0, i.jsx)(i.Fragment, {
-                            children: (0, i.jsx)(f.x, {
+                        children: 0 === t.length ? (0, r.jsx)(r.Fragment, {
+                            children: (0, r.jsx)(f.x, {
                                 fontSize: 18,
                                 color: "gray",
                                 children: "No schema changes detected."
                             })
-                        }) : (0, i.jsx)(i.Fragment, {
-                            children: (0, i.jsx)(e0.M, {
+                        }) : (0, r.jsx)(r.Fragment, {
+                            children: (0, r.jsx)(e6.M, {
                                 minChildWidth: "400px",
                                 spacing: "2vw",
                                 padding: "2.5vw",
                                 width: "100%",
                                 backgroundColor: "lightgray",
-                                children: t.map(e => (0, i.jsx)(SchemaDiffCard, {
+                                children: t.map(e => (0, r.jsx)(SchemaDiffCard, {
                                     title: e.name,
                                     node: e
                                 }, e.id))
                             })
                         })
                     })]
                 })
             }
 
             function SummaryView() {
                 let {
                     lineageGraphSets: e
                 } = useLineageGraphsContext();
-                return (0, i.jsx)(i.Fragment, {
-                    children: (0, i.jsxs)(a.k, {
+                return (0, r.jsx)(r.Fragment, {
+                    children: (0, r.jsxs)(a.k, {
                         direction: "column",
                         w: "100%",
                         minHeight: "650px",
-                        children: [(0, i.jsx)(a.k, {
+                        children: [(0, r.jsx)(a.k, {
                             w: "100%",
                             paddingBottom: "10px",
                             marginBottom: "20px",
-                            children: (0, i.jsx)(ea.X, {
+                            children: (0, r.jsx)(ea.X, {
                                 fontSize: 24,
                                 children: "Change Summary"
                             })
-                        }), e && (0, i.jsxs)(i.Fragment, {
-                            children: [(0, i.jsx)(ChangeSummary, {
+                        }), e && (0, r.jsxs)(r.Fragment, {
+                            children: [(0, r.jsx)(ChangeSummary, {
                                 lineageGraphSets: e
-                            }), (0, i.jsx)(eH.i, {}), (0, i.jsx)(SchemaSummary, {
+                            }), (0, r.jsx)(eK.i, {}), (0, r.jsx)(SchemaSummary, {
                                 lineageGraphSets: e
                             })]
                         })]
                     })
                 })
             }
-            var e1 = t(45438),
-                e2 = t(72491),
-                e5 = t(52246),
-                e3 = t(25807),
-                e4 = t(15012);
+            var e4 = t(45438),
+                e9 = t(72491),
+                e8 = t(52246),
+                e7 = t(25807),
+                ne = t(15012);
 
             function AddSchemaChangesCheckButton(e) {
                 let {
                     nodes: n,
                     onFinish: t
-                } = e, [, r] = (0, eT.TH)();
-                return (0, i.jsxs)(m.z, {
+                } = e, [, i] = (0, eN.TH)();
+                return (0, r.jsxs)(m.z, {
                     size: "xs",
                     variant: "outline",
                     isDisabled: 0 === n.length,
                     onClick: async () => {
                         let e;
                         1 === n.length ? e = await createCheckByNodeSchema(n[0].id) : await Promise.all(n.map(async e => {
                             await createCheckByNodeSchema(e.id)
-                        })), t(), e ? r("/checks/".concat(e.check_id)) : r("/checks")
+                        })), t(), e ? i("/checks/".concat(e.check_id)) : i("/checks")
                     },
-                    children: [(0, i.jsx)(s.J, {
+                    children: [(0, r.jsx)(s.J, {
                         as: q.Edg
                     }), "Add schema check"]
                 })
             }
 
             function AddLineageDiffCheckButton(e) {
                 let {
                     viewMode: n,
                     nodes: t,
-                    onFinish: r,
+                    onFinish: i,
                     withIcon: l
-                } = e, [, o] = (0, eT.TH)();
-                return (0, i.jsxs)(m.z, {
+                } = e, [, o] = (0, eN.TH)();
+                return (0, r.jsxs)(m.z, {
                     size: "xs",
                     variant: "outline",
                     backgroundColor: "white",
                     isDisabled: 0 === t.length,
                     onClick: async () => {
                         let e = t.map(e => e.id),
-                            i = await createLineageDiffCheck(n, e);
-                        r(), i ? o("/checks/".concat(i.check_id)) : o("/checks")
+                            r = await createLineageDiffCheck(n, e);
+                        i(), r ? o("/checks/".concat(r.check_id)) : o("/checks")
                     },
-                    children: [l && (0, i.jsx)(s.J, {
-                        as: e4.Ks7
+                    children: [l && (0, r.jsx)(s.J, {
+                        as: ne.Ks7
                     }), "Add lineage diff check"]
                 })
             }
 
             function NodeSelector(e) {
-                var n, t, r, o;
+                var n, t, i, o;
                 let {
                     viewMode: a,
                     nodes: c,
                     onClose: d,
                     onActionStarted: u,
                     onActionNodeUpdated: h,
                     onActionCompleted: f
                 } = e, [p, g] = (0, S.useState)({
                     mode: "per_node",
                     status: "pending",
                     completed: 0,
                     total: 0
-                }), v = (0, H.NL)(), [, j] = (0, eT.TH)(), submitRunForNodes = async (e, n, t) => {
-                    let i = "multi_nodes";
-                    p.mode = i, u(), p.status = "running";
-                    let r = [];
+                }), j = (0, H.NL)(), [, y] = (0, eN.TH)(), submitRunForNodes = async (e, n, t) => {
+                    let r = "multi_nodes";
+                    p.mode = r, u(), p.status = "running";
+                    let i = [];
                     for (let e of c) {
                         let t = n(e);
                         t ? (e.action = {
-                            mode: i,
+                            mode: r,
                             status: "skipped",
                             skipReason: t
                         }, h(e)) : (e.action = {
-                            mode: i,
+                            mode: r,
                             status: "pending"
-                        }, r.push(e))
+                        }, i.push(e))
                     }
-                    let l = t(r);
+                    let l = t(i);
                     try {
                         let {
                             run_id: n
                         } = await submitRun(e, l, {
                             nowait: !0
                         });
                         for (p.currentRun = {
                                 run_id: n
                             }, p.total = 1;;) {
                             let e = await waitRun(n, 2);
                             p.currentRun = e;
                             let t = e.error ? "failure" : e.result ? "success" : "running";
-                            for (let n of r) n.action = {
-                                mode: i,
+                            for (let n of i) n.action = {
+                                mode: r,
                                 status: t,
                                 run: e
                             }, h(n);
                             if (e.error || e.result) break
                         }
                     } catch (e) {}
                     if (p.completed = 1, "canceling" === p.status) {
@@ -3750,44 +3857,44 @@
                     p.status = "completed", f()
                 }, submitRunsPerNodes = async (e, n) => {
                     let t = "per_node";
                     for (let e of (p.mode = t, u(), p.status = "running", c)) e.action = {
                         mode: t,
                         status: "pending"
                     }, h(e);
-                    for (let i of (p.completed = 0, p.total = c.length, c)) {
+                    for (let r of (p.completed = 0, p.total = c.length, c)) {
                         let {
-                            params: r,
+                            params: i,
                             skipReason: l
-                        } = n(i);
-                        if (l) i.action = {
+                        } = n(r);
+                        if (l) r.action = {
                             mode: t,
                             status: "skipped",
                             skipReason: l
-                        }, h(i);
+                        }, h(r);
                         else try {
                             let {
                                 run_id: n
-                            } = await submitRun(e, r, {
+                            } = await submitRun(e, i, {
                                 nowait: !0
                             });
                             for (p.currentRun = {
                                     run_id: n
-                                }, i.action = {
+                                }, r.action = {
                                     mode: t,
                                     status: "running"
-                                }, h(i);;) {
+                                }, h(r);;) {
                                 let e = await waitRun(n, 2);
                                 p.currentRun = e;
-                                let r = e.error ? "failure" : e.result ? "success" : "running";
-                                if (i.action = {
+                                let i = e.error ? "failure" : e.result ? "success" : "running";
+                                if (r.action = {
                                         mode: t,
-                                        status: r,
+                                        status: i,
                                         run: e
-                                    }, h(i), e.error || e.result) break
+                                    }, h(r), e.error || e.result) break
                             }
                         } catch (e) {} finally {
                             p.currentRun = void 0
                         }
                         if (p.completed++, "canceling" === p.status) {
                             p.status = "canceled", f();
                             return
@@ -3808,117 +3915,117 @@
                             node_names: e.map(e => e.name)
                         };
                         return n
                     })
                 }, handleValueDiffClick = async () => {
                     submitRunsPerNodes("value_diff", e => {
                         var n, t;
-                        let i = null === (t = e.data) || void 0 === t ? void 0 : null === (n = t.current) || void 0 === n ? void 0 : n.primary_key;
-                        if (!i) return {
+                        let r = null === (t = e.data) || void 0 === t ? void 0 : null === (n = t.current) || void 0 === n ? void 0 : n.primary_key;
+                        if (!r) return {
                             skipReason: "No primary key found. The first unique column is used as primary key."
                         };
-                        let r = {
+                        let i = {
                             model: e.name,
-                            primary_key: i
+                            primary_key: r
                         };
                         return {
-                            params: r
+                            params: i
                         }
                     })
                 }, handleCancel = async () => {
                     var e;
                     p.status = "canceling", (null === (e = p.currentRun) || void 0 === e ? void 0 : e.run_id) && cancelRun(p.currentRun.run_id)
-                }, y = (0, S.useCallback)(async () => {
+                }, v = (0, S.useCallback)(async () => {
                     var e;
                     let n = null === (e = p.currentRun) || void 0 === e ? void 0 : e.run_id;
                     if (!n) return;
                     let t = await checks_createCheckByRun(n);
-                    v.invalidateQueries({
+                    j.invalidateQueries({
                         queryKey: Z.checks()
-                    }), j("/checks/".concat(t.check_id))
-                }, [null === (n = p.currentRun) || void 0 === n ? void 0 : n.run_id, j, v]);
-                return (0, e2.z)(() => {
+                    }), y("/checks/".concat(t.check_id))
+                }, [null === (n = p.currentRun) || void 0 === n ? void 0 : n.run_id, y, j]);
+                return (0, e9.z)(() => {
                     "running" === p.status && handleCancel()
-                }), (0, i.jsxs)(l.xu, {
+                }), (0, r.jsxs)(l.xu, {
                     bg: "white",
                     rounded: "md",
                     shadow: "dark-lg",
-                    children: ["pending" === p.status && (0, i.jsxs)(x.U, {
+                    children: ["pending" === p.status && (0, r.jsxs)(x.U, {
                         p: "5px 15px",
                         mt: "4",
-                        divider: (0, i.jsx)(e5.c, {
+                        divider: (0, r.jsx)(e8.c, {
                             borderColor: "gray.200"
                         }),
                         spacing: 4,
-                        children: [(0, i.jsxs)(e3.h, {
+                        children: [(0, r.jsxs)(e7.h, {
                             size: "xs",
                             isAttached: !0,
                             variant: "outline",
                             rounded: "xs",
                             onClick: d,
-                            children: [(0, i.jsxs)(m.z, {
+                            children: [(0, r.jsxs)(m.z, {
                                 children: [c.length, " selected"]
-                            }), (0, i.jsx)(P.h, {
+                            }), (0, r.jsx)(P.h, {
                                 "aria-label": "Exit select Mode",
-                                icon: (0, i.jsx)(e1.D, {})
+                                icon: (0, r.jsx)(e4.D, {})
                             })]
-                        }), (0, i.jsxs)(x.U, {
-                            children: [(0, i.jsx)(AddSchemaChangesCheckButton, {
+                        }), (0, r.jsxs)(x.U, {
+                            children: [(0, r.jsx)(AddSchemaChangesCheckButton, {
                                 nodes: c,
                                 onFinish: d
-                            }), (0, i.jsx)(AddLineageDiffCheckButton, {
+                            }), (0, r.jsx)(AddLineageDiffCheckButton, {
                                 viewMode: a,
                                 nodes: c,
                                 onFinish: d,
                                 withIcon: !0
                             })]
-                        }), (0, i.jsxs)(x.U, {
-                            children: [(0, i.jsxs)(m.z, {
+                        }), (0, r.jsxs)(x.U, {
+                            children: [(0, r.jsxs)(m.z, {
                                 size: "xs",
                                 variant: "outline",
                                 isDisabled: 0 === c.length,
                                 onClick: handleRowCountDiffClick,
-                                children: [(0, i.jsx)(s.J, {
+                                children: [(0, r.jsx)(s.J, {
                                     as: B.SwK
                                 }), "Row count diff"]
-                            }), (0, i.jsxs)(m.z, {
+                            }), (0, r.jsxs)(m.z, {
                                 size: "xs",
                                 variant: "outline",
                                 isDisabled: 0 === c.length,
                                 onClick: handleValueDiffClick,
-                                children: [(0, i.jsx)(s.J, {
-                                    as: e4.pRi
+                                children: [(0, r.jsx)(s.J, {
+                                    as: ne.pRi
                                 }), "Value diff"]
                             })]
                         })]
-                    }), "pending" !== p.status && (0, i.jsxs)(x.U, {
+                    }), "pending" !== p.status && (0, r.jsxs)(x.U, {
                         p: "5px 15px",
                         mt: "4",
-                        divider: (0, i.jsx)(e5.c, {
+                        divider: (0, r.jsx)(e8.c, {
                             borderColor: "gray.200"
                         }),
                         spacing: 4,
-                        children: [(0, i.jsxs)(l.xu, {
+                        children: [(0, r.jsxs)(l.xu, {
                             fontSize: "10pt",
-                            children: ["Progress: ", "per_node" === p.mode ? "".concat(p.completed, " / ").concat(p.total) : (null === (o = p.currentRun) || void 0 === o ? void 0 : null === (r = o.progress) || void 0 === r ? void 0 : r.percentage) ? "".concat(100 * p.currentRun.progress.percentage, "%") : "completed" === p.status ? "100%" : "0%", " ", "canceled" === p.status ? " (canceled)" : ""]
-                        }), "running" === p.status || "canceling" === p.status ? (0, i.jsx)(m.z, {
+                            children: ["Progress: ", "per_node" === p.mode ? "".concat(p.completed, " / ").concat(p.total) : (null === (o = p.currentRun) || void 0 === o ? void 0 : null === (i = o.progress) || void 0 === i ? void 0 : i.percentage) ? "".concat(100 * p.currentRun.progress.percentage, "%") : "completed" === p.status ? "100%" : "0%", " ", "canceled" === p.status ? " (canceled)" : ""]
+                        }), "running" === p.status || "canceling" === p.status ? (0, r.jsx)(m.z, {
                             size: "xs",
                             variant: "outline",
                             onClick: handleCancel,
                             isLoading: "canceling" === p.status,
                             loadingText: "Canceling",
                             children: "Cancel"
-                        }) : (0, i.jsxs)(x.U, {
-                            children: ["multi_nodes" === p.mode && (null === (t = p.currentRun) || void 0 === t ? void 0 : t.result) && (0, i.jsx)(m.z, {
+                        }) : (0, r.jsxs)(x.U, {
+                            children: ["multi_nodes" === p.mode && (null === (t = p.currentRun) || void 0 === t ? void 0 : t.result) && (0, r.jsx)(m.z, {
                                 display: "none",
                                 size: "xs",
                                 variant: "outline",
-                                onClick: y,
+                                onClick: v,
                                 children: "Add to checklist"
-                            }), (0, i.jsx)(m.z, {
+                            }), (0, r.jsx)(m.z, {
                                 size: "xs",
                                 variant: "outline",
                                 onClick: d,
                                 children: "Close"
                             })]
                         })]
                     })]
@@ -3933,30 +4040,30 @@
                 function columnCellClass(e) {
                     if (e.base === e.current);
                     else if (e.base < e.current || "N/A" === e.base) return "column-body-added";
                     else if (e.base > e.current || "N/A" === e.current) return "column-body-removed";
                     return "column-body-normal"
                 }
                 let t = n.result || {},
-                    r = Object.keys(n.result || {}).map(e => {
+                    i = Object.keys(n.result || {}).map(e => {
                         let n = t[e],
-                            i = (null == n ? void 0 : n.base) || null,
-                            r = (null == n ? void 0 : n.curr) || null,
+                            r = (null == n ? void 0 : n.base) || null,
+                            i = (null == n ? void 0 : n.curr) || null,
                             l = "No Change";
-                        return null !== i && null !== r ? l = i < r ? "+ ".concat(Math.round((r - i) / i * 100), "%") : i > r ? "- ".concat(Math.round((i - r) / i * 100), "%") : "No Change" : i === r ? l = "N/A" : null === i ? l = "Added" : null === r && (l = "Removed"), {
+                        return null !== r && null !== i ? l = r < i ? "+ ".concat(Math.round((i - r) / r * 100), "%") : r > i ? "- ".concat(Math.round((r - i) / r * 100), "%") : "No Change" : r === i ? l = "N/A" : null === r ? l = "Added" : null === i && (l = "Removed"), {
                             name: e,
-                            base: null === i ? "N/A" : Number(i),
-                            current: null === r ? "N/A" : Number(r),
+                            base: null === r ? "N/A" : Number(r),
+                            current: null === i ? "N/A" : Number(i),
                             delta: l
                         }
                     });
-                return (0, i.jsx)(a.k, {
+                return (0, r.jsx)(a.k, {
                     direction: "column",
-                    children: Object.keys(t).length > 0 && (0, i.jsx)(i.Fragment, {
-                        children: (0, i.jsx)(ScreenshotDataGrid, {
+                    children: Object.keys(t).length > 0 && (0, r.jsx)(r.Fragment, {
+                        children: (0, r.jsx)(ScreenshotDataGrid, {
                             style: {
                                 blockSize: "auto",
                                 maxHeight: "100%",
                                 overflow: "auto",
                                 fontSize: "10pt",
                                 borderWidth: 1
                             },
@@ -3973,156 +4080,159 @@
                                 name: "Current Rows",
                                 cellClass: columnCellClass
                             }, {
                                 key: "delta",
                                 name: "Delta",
                                 cellClass: columnCellClass
                             }],
-                            rows: r,
+                            rows: i,
+                            renderers: {
+                                noRowsFallback: (0, r.jsx)(EmptyRowsRenderer, {})
+                            },
                             className: "rdg-light",
                             enableScreenshot: !0
                         })
                     })
                 })
             }
 
             function NodeRunView(e) {
-                var n, t, r, o, s, c, d, u;
+                var n, t, i, o, s, c, d, u;
                 let {
                     node: h,
                     onCloseNode: f
-                } = e, p = null === (n = h.action) || void 0 === n ? void 0 : n.run, [, g] = (0, eT.TH)(), v = (0, H.NL)(), [j, y] = (0, S.useState)(), C = (0, S.useCallback)(async () => {
+                } = e, p = null === (n = h.action) || void 0 === n ? void 0 : n.run, [, g] = (0, eN.TH)(), j = (0, H.NL)(), [y, v] = (0, S.useState)(), C = (0, S.useCallback)(async () => {
                     if (!(null == p ? void 0 : p.run_id)) return;
-                    let e = await checks_createCheckByRun(p.run_id, j);
-                    v.invalidateQueries({
+                    let e = await checks_createCheckByRun(p.run_id, y);
+                    j.invalidateQueries({
                         queryKey: Z.checks()
                     }), g("/checks/".concat(e.check_id))
-                }, [null == p ? void 0 : p.run_id, g, v, j]), b = (null === (r = h.action) || void 0 === r ? void 0 : null === (t = r.run) || void 0 === t ? void 0 : t.type) === "value_diff" ? ValueDiffResultView : (null === (s = h.action) || void 0 === s ? void 0 : null === (o = s.run) || void 0 === o ? void 0 : o.type) === "row_count_diff" ? RowCountDiffResultView : null;
-                return (0, i.jsxs)(eo.r, {
+                }, [null == p ? void 0 : p.run_id, g, j, y]), b = (null === (i = h.action) || void 0 === i ? void 0 : null === (t = i.run) || void 0 === t ? void 0 : t.type) === "value_diff" ? ValueDiffResultView : (null === (s = h.action) || void 0 === s ? void 0 : null === (o = s.run) || void 0 === o ? void 0 : o.type) === "row_count_diff" ? RowCountDiffResultView : null;
+                return (0, r.jsxs)(eo.r, {
                     height: "100%",
                     templateRows: "auto auto 1fr",
-                    children: [(0, i.jsxs)(x.U, {
-                        children: [(0, i.jsx)(l.xu, {
+                    children: [(0, r.jsxs)(x.U, {
+                        children: [(0, r.jsx)(l.xu, {
                             flex: "0 1 20%",
                             p: "16px",
-                            children: (0, i.jsx)(ea.X, {
+                            children: (0, r.jsx)(ea.X, {
                                 size: "sm",
                                 children: h.name
                             })
-                        }), (0, i.jsx)(E.L, {}), (0, i.jsx)(l.xu, {
+                        }), (0, r.jsx)(E.L, {}), (0, r.jsx)(l.xu, {
                             flex: "0 1 1%",
                             p: "16px",
-                            children: (0, i.jsx)(ec.P, {
+                            children: (0, r.jsx)(ec.P, {
                                 onClick: f
                             })
                         })]
-                    }), (0, i.jsx)(l.xu, {
+                    }), (0, r.jsx)(l.xu, {
                         color: "gray",
                         paddingLeft: "16px",
-                        children: (0, i.jsx)(x.U, {
+                        children: (0, r.jsx)(x.U, {
                             spacing: "8px",
-                            children: (0, i.jsx)(ResourceTypeTag, {
+                            children: (0, r.jsx)(ResourceTypeTag, {
                                 node: h
                             })
                         })
-                    }), (0, i.jsxs)(ed.m, {
+                    }), (0, r.jsxs)(ed.m, {
                         overflow: "auto",
                         as: a.k,
-                        children: [(0, i.jsx)(eu.t, {
-                            children: (0, i.jsx)(eh.O, {
+                        children: [(0, r.jsx)(eu.t, {
+                            children: (0, r.jsx)(eh.O, {
                                 children: "Run"
                             })
-                        }), (0, i.jsx)(em.n, {
+                        }), (0, r.jsx)(em.n, {
                             overflow: "auto",
                             height: "calc(100% - 42px)",
-                            children: (0, i.jsx)(ex.x, {
+                            children: (0, r.jsx)(ex.x, {
                                 p: 0,
                                 overflowY: "auto",
                                 height: "100%",
-                                children: b ? (0, i.jsx)(RunView, {
+                                children: b ? (0, r.jsx)(RunView, {
                                     run: null === (c = h.action) || void 0 === c ? void 0 : c.run,
-                                    viewOptions: j,
-                                    onViewOptionsChanged: y,
+                                    viewOptions: y,
+                                    onViewOptionsChanged: v,
                                     RunResultView: b
-                                }) : (0, i.jsx)(l.xu, {
+                                }) : (0, r.jsx)(l.xu, {
                                     p: "20px 10px",
                                     children: "No run result"
                                 })
                             })
                         })]
-                    }), (0, i.jsxs)(x.U, {
+                    }), (0, r.jsxs)(x.U, {
                         p: "16px",
-                        children: [(0, i.jsx)(E.L, {}), (0, i.jsx)(m.z, {
+                        children: [(0, r.jsx)(E.L, {}), (0, r.jsx)(m.z, {
                             size: "sm",
                             colorScheme: "blue",
                             isDisabled: !(null === (u = h.action) || void 0 === u ? void 0 : null === (d = u.run) || void 0 === d ? void 0 : d.result),
                             onClick: C,
                             children: "Add to checklist"
                         })]
                     })]
                 })
             }
             let layout = function(e, n) {
                     let t = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "LR",
-                        i = new(N()).graphlib.Graph;
-                    i.setDefaultEdgeLabel(() => ({})), i.setGraph({
+                        r = new(T()).graphlib.Graph;
+                    r.setDefaultEdgeLabel(() => ({})), r.setGraph({
                         rankdir: t
                     }), e.forEach(e => {
-                        i.setNode(e.id, {
+                        r.setNode(e.id, {
                             width: 300,
                             height: 36
                         })
                     }), n.forEach(e => {
-                        i.setEdge(e.source, e.target)
-                    }), N().layout(i), e.forEach(e => {
-                        let n = i.node(e.id);
+                        r.setEdge(e.source, e.target)
+                    }), T().layout(r), e.forEach(e => {
+                        let n = r.node(e.id);
                         return e.position = {
                             x: n.x - 150,
                             y: n.y - 18
                         }, e
                     })
                 },
-                e6 = {
+                nn = {
                     customNode: GraphNode
                 },
-                e9 = {
+                nt = {
                     customEdge: GraphEdge
                 },
                 nodeColor = e => {
                     var n, t;
                     return (null == e ? void 0 : null === (n = e.data) || void 0 === n ? void 0 : n.changeStatus) ? getIconForChangeStatus(null == e ? void 0 : null === (t = e.data) || void 0 === t ? void 0 : t.changeStatus).color : "lightgray"
                 },
-                e8 = {
+                nr = {
                     all: "All",
                     changed_models: "Changed Models"
                 };
 
             function ChangeStatusLegend() {
-                return (0, i.jsx)(l.xu, {
+                return (0, r.jsx)(l.xu, {
                     bg: "white",
                     padding: "12px",
                     borderWidth: "1px",
                     borderColor: "gray.200",
                     fontSize: "sm",
                     children: Object.entries({
                         added: ["Added", "Added resource"],
                         removed: ["Removed", "Removed resource"],
                         modified: ["Modified", "Modified resource"]
                     }).map(e => {
-                        let [n, [t, r]] = e, {
+                        let [n, [t, i]] = e, {
                             icon: l,
                             color: c
                         } = getIconForChangeStatus(n);
-                        return (0, i.jsx)(o.u, {
-                            label: r,
-                            children: (0, i.jsxs)(a.k, {
+                        return (0, r.jsx)(o.u, {
+                            label: i,
+                            children: (0, r.jsxs)(a.k, {
                                 alignItems: "center",
                                 gap: "6px",
                                 marginBottom: "2px",
-                                children: [(0, i.jsx)(s.J, {
+                                children: [(0, r.jsx)(s.J, {
                                     color: c,
                                     as: l
                                 }), " ", t]
                             })
                         }, n)
                     })
                 })
@@ -4130,144 +4240,144 @@
 
             function _LineageView(e) {
                 let {
                     ...n
                 } = e, {
                     fitView: t,
                     setCenter: o,
-                    getZoom: T
-                } = (0, r._K)(), {
-                    successToast: N,
+                    getZoom: N
+                } = (0, i._K)(), {
+                    successToast: T,
                     failToast: E
                 } = useClipBoardToast(), {
                     toImage: L,
                     ref: I
                 } = useToBlob({
                     imageType: "png",
                     shadowEffect: !0,
                     backgroundColor: "white",
                     ignoreElements: e => {
                         let n = e.className;
                         return !!("string" == typeof n && n.includes(ek))
                     },
                     onSuccess: async e => {
                         try {
-                            await copyBlobToClipboard(e), N("Copied the Lineage View as an image to clipboard")
+                            await copyBlobToClipboard(e), T("Copied the Lineage View as an image to clipboard")
                         } catch (e) {
                             E("Failed to copy image to clipboard", e)
                         }
                     },
                     onError: e => {
                         console.error("Error taking screenshot", e), E("Failed to copy image to clipboard", e)
                     }
-                }), [z, M, F] = (0, r.Rr)([]), [O, A, V] = (0, r.ll)([]), [P, q] = (0, S.useState)(), [H, K] = (0, S.useState)(), {
+                }), [z, F, M] = (0, i.Rr)([]), [O, A, V] = (0, i.ll)([]), [P, q] = (0, S.useState)(), [H, K] = (0, S.useState)(), {
                     lineageGraphSets: W,
                     isLoading: U,
                     error: G
                 } = useLineageGraphsContext(), {
                     isOpen: Q,
                     onOpen: J,
                     onClose: Z
-                } = (0, c.q)(), [X, Y] = (0, S.useState)("detail"), [$, ee] = (0, S.useState)(), [en, et] = (0, S.useState)(!1), [ei, er] = (0, S.useState)(n.viewMode || "changed_models"), [eo, ea] = (0, S.useState)(!1), [es, ec] = (0, S.useState)({
+                } = (0, c.q)(), [X, Y] = (0, S.useState)("detail"), [$, ee] = (0, S.useState)(), [en, et] = (0, S.useState)(!1), [er, ei] = (0, S.useState)(n.viewMode || "changed_models"), [eo, ea] = (0, S.useState)(!1), [es, ec] = (0, S.useState)({
                     x: 0,
                     y: 0
                 });
                 (0, S.useEffect)(() => {
                     if (!W) return;
-                    let e = "changed_models" === ei ? {
+                    let e = "changed_models" === er ? {
                             ...W.changed
                         } : {
                             ...W.all
                         },
                         t = W.modifiedSet;
                     if ("function" == typeof n.filterNodes) {
                         let t = n.filterNodes ? n.filterNodes : () => !0;
                         e.nodes = Object.fromEntries(Object.entries(e.nodes).filter(e => {
-                            let [n, i] = e;
-                            return t(n, i)
+                            let [n, r] = e;
+                            return t(n, r)
                         }))
                     }
-                    let [i, r] = toReactflow(e, W.modifiedSet);
-                    layout(i, r), q(e), K(t), M(i), A(r)
-                }, [M, A, ei, W, n.filterNodes]);
+                    let [r, i] = toReactflow(e, W.modifiedSet);
+                    layout(r, i), q(e), K(t), F(r), A(i)
+                }, [F, A, er, W, n.filterNodes]);
                 let centerNode = e => {
                         if (e.width && e.height) {
                             let n = e.position.x + e.width / 2,
                                 t = e.position.y + e.height / 2,
-                                i = T();
+                                r = N();
                             o(n, t, {
-                                zoom: i,
+                                zoom: r,
                                 duration: 200
                             })
                         }
                     },
                     ed = (0, S.useCallback)(e => {
-                        M(n => {
+                        F(n => {
                             let t = n.map(n => n.id === e.id ? {
                                 ...n,
                                 data: e
                             } : n);
                             return t
                         })
-                    }, [M]);
-                if (U) return (0, i.jsx)(a.k, {
+                    }, [F]);
+                if (U) return (0, r.jsx)(a.k, {
                     width: "100%",
                     height: "100%",
                     alignItems: "center",
                     justifyContent: "center",
-                    children: (0, i.jsx)(d.$, {
+                    children: (0, r.jsx)(d.$, {
                         size: "xl"
                     })
                 });
                 let closeContextMenu = () => {
                     ea(!1), ec({
                         x: 0,
                         y: 0
                     })
                 };
-                return G ? (0, i.jsxs)(i.Fragment, {
+                return G ? (0, r.jsxs)(r.Fragment, {
                     children: ["Fail to load lineage data: ", G]
-                }) : "changed_models" === ei && (void 0 === H || (null == H ? void 0 : H.length) === 0) ? (0, i.jsx)(u.M, {
+                }) : "changed_models" === er && (void 0 === H || (null == H ? void 0 : H.length) === 0) ? (0, r.jsx)(u.M, {
                     h: "100%",
-                    children: (0, i.jsxs)(h.g, {
-                        children: [(0, i.jsx)(i.Fragment, {
+                    children: (0, r.jsxs)(h.g, {
+                        children: [(0, r.jsx)(r.Fragment, {
                             children: "No change detected"
-                        }), (0, i.jsx)(m.z, {
+                        }), (0, r.jsx)(m.z, {
                             colorScheme: "blue",
                             onClick: () => {
-                                er("all")
+                                ei("all")
                             },
                             children: "Show all nodes"
                         })]
                     })
-                }) : (0, i.jsxs)(a.k, {
+                }) : (0, r.jsxs)(a.k, {
                     width: "100%",
                     height: "100%",
-                    children: [(0, i.jsx)(l.xu, {
+                    children: [(0, r.jsx)(l.xu, {
                         flex: "1 0 0px",
-                        children: (0, i.jsxs)(r.x$, {
-                            nodeTypes: e6,
-                            edgeTypes: e9,
+                        children: (0, r.jsxs)(i.x$, {
+                            nodeTypes: nn,
+                            edgeTypes: nt,
                             nodes: z,
                             edges: O,
-                            onNodesChange: F,
+                            onNodesChange: M,
                             onEdgesChange: V,
                             onNodeClick: (e, t) => {
-                                !1 !== n.interactive && (closeContextMenu(), "detail" === X ? (ee(t.data), en || et(!0), M(selectSingleNode(t.id, z)), centerNode(t)) : "action_result" === X ? (ee(t.data), en || et(!0), M(selectSingleNode(t.id, z)), centerNode(t)) : M(selectNode(t.id, z)))
+                                !1 !== n.interactive && (closeContextMenu(), "detail" === X ? (ee(t.data), en || et(!0), F(selectSingleNode(t.id, z)), centerNode(t)) : "action_result" === X ? (ee(t.data), en || et(!0), F(selectSingleNode(t.id, z)), centerNode(t)) : F(selectNode(t.id, z)))
                             },
                             onNodeMouseEnter: (e, n) => {
                                 if (P && void 0 !== H) {
                                     let [e, t] = highlightPath(P, H, z, O, n.id);
-                                    M(e), A(t)
+                                    F(e), A(t)
                                 }
                             },
                             onNodeMouseLeave: (e, n) => {
                                 if (P && void 0 !== H) {
                                     let [e, n] = highlightPath(P, H, z, O, null);
-                                    M(e), A(n)
+                                    F(e), A(n)
                                 }
                             },
                             onNodeContextMenu: (e, n) => {
                                 "action" === X && (e.preventDefault(), ec({
                                     x: e.clientX,
                                     y: e.clientY,
                                     selectedNode: n
@@ -4275,208 +4385,208 @@
                             },
                             onClick: closeContextMenu,
                             maxZoom: 1,
                             minZoom: .1,
                             fitView: !0,
                             nodesDraggable: n.interactive,
                             ref: I,
-                            children: [(0, i.jsx)(_.A, {
+                            children: [(0, r.jsx)(_.A, {
                                 color: "#ccc"
-                            }), (0, i.jsxs)(R.Z, {
+                            }), (0, r.jsxs)(R.Z, {
                                 showInteractive: !1,
                                 position: "top-right",
                                 className: ek,
-                                children: [n.interactive && (0, i.jsxs)(i.Fragment, {
-                                    children: [(0, i.jsx)(R.B, {
+                                children: [n.interactive && (0, r.jsxs)(r.Fragment, {
+                                    children: [(0, r.jsx)(R.B, {
                                         title: "switch mode",
                                         onClick: () => {
-                                            er("all" === ei ? "changed_models" : "all");
+                                            ei("all" === er ? "changed_models" : "all");
                                             let e = cleanUpSelectedNodes(z);
-                                            M(e)
+                                            F(e)
                                         },
-                                        children: (0, i.jsx)(s.J, {
+                                        children: (0, r.jsx)(s.J, {
                                             as: B.Bw1
                                         })
-                                    }), (0, i.jsx)(R.B, {
+                                    }), (0, r.jsx)(R.B, {
                                         title: "summary",
                                         onClick: J,
-                                        children: (0, i.jsx)(s.J, {
+                                        children: (0, r.jsx)(s.J, {
                                             as: B.SnF
                                         })
                                     })]
-                                }), (0, i.jsx)(R.B, {
+                                }), (0, r.jsx)(R.B, {
                                     title: "copy image",
                                     onClick: () => {
                                         L()
                                     },
-                                    children: (0, i.jsx)(s.J, {
+                                    children: (0, r.jsx)(s.J, {
                                         as: B.C3L
                                     })
                                 })]
-                            }), (0, i.jsx)(r.s_, {
+                            }), (0, r.jsx)(i.s_, {
                                 position: "bottom-left",
-                                children: (0, i.jsxs)(x.U, {
-                                    children: [(0, i.jsx)(ChangeStatusLegend, {}), n.interactive && (0, i.jsxs)(l.xu, {
+                                children: (0, r.jsxs)(x.U, {
+                                    children: [(0, r.jsx)(ChangeStatusLegend, {}), n.interactive && (0, r.jsxs)(l.xu, {
                                         p: 2,
                                         flex: "0 1 160px",
                                         fontSize: "14px",
                                         className: ek,
-                                        children: [(0, i.jsx)(f.x, {
+                                        children: [(0, r.jsx)(f.x, {
                                             color: "gray",
                                             mb: "2px",
                                             children: "Actions"
-                                        }), (0, i.jsxs)(h.g, {
+                                        }), (0, r.jsxs)(h.g, {
                                             spacing: 1,
                                             align: "baseline",
-                                            children: [(0, i.jsx)(m.z, {
+                                            children: [(0, r.jsx)(m.z, {
                                                 size: "xs",
                                                 variant: "outline",
                                                 backgroundColor: "white",
                                                 isDisabled: "detail" !== X,
                                                 onClick: () => {
                                                     ee(void 0), et(!1);
                                                     let e = cleanUpSelectedNodes(z);
-                                                    M(e), Y("detail" === X ? "action" : "detail")
+                                                    F(e), Y("detail" === X ? "action" : "detail")
                                                 },
                                                 children: "Select Models"
-                                            }), (0, i.jsx)(AddLineageDiffCheckButton, {
-                                                viewMode: ei,
+                                            }), (0, r.jsx)(AddLineageDiffCheckButton, {
+                                                viewMode: er,
                                                 nodes: z.map(e => e.data),
                                                 onFinish: () => Y("detail")
                                             })]
                                         })]
                                     })]
                                 })
-                            }), (0, i.jsx)(r.s_, {
+                            }), (0, r.jsx)(i.s_, {
                                 position: "top-left",
-                                children: (0, i.jsx)(f.x, {
+                                children: (0, r.jsx)(f.x, {
                                     fontSize: "xl",
                                     color: "grey",
                                     opacity: .5,
-                                    children: e8[ei]
+                                    children: nr[er]
                                 })
-                            }), (0, i.jsx)(r.s_, {
+                            }), (0, r.jsx)(i.s_, {
                                 position: "bottom-center",
                                 className: ek,
-                                children: (0, i.jsx)(p.R, {
+                                children: (0, r.jsx)(p.R, {
                                     in: "detail" !== X,
                                     unmountOnExit: !0,
                                     style: {
                                         zIndex: 10
                                     },
-                                    children: (0, i.jsx)(NodeSelector, {
-                                        viewMode: ei,
+                                    children: (0, r.jsx)(NodeSelector, {
+                                        viewMode: er,
                                         nodes: z.map(e => e.data).filter(e => e.isSelected),
                                         onClose: () => {
                                             Y("detail");
                                             let e = cleanUpSelectedNodes(z);
-                                            ee(void 0), et(!1), M(e)
+                                            ee(void 0), et(!1), F(e)
                                         },
                                         onActionStarted: () => {
                                             Y("action_result")
                                         },
                                         onActionNodeUpdated: ed,
                                         onActionCompleted: () => {}
                                     })
                                 })
-                            }), (0, i.jsx)(D.a, {
+                            }), (0, r.jsx)(D.a, {
                                 nodeColor: nodeColor,
                                 nodeStrokeWidth: 3
                             })]
                         })
-                    }), (0, i.jsxs)(g.u_, {
+                    }), (0, r.jsxs)(g.u_, {
                         isOpen: Q,
                         onClose: Z,
                         size: "6xl",
-                        children: [(0, i.jsx)(v.Z, {}), (0, i.jsxs)(j.h, {
+                        children: [(0, r.jsx)(j.Z, {}), (0, r.jsxs)(y.h, {
                             overflowY: "auto",
                             height: "80%",
-                            children: [(0, i.jsx)(y.o, {}), (0, i.jsx)(C.f, {
-                                children: (0, i.jsx)(SummaryView, {})
+                            children: [(0, r.jsx)(v.o, {}), (0, r.jsx)(C.f, {
+                                children: (0, r.jsx)(SummaryView, {})
                             })]
                         })]
-                    }), "detail" === X && $ && (0, i.jsx)(l.xu, {
+                    }), "detail" === X && $ && (0, r.jsx)(l.xu, {
                         flex: "0 0 500px",
                         borderLeft: "solid 1px lightgray",
                         height: "100%",
-                        children: (0, i.jsx)(NodeView, {
+                        children: (0, r.jsx)(NodeView, {
                             node: $,
                             onCloseNode: () => {
-                                ee(void 0), et(!1), M(cleanUpSelectedNodes(z))
+                                ee(void 0), et(!1), F(cleanUpSelectedNodes(z))
                             }
                         })
-                    }), "action_result" === X && $ && (0, i.jsx)(l.xu, {
+                    }), "action_result" === X && $ && (0, r.jsx)(l.xu, {
                         flex: "0 0 500px",
                         borderLeft: "solid 1px lightgray",
                         height: "100%",
-                        children: (0, i.jsx)(NodeRunView, {
+                        children: (0, r.jsx)(NodeRunView, {
                             node: $,
                             onCloseNode: () => {
                                 ee(void 0), et(!1)
                             }
                         })
-                    }), eo && (0, i.jsx)(b.v, {
+                    }), eo && (0, r.jsx)(b.v, {
                         isOpen: !0,
                         onClose: closeContextMenu,
-                        children: (0, i.jsxs)(k.q, {
+                        children: (0, r.jsxs)(k.q, {
                             style: {
                                 position: "absolute",
                                 left: "".concat(es.x, "px"),
                                 top: "".concat(es.y, "px")
                             },
-                            children: [(0, i.jsx)(w.s, {
-                                icon: (0, i.jsx)(el.Cv2, {}),
+                            children: [(0, r.jsx)(w.s, {
+                                icon: (0, r.jsx)(el.Cv2, {}),
                                 onClick: () => {
                                     let e = es.selectedNode;
                                     if ("action" !== X || void 0 === e || void 0 === P) return;
                                     let n = e.id,
                                         t = selectUpstream(P, [n]),
-                                        i = selectNodes([...t], z);
-                                    M(i)
+                                        r = selectNodes([...t], z);
+                                    F(r)
                                 },
                                 children: "Select parent nodes"
-                            }), (0, i.jsx)(w.s, {
-                                icon: (0, i.jsx)(el.IMj, {}),
+                            }), (0, r.jsx)(w.s, {
+                                icon: (0, r.jsx)(el.IMj, {}),
                                 onClick: () => {
                                     let e = es.selectedNode;
                                     if ("action" !== X || void 0 === e || void 0 === P) return;
                                     let n = e.id,
                                         t = selectDownstream(P, [n]),
-                                        i = selectNodes([...t], z);
-                                    M(i)
+                                        r = selectNodes([...t], z);
+                                    F(r)
                                 },
                                 children: "Select child nodes"
                             })]
                         })
                     })]
                 })
             }
 
             function LineageView(e) {
                 let {
                     ...n
                 } = e;
-                return void 0 === n.interactive && (n.interactive = !0), void 0 === n.viewMode && (n.viewMode = "changed_models"), (0, i.jsx)(r.tV, {
-                    children: (0, i.jsx)(_LineageView, {
+                return void 0 === n.interactive && (n.interactive = !0), void 0 === n.viewMode && (n.viewMode = "changed_models"), (0, r.jsx)(i.tV, {
+                    children: (0, r.jsx)(_LineageView, {
                         ...n
                     })
                 })
             }
-            var e7 = t(12844),
-                ne = t(98786);
+            var ni = t(12844),
+                nl = t(98786);
 
             function RecceContextProvider(e) {
                 let {
                     children: n
                 } = e;
-                return (0, i.jsx)(i.Fragment, {
-                    children: (0, i.jsx)(RecceQueryContextProvider, {
-                        children: (0, i.jsx)(LineageGraphsContextProvider, {
-                            children: (0, i.jsx)(RowCountStateContextProvider, {
-                                children: (0, i.jsx)(RecceActionContextProvider, {
+                return (0, r.jsx)(r.Fragment, {
+                    children: (0, r.jsx)(RecceQueryContextProvider, {
+                        children: (0, r.jsx)(LineageGraphsContextProvider, {
+                            children: (0, r.jsx)(RowCountStateContextProvider, {
+                                children: (0, r.jsx)(RecceActionContextProvider, {
                                     children: n
                                 })
                             })
                         })
                     })
                 })
             }
@@ -4490,69 +4600,69 @@
                             n(e.data)
                         } catch (e) {
                             console.error("Error fetching version number:", e)
                         }
                     })()
                 }, []), e
             }
-            var nn = t(45489),
-                nt = t(69005),
-                ni = t(14800),
-                nr = t(2600),
-                nl = t(68677),
-                no = t(83358),
-                na = t(44525),
-                ns = t(79935),
-                nc = t(93197),
-                nd = t(234),
-                nu = t(96094),
-                nh = t(36334);
+            var no = t(45489),
+                na = t(69005),
+                ns = t(14800),
+                nc = t(2600),
+                nd = t(68677),
+                nu = t(83358),
+                nh = t(44525),
+                nm = t(79935),
+                nx = t(93197),
+                nf = t(234),
+                np = t(96094),
+                ng = t(36334);
 
             function CheckBreadcrumb(e) {
                 let {
                     name: n,
                     setName: t
-                } = e, [r, o] = (0, S.useState)(!1), [a, s] = (0, S.useState)(n), c = (0, S.useRef)(null), d = (0, S.useCallback)(() => {
+                } = e, [i, o] = (0, S.useState)(!1), [a, s] = (0, S.useState)(n), c = (0, S.useRef)(null), d = (0, S.useCallback)(() => {
                     t(a), o(!1)
                 }, [t, o, a]);
                 return (0, S.useEffect)(() => {
                     let handleClickOutside = e => {
                         c.current && !c.current.contains(e.target) && d()
                     };
-                    return r && document.addEventListener("mousedown", handleClickOutside), () => {
+                    return i && document.addEventListener("mousedown", handleClickOutside), () => {
                         document.removeEventListener("mousedown", handleClickOutside)
                     }
-                }, [r, c, d]), (0, i.jsxs)(nd.a, {
+                }, [i, c, d]), (0, r.jsxs)(nf.a, {
                     flex: "0 1",
                     fontSize: "12pt",
                     fontWeight: "500",
-                    separator: (0, i.jsx)(nh.X, {
+                    separator: (0, r.jsx)(ng.X, {
                         color: "gray.500"
                     }),
-                    children: [(0, i.jsx)(nu.g, {
-                        children: (0, i.jsx)(l.xu, {
+                    children: [(0, r.jsx)(np.g, {
+                        children: (0, r.jsx)(l.xu, {
                             children: "Checklist"
                         })
-                    }), (0, i.jsx)(nu.g, {
+                    }), (0, r.jsx)(np.g, {
                         flex: "0 1",
                         cursor: "pointer",
-                        children: r ? (0, i.jsx)(ez.I, {
+                        children: i ? (0, r.jsx)(ez.I, {
                             ref: c,
                             value: a,
                             onChange: e => {
                                 s(e.target.value)
                             },
                             onKeyDown: e => {
                                 "Enter" === e.key ? (t(a), o(!1)) : "Escape" === e.key && (s(n), o(!1))
                             },
                             size: "sm",
                             w: "auto",
                             minW: "200px",
                             maxW: "600px"
-                        }) : (0, i.jsx)(l.xu, {
+                        }) : (0, r.jsx)(l.xu, {
                             onClick: () => {
                                 s(n), o(!0)
                             },
                             textOverflow: "ellipsis",
                             whiteSpace: "nowrap",
                             overflow: "hidden",
                             children: n
@@ -4562,83 +4672,83 @@
             }
 
             function SchemaDiffView(e) {
                 let {
                     check: n
                 } = e, {
                     lineageGraphSets: t
-                } = useLineageGraphsContext(), r = n.params, l = r.node_id, o = l ? null == t ? void 0 : t.all.nodes[l] : void 0;
-                return o ? (0, i.jsx)(SchemaView, {
+                } = useLineageGraphsContext(), i = n.params, l = i.node_id, o = l ? null == t ? void 0 : t.all.nodes[l] : void 0;
+                return o ? (0, r.jsx)(SchemaView, {
                     base: o.data.base,
                     current: o.data.current,
                     enableScreenshot: !0
-                }) : (0, i.jsx)(i.Fragment, {})
+                }) : (0, r.jsx)(r.Fragment, {})
             }
-            var nm = t(33695);
+            var nj = t(33695);
 
             function CheckDescription(e) {
                 let {
                     value: n,
                     onChange: t
-                } = e, [r, l] = (0, S.useState)(!1), [o, s] = (0, S.useState)(), c = (0, S.useRef)(null);
+                } = e, [i, l] = (0, S.useState)(!1), [o, s] = (0, S.useState)(), c = (0, S.useRef)(null);
                 return ((0, S.useEffect)(() => {
-                    if (r && c.current) {
+                    if (i && c.current) {
                         let e = c.current;
                         e.focus(), e.setSelectionRange(e.value.length, e.value.length)
                     }
-                }, [r]), r) ? (0, i.jsxs)(a.k, {
+                }, [i]), i) ? (0, r.jsxs)(a.k, {
                     direction: "column",
                     align: "flex-end",
-                    children: [(0, i.jsx)(nm.g, {
+                    children: [(0, r.jsx)(nj.g, {
                         h: "200px",
                         value: o,
                         onChange: e => {
                             s(e.target.value)
                         },
                         onKeyDown: e => {
                             "Escape" === e.key && l(!1)
                         },
                         ref: c
-                    }), (0, i.jsxs)(a.k, {
+                    }), (0, r.jsxs)(a.k, {
                         gap: "12px",
                         alignItems: "flex-end",
-                        children: [(0, i.jsx)(eK.r, {
+                        children: [(0, r.jsx)(eH.r, {
                             onClick: () => {
                                 setTimeout(() => {
                                     l(!1)
                                 }, 100)
                             },
                             colorScheme: "blue",
                             children: "cancel"
-                        }), (0, i.jsx)(m.z, {
+                        }), (0, r.jsx)(m.z, {
                             mt: "8px",
                             size: "sm",
                             colorScheme: "blue",
                             onClick: () => {
                                 t && (t(o), l(!1))
                             },
                             children: "Update"
                         })]
                     })]
-                }) : (0, i.jsx)(f.x, {
+                }) : (0, r.jsx)(f.x, {
                     maxHeight: "400px",
                     overflow: "auto",
                     fontSize: "11pt",
                     onClick: () => {
                         s(n || ""), l(!0)
                     },
                     whiteSpace: "pre-line",
                     color: n ? "inherit" : "lightgray",
                     children: n || "Add description here"
                 })
             }
-            var nx = t(48742);
+            var ny = t(48742);
 
             function _templateObject() {
-                let e = (0, nn._)(["\n    **SQL**\n    ```sql\n    ", "\n    ```\n    "], ["\n    **SQL**\n    \\`\\`\\`sql\n    ", "\n    \\`\\`\\`\n    "]);
+                let e = (0, no._)(["\n    **SQL**\n    ```sql\n    ", "\n    ```\n    "], ["\n    **SQL**\n    \\`\\`\\`sql\n    ", "\n    \\`\\`\\`\n    "]);
                 return _templateObject = function() {
                     return e
                 }, e
             }
 
             function buildTitle(e) {
                 return "".concat(e.is_checked ? "✅ " : "").concat(e.name)
@@ -4646,34 +4756,34 @@
 
             function buildDescription(e) {
                 return e.description ? e.description : "_(no description)_"
             }
 
             function buildQuery(e) {
                 var n;
-                return (0, nx.Pn)(_templateObject(), null === (n = e.params) || void 0 === n ? void 0 : n.sql_template)
+                return (0, ny.Pn)(_templateObject(), null === (n = e.params) || void 0 === n ? void 0 : n.sql_template)
             }
             var query_SqlEditor = e => {
                 let {
                     value: n,
                     onChange: t,
-                    onRun: r,
+                    onRun: i,
                     onRunDiff: l,
                     options: o = {},
                     ...a
                 } = e;
-                return (0, i.jsx)(eD.ZP, {
+                return (0, r.jsx)(eD.ZP, {
                     language: "sql",
                     theme: "vs",
                     value: n,
                     onChange: e => {
                         void 0 !== e && t && t(e)
                     },
                     onMount: (e, n) => {
-                        r && e.addCommand(n.KeyMod.CtrlCmd | n.KeyCode.Enter, r), l && e.addCommand(n.KeyMod.CtrlCmd | n.KeyMod.Shift | n.KeyCode.Enter, l)
+                        i && e.addCommand(n.KeyMod.CtrlCmd | n.KeyCode.Enter, i), l && e.addCommand(n.KeyMod.CtrlCmd | n.KeyMod.Shift | n.KeyCode.Enter, l)
                     },
                     options: {
                         tabSize: 2,
                         fontSize: 16,
                         lineNumbers: "on",
                         automaticLayout: !0,
                         minimap: {
@@ -4686,231 +4796,237 @@
                 })
             };
 
             function DataFrameColumnHeader(e) {
                 let {
                     name: n,
                     pinnedColumns: t = [],
-                    onPinnedColumnsChange: r = () => {}
+                    onPinnedColumnsChange: i = () => {}
                 } = e, o = t.includes(n);
-                return (0, i.jsxs)(a.k, {
+                return (0, r.jsxs)(a.k, {
                     className: "grid-header",
                     alignItems: "center",
-                    children: [(0, i.jsx)(l.xu, {
+                    children: [(0, r.jsx)(l.xu, {
                         flex: 1,
                         children: n
-                    }), (0, i.jsx)(s.J, {
+                    }), (0, r.jsx)(s.J, {
                         className: o ? "unpin-icon" : "pin-icon",
                         display: o ? "block" : "none",
                         cursor: "pointer",
                         as: o ? L.$kI : L.oJP,
                         onClick: o ? () => {
                             let e = t.filter(e => e !== n);
-                            r(e)
+                            i(e)
                         } : () => {
                             let e = [...t, n];
-                            r(e)
+                            i(e)
                         }
                     })]
                 })
             }
 
             function QueryResultView_toDataGrid(e, n) {
                 let t = [],
-                    r = n.pinnedColumns || [],
+                    i = n.pinnedColumns || [],
                     toColumn = (e, t) => ({
                         key: String(e),
-                        name: (0, i.jsx)(DataFrameColumnHeader, {
+                        name: (0, r.jsx)(DataFrameColumnHeader, {
                             name: t,
                             ...n
                         }),
                         width: "auto",
                         renderCell: defaultRenderCell
                     });
                 return t.push({
                     key: "_index",
                     name: "",
                     width: 10,
                     cellClass: "index-column"
-                }), r.forEach(n => {
-                    let i = eA().findIndex(e.columns, e => e.name === n);
-                    i < 0 || t.push(toColumn(i, n))
+                }), i.forEach(n => {
+                    let r = eA().findIndex(e.columns, e => e.name === n);
+                    r < 0 || t.push(toColumn(r, n))
                 }), e.columns.forEach((e, n) => {
-                    r.includes(e.name) || t.push(toColumn(n, e.name))
+                    i.includes(e.name) || t.push(toColumn(n, e.name))
                 }), e.data.forEach((e, n) => {
                     e._index = n + 1
                 }), {
                     columns: t,
                     rows: e.data
                 }
             }
             let QueryResultView = e => {
                     let {
                         run: n,
                         viewOptions: t,
-                        onViewOptionsChanged: r,
+                        onViewOptionsChanged: i,
                         onAddToChecklist: s
                     } = e, c = (0, S.useMemo)(() => (null == t ? void 0 : t.pinned_columns) || [], [t]), d = null == n ? void 0 : n.result, h = (0, S.useMemo)(() => d ? QueryResultView_toDataGrid(d, {
                         pinnedColumns: c,
                         onPinnedColumnsChange: e => {
-                            r && r({
+                            i && i({
                                 ...t,
                                 pinned_columns: e
                             })
                         }
                     }) : {
                         rows: [],
                         columns: []
-                    }, [d, c, t, r]);
-                    if (0 === h.columns.length) return (0, i.jsx)(u.M, {
+                    }, [d, c, t, i]);
+                    if (0 === h.columns.length) return (0, r.jsx)(u.M, {
                         height: "100%",
                         children: "No data"
                     });
                     let m = (null == d ? void 0 : d.limit) || 0,
                         x = m > 0 && (null == d ? void 0 : d.more) ? "Warning: Displayed results are limited to ".concat(m.toLocaleString(), " records. To ensure complete data retrieval, consider applying a LIMIT or WHERE clause to constrain the result set.") : null;
-                    return (0, i.jsxs)(a.k, {
+                    return (0, r.jsxs)(a.k, {
                         direction: "column",
                         backgroundColor: "rgb(249, 249, 249)",
                         height: "100%",
-                        children: [(s || x) && (0, i.jsxs)(a.k, {
+                        children: [(s || x) && (0, r.jsxs)(a.k, {
                             borderBottom: "1px solid lightgray",
                             alignItems: "center",
                             gap: "5px",
                             px: "10px",
                             bg: x ? "orange.100" : "inherit",
-                            children: [x && (0, i.jsxs)(i.Fragment, {
-                                children: [(0, i.jsx)(ei.a, {
+                            children: [x && (0, r.jsxs)(r.Fragment, {
+                                children: [(0, r.jsx)(er.a, {
                                     color: "orange.600",
                                     alignSelf: "center"
-                                }), " ", (0, i.jsx)(l.xu, {
+                                }), " ", (0, r.jsx)(l.xu, {
                                     children: x
                                 })]
-                            }), (0, i.jsx)(E.L, {
+                            }), (0, r.jsx)(E.L, {
                                 minHeight: "32px"
-                            }), s && (0, i.jsx)(o.u, {
+                            }), s && (0, r.jsx)(o.u, {
                                 label: "Add to Checklist",
-                                children: (0, i.jsx)(P.h, {
+                                children: (0, r.jsx)(P.h, {
                                     variant: "unstyled",
                                     size: "sm",
                                     "aria-label": "Add",
-                                    icon: (0, i.jsx)(eq.d, {}),
+                                    icon: (0, r.jsx)(eq.d, {}),
                                     onClick: () => s(n)
                                 })
                             })]
-                        }), (0, i.jsx)(ScreenshotDataGrid, {
+                        }), (0, r.jsx)(ScreenshotDataGrid, {
                             style: {
                                 blockSize: "auto",
                                 maxHeight: "100%",
                                 overflow: "auto"
                             },
                             columns: h.columns,
                             rows: h.rows,
+                            renderers: {
+                                noRowsFallback: (0, r.jsx)(EmptyRowsRenderer, {})
+                            },
                             defaultColumnOptions: {
                                 resizable: !0,
                                 maxWidth: 800,
                                 minWidth: 35
                             },
                             className: "rdg-light",
                             enableScreenshot: !0
                         })]
                     })
                 },
                 QueryDiffResultView = e => {
-                    var n, t, r, s, c, d;
+                    var n, t, i, s, c, d;
                     let {
                         run: m,
                         onAddToChecklist: x,
                         viewOptions: f,
                         onViewOptionsChanged: p
-                    } = e, g = (0, S.useMemo)(() => (null == f ? void 0 : f.primary_keys) || [], [f]), v = (0, S.useMemo)(() => (null == f ? void 0 : f.changed_only) || !1, [f]), j = (0, S.useMemo)(() => (null == f ? void 0 : f.pinned_columns) || [], [f]), y = (0, S.useMemo)(() => {
+                    } = e, g = (0, S.useMemo)(() => (null == f ? void 0 : f.primary_keys) || [], [f]), j = (0, S.useMemo)(() => (null == f ? void 0 : f.changed_only) || !1, [f]), y = (0, S.useMemo)(() => (null == f ? void 0 : f.pinned_columns) || [], [f]), v = (0, S.useMemo)(() => {
                         var e, n;
                         return toDataDiffGrid(null == m ? void 0 : null === (e = m.result) || void 0 === e ? void 0 : e.base, null == m ? void 0 : null === (n = m.result) || void 0 === n ? void 0 : n.current, {
-                            changedOnly: v,
+                            changedOnly: j,
                             primaryKeys: g,
                             onPrimaryKeyChange: e => {
                                 p && p({
                                     ...f,
                                     primary_keys: e
                                 })
                             },
-                            pinnedColumns: j,
+                            pinnedColumns: y,
                             onPinnedColumnsChange: e => {
                                 p && p({
                                     ...f,
                                     pinned_columns: e
                                 })
                             }
                         })
-                    }, [m, f, v, g, j, p]), C = (0, S.useMemo)(() => {
+                    }, [m, f, j, g, y, p]), C = (0, S.useMemo)(() => {
                         let e = g.join(", ");
-                        return y.invalidPKeyBase && y.invalidPKeyCurrent ? "Warning: The primary key '".concat(e, "' is not unique in the base and current environments") : y.invalidPKeyBase ? "Warning: The primary key '".concat(e, "' is not unique in the base environment") : y.invalidPKeyCurrent ? "Warning: The primary key '".concat(e, "' is not unique in the current environment") : void 0
-                    }, [y.invalidPKeyBase, y.invalidPKeyCurrent, g]);
-                    if (0 === y.columns.length) return (0, i.jsx)(u.M, {
+                        return v.invalidPKeyBase && v.invalidPKeyCurrent ? "Warning: The primary key '".concat(e, "' is not unique in the base and current environments") : v.invalidPKeyBase ? "Warning: The primary key '".concat(e, "' is not unique in the base environment") : v.invalidPKeyCurrent ? "Warning: The primary key '".concat(e, "' is not unique in the current environment") : void 0
+                    }, [v.invalidPKeyBase, v.invalidPKeyCurrent, g]);
+                    if (0 === v.columns.length) return (0, r.jsx)(u.M, {
                         height: "100%",
                         children: "No data"
                     });
-                    if (v && 0 === y.rows.length) return (0, i.jsx)(u.M, {
+                    if (j && 0 === v.rows.length) return (0, r.jsx)(u.M, {
                         height: "100%",
                         children: "No change"
                     });
                     let b = (null === (t = m.result) || void 0 === t ? void 0 : null === (n = t.current) || void 0 === n ? void 0 : n.limit) || 0,
-                        k = b > 0 && ((null == m ? void 0 : null === (s = m.result) || void 0 === s ? void 0 : null === (r = s.current) || void 0 === r ? void 0 : r.more) || (null == m ? void 0 : null === (d = m.result) || void 0 === d ? void 0 : null === (c = d.base) || void 0 === c ? void 0 : c.more)) ? "Warning: Displayed results are limited to ".concat(b.toLocaleString(), " records. To ensure complete data retrieval, consider applying a LIMIT or WHERE clause to constrain the result set.") : null;
-                    return (0, i.jsxs)(a.k, {
+                        k = b > 0 && ((null == m ? void 0 : null === (s = m.result) || void 0 === s ? void 0 : null === (i = s.current) || void 0 === i ? void 0 : i.more) || (null == m ? void 0 : null === (d = m.result) || void 0 === d ? void 0 : null === (c = d.base) || void 0 === c ? void 0 : c.more)) ? "Warning: Displayed results are limited to ".concat(b.toLocaleString(), " records. To ensure complete data retrieval, consider applying a LIMIT or WHERE clause to constrain the result set.") : null;
+                    return (0, r.jsxs)(a.k, {
                         direction: "column",
                         backgroundColor: "rgb(249, 249, 249)",
                         height: "100%",
-                        children: [(0, i.jsxs)(a.k, {
+                        children: [(0, r.jsxs)(a.k, {
                             borderBottom: "1px solid lightgray",
                             justifyContent: "flex-end",
                             gap: "5px",
                             alignItems: "center",
                             px: "10px",
                             bg: k || C ? "orange.100" : "inherit",
-                            children: [(0, i.jsxs)(h.g, {
+                            children: [(0, r.jsxs)(h.g, {
                                 alignItems: "flex-start",
                                 spacing: 0,
-                                children: [C && (0, i.jsxs)(l.xu, {
-                                    children: [(0, i.jsx)(ei.a, {
+                                children: [C && (0, r.jsxs)(l.xu, {
+                                    children: [(0, r.jsx)(er.a, {
                                         color: "orange.600"
                                     }), " ", C]
-                                }), k && (0, i.jsxs)(l.xu, {
-                                    children: [(0, i.jsx)(ei.a, {
+                                }), k && (0, r.jsxs)(l.xu, {
+                                    children: [(0, r.jsx)(er.a, {
                                         color: "orange.600"
                                     }), " ", k]
                                 })]
-                            }), (0, i.jsx)(E.L, {
+                            }), (0, r.jsx)(E.L, {
                                 minHeight: "32px"
-                            }), (0, i.jsx)(eM.X, {
+                            }), (0, r.jsx)(eF.X, {
                                 isChecked: null == f ? void 0 : f.changed_only,
                                 onChange: () => {
                                     let e = !(null == f ? void 0 : f.changed_only);
                                     p && p({
                                         ...f,
                                         changed_only: e
                                     })
                                 },
                                 children: "Changed only"
-                            }), x && (0, i.jsx)(o.u, {
+                            }), x && (0, r.jsx)(o.u, {
                                 label: "Add to Checklist",
-                                children: (0, i.jsx)(P.h, {
+                                children: (0, r.jsx)(P.h, {
                                     variant: "unstyled",
                                     size: "sm",
                                     "aria-label": "Add",
-                                    icon: (0, i.jsx)(eq.d, {}),
+                                    icon: (0, r.jsx)(eq.d, {}),
                                     onClick: () => x(m)
                                 })
                             })]
-                        }), (0, i.jsx)(ScreenshotDataGrid, {
+                        }), (0, r.jsx)(ScreenshotDataGrid, {
                             style: {
                                 blockSize: "auto",
                                 maxHeight: "100%",
                                 overflow: "auto"
                             },
-                            columns: y.columns,
-                            rows: y.rows,
+                            columns: v.columns,
+                            rows: v.rows,
+                            renderers: {
+                                noRowsFallback: (0, r.jsx)(EmptyRowsRenderer, {})
+                            },
                             defaultColumnOptions: {
                                 resizable: !0,
                                 maxWidth: 800,
                                 minWidth: 35
                             },
                             className: "rdg-light",
                             enableScreenshot: !0
@@ -4918,124 +5034,124 @@
                     })
                 };
 
             function LineageDiffView(e) {
                 var n;
                 let {
                     check: t
-                } = e, r = (null === (n = t.params) || void 0 === n ? void 0 : n.view_mode) || "";
-                return (0, i.jsx)(a.k, {
+                } = e, i = (null === (n = t.params) || void 0 === n ? void 0 : n.view_mode) || "";
+                return (0, r.jsx)(a.k, {
                     direction: "column",
                     height: "100%",
-                    children: (0, i.jsx)(LineageView, {
-                        viewMode: r,
+                    children: (0, r.jsx)(LineageView, {
+                        viewMode: i,
                         interactive: !1,
                         filterNodes: e => {
-                            var n, i;
-                            return null === (i = t.params) || void 0 === i ? void 0 : null === (n = i.node_ids) || void 0 === n ? void 0 : n.includes(e)
+                            var n, r;
+                            return null === (r = t.params) || void 0 === r ? void 0 : null === (n = r.node_ids) || void 0 === n ? void 0 : n.includes(e)
                         }
                     })
                 })
             }
 
             function CheckDetail_templateObject() {
-                let e = (0, nn._)(["\n  <details><summary>", "</summary>\n\n  ", "\n\n  </details>"]);
+                let e = (0, no._)(["\n  <details><summary>", "</summary>\n\n  ", "\n\n  </details>"]);
                 return CheckDetail_templateObject = function() {
                     return e
                 }, e
             }
-            let nf = {
+            let nv = {
                     query: QueryResultView,
                     query_diff: QueryDiffResultView,
                     value_diff: ValueDiffResultView,
                     value_diff_detail: ValueDiffDetailResultView,
                     profile_diff: ProfileDiffResultView,
                     row_count_diff: RowCountDiffResultView,
                     top_k_diff: TopKDiffResultView,
                     histogram_diff: HistogramDiffResultView
                 },
                 useCancelOnUnmount = e => {
                     let {
                         runId: n,
                         isPending: t,
-                        setAborting: i
+                        setAborting: r
                     } = e;
                     (0, S.useEffect)(() => () => {
-                        i(!1), n && t && cancelRun(n)
-                    }, [t, n, i])
+                        r(!1), n && t && cancelRun(n)
+                    }, [t, n, r])
                 },
                 CheckDetail = e => {
                     var n;
                     let {
                         checkId: t
-                    } = e, r = (0, H.NL)(), [, c] = (0, eT.TH)(), {
+                    } = e, i = (0, H.NL)(), [, c] = (0, eN.TH)(), {
                         successToast: d,
                         failToast: h
-                    } = useClipBoardToast(), [x, f] = (0, S.useState)(), [p, g] = (0, S.useState)(), [v, j] = (0, S.useState)(!1), {
-                        isLoading: y,
+                    } = useClipBoardToast(), [x, f] = (0, S.useState)(), [p, g] = (0, S.useState)(), [j, y] = (0, S.useState)(!1), {
+                        isLoading: v,
                         error: C,
                         refetch: _,
                         data: R
                     } = (0, ee.a)({
                         queryKey: Z.check(t),
                         queryFn: async () => getCheck(t),
                         refetchOnMount: !1,
                         staleTime: 3e5
-                    }), D = R && (null == R ? void 0 : R.type) in nf ? nf[null == R ? void 0 : R.type] : void 0, {
-                        mutate: T
+                    }), D = R && (null == R ? void 0 : R.type) in nv ? nv[null == R ? void 0 : R.type] : void 0, {
+                        mutate: N
                     } = (0, eP.D)({
                         mutationFn: e => updateCheck(t, e),
                         onSuccess: () => {
-                            r.invalidateQueries({
+                            i.invalidateQueries({
                                 queryKey: Z.check(t)
-                            }), r.invalidateQueries({
+                            }), i.invalidateQueries({
                                 queryKey: Z.checks()
                             })
                         }
                     }), {
-                        mutate: N
+                        mutate: T
                     } = (0, eP.D)({
                         mutationFn: () => deleteCheck(t),
                         onSuccess: () => {
-                            r.invalidateQueries({
+                            i.invalidateQueries({
                                 queryKey: Z.checks()
                             }), c("/checks")
                         }
                     }), submitRunFn = async () => {
                         let e = null == R ? void 0 : R.type;
                         if (!e) return;
                         let {
                             run_id: n
                         } = await submitRunFromCheck(t, {
                             nowait: !0
                         });
                         for (f(n);;) {
                             let e = await waitRun(n, 2);
-                            if (g(e.progress), e.result || e.error) return j(!1), g(void 0), e
+                            if (g(e.progress), e.result || e.error) return y(!1), g(void 0), e
                         }
                     }, {
                         data: I,
                         mutate: z,
-                        error: M,
-                        isIdle: F,
+                        error: F,
+                        isIdle: M,
                         isPending: O
                     } = (0, eP.D)({
                         mutationFn: submitRunFn,
                         onSuccess: e => {
                             _()
                         }
                     }), handleRerun = async () => {
                         z()
                     }, A = (0, S.useCallback)(async () => {
-                        if (j(!0), x) return await cancelRun(x)
+                        if (y(!0), x) return await cancelRun(x)
                     }, [x]);
                     useCancelOnUnmount({
                         runId: x,
                         isPending: O,
-                        setAborting: j
+                        setAborting: y
                     });
                     let handleCopy = async () => {
                         if (!R) return;
                         let e = buildMarkdown(R);
                         if (!navigator.clipboard) {
                             h("Failed to copy the check to clipboard", Error("Copy to clipboard is available only in secure contexts (HTTPS)"));
                             return
@@ -5043,278 +5159,278 @@
                         try {
                             await navigator.clipboard.writeText(e), d("Copied the check to the clipboard")
                         } catch (e) {
                             h("Failed to copy the check to clipboard", e)
                         }
                     }, V = (0, S.useCallback)(() => {
                         let e = null == R ? void 0 : R.is_checked;
-                        T({
+                        N({
                             is_checked: !e
                         })
-                    }, [null == R ? void 0 : R.is_checked, T]);
-                    if (y) return (0, i.jsx)(u.M, {
+                    }, [null == R ? void 0 : R.is_checked, N]);
+                    if (v) return (0, r.jsx)(u.M, {
                         h: "100%",
                         children: "Loading"
                     });
-                    if (C) return (0, i.jsxs)(u.M, {
+                    if (C) return (0, r.jsxs)(u.M, {
                         h: "100%",
                         children: ["Error: ", C.message]
                     });
-                    let B = F ? null == R ? void 0 : R.last_run : I,
+                    let B = M ? null == R ? void 0 : R.last_run : I,
                         q = (null == B ? void 0 : B.run_at) ? (0, eB.Z)(new Date(B.run_at), {
                             addSuffix: !0
                         }) : null;
-                    return (0, i.jsxs)(a.k, {
+                    return (0, r.jsxs)(a.k, {
                         height: "100%",
                         width: "100%",
                         maxHeight: "100%",
                         direction: "column",
-                        children: [(0, i.jsxs)(a.k, {
+                        children: [(0, r.jsxs)(a.k, {
                             p: "0px 16px",
                             alignItems: "center",
-                            children: [(0, i.jsx)(CheckBreadcrumb, {
+                            children: [(0, r.jsx)(CheckBreadcrumb, {
                                 name: (null == R ? void 0 : R.name) || "",
                                 setName: e => {
-                                    T({
+                                    N({
                                         name: e
                                     })
                                 }
-                            }), (0, i.jsx)(E.L, {}), (0, i.jsxs)(b.v, {
-                                children: [(0, i.jsx)(ef.j, {
+                            }), (0, r.jsx)(E.L, {}), (0, r.jsxs)(b.v, {
+                                children: [(0, r.jsx)(ef.j, {
                                     isRound: !0,
                                     as: P.h,
-                                    icon: (0, i.jsx)(s.J, {
+                                    icon: (0, r.jsx)(s.J, {
                                         as: L.D_A
                                     }),
                                     variant: "ghost"
-                                }), (0, i.jsx)(k.q, {
-                                    children: (0, i.jsx)(w.s, {
-                                        icon: (0, i.jsx)(na.p, {}),
-                                        onClick: () => N(),
+                                }), (0, r.jsx)(k.q, {
+                                    children: (0, r.jsx)(w.s, {
+                                        icon: (0, r.jsx)(nh.p, {}),
+                                        onClick: () => T(),
                                         children: "Delete"
                                     })
                                 })]
-                            }), q && (0, i.jsx)(l.xu, {
+                            }), q && (0, r.jsx)(l.xu, {
                                 textOverflow: "ellipsis",
                                 whiteSpace: "nowrap",
                                 overflow: "hidden",
                                 fontSize: "10pt",
                                 children: q
-                            }), R && (null == R ? void 0 : R.type) in nf && (0, i.jsx)(o.u, {
+                            }), R && (null == R ? void 0 : R.type) in nv && (0, r.jsx)(o.u, {
                                 label: "Rerun",
-                                children: (0, i.jsx)(P.h, {
+                                children: (0, r.jsx)(P.h, {
                                     isRound: !0,
                                     isLoading: O,
                                     variant: "ghost",
                                     "aria-label": "Rerun",
-                                    icon: (0, i.jsx)(ns.n, {}),
+                                    icon: (0, r.jsx)(nm.n, {}),
                                     onClick: () => handleRerun()
                                 })
-                            }), (0, i.jsx)(o.u, {
+                            }), (0, r.jsx)(o.u, {
                                 label: "Copy markdown",
-                                children: (0, i.jsx)(P.h, {
+                                children: (0, r.jsx)(P.h, {
                                     isRound: !0,
                                     variant: "ghost",
                                     "aria-label": "Copy markdown",
-                                    icon: (0, i.jsx)(ej.T, {}),
+                                    icon: (0, r.jsx)(ey.T, {}),
                                     onClick: () => handleCopy()
                                 })
-                            }), (0, i.jsx)(o.u, {
+                            }), (0, r.jsx)(o.u, {
                                 label: (null == R ? void 0 : R.is_checked) ? "Mark as unchecked" : "Mark as checked",
-                                children: (0, i.jsx)(m.z, {
+                                children: (0, r.jsx)(m.z, {
                                     size: "sm",
                                     colorScheme: (null == R ? void 0 : R.is_checked) ? "green" : "gray",
-                                    leftIcon: (0, i.jsx)(nc.r, {}),
+                                    leftIcon: (0, r.jsx)(nx.r, {}),
                                     onClick: () => V(),
                                     children: (null == R ? void 0 : R.is_checked) ? "Checked" : "Unchecked"
                                 })
                             })]
-                        }), (0, i.jsx)(l.xu, {
+                        }), (0, r.jsx)(l.xu, {
                             p: "8px 16px",
                             minHeight: "100px",
-                            children: (0, i.jsx)(CheckDescription, {
+                            children: (0, r.jsx)(CheckDescription, {
                                 value: null == R ? void 0 : R.description,
                                 onChange: e => {
-                                    T({
+                                    N({
                                         description: e
                                     })
                                 }
                             }, null == R ? void 0 : R.check_id)
-                        }), ((null == R ? void 0 : R.type) === "query" || (null == R ? void 0 : R.type) === "query_diff") && (0, i.jsx)(nt.U, {
+                        }), ((null == R ? void 0 : R.type) === "query" || (null == R ? void 0 : R.type) === "query_diff") && (0, r.jsx)(na.U, {
                             defaultIndex: [],
                             allowToggle: !0,
-                            children: (0, i.jsxs)(ni.Q, {
-                                children: [(0, i.jsxs)(nr.K, {
-                                    children: ["query", (0, i.jsx)(nl.X, {})]
-                                }), (0, i.jsx)(no.H, {
-                                    children: (0, i.jsx)(l.xu, {
+                            children: (0, r.jsxs)(ns.Q, {
+                                children: [(0, r.jsxs)(nc.K, {
+                                    children: ["query", (0, r.jsx)(nd.X, {})]
+                                }), (0, r.jsx)(nu.H, {
+                                    children: (0, r.jsx)(l.xu, {
                                         height: "400px",
                                         width: "100%",
                                         border: "lightgray 1px solid ",
-                                        children: (0, i.jsx)(query_SqlEditor, {
+                                        children: (0, r.jsx)(query_SqlEditor, {
                                             value: (null === (n = null == R ? void 0 : R.params) || void 0 === n ? void 0 : n.sql_template) || "",
                                             options: {
                                                 readOnly: !0
                                             }
                                         })
                                     })
                                 })]
                             })
-                        }), (0, i.jsxs)(l.xu, {
+                        }), (0, r.jsxs)(l.xu, {
                             style: {
                                 contain: "size"
                             },
                             flex: "1 1 0%",
-                            children: [D && (0, i.jsx)(RunView, {
+                            children: [D && (0, r.jsx)(RunView, {
                                 isPending: O,
-                                isAborting: v,
+                                isAborting: j,
                                 run: B,
-                                error: M,
+                                error: F,
                                 progress: p,
                                 RunResultView: D,
                                 viewOptions: null == R ? void 0 : R.view_options,
                                 onViewOptionsChanged: e => {
-                                    T({
+                                    N({
                                         view_options: e
                                     })
                                 },
                                 onCancel: A
-                            }), R && "schema_diff" === R.type && (0, i.jsx)(SchemaDiffView, {
+                            }), R && "schema_diff" === R.type && (0, r.jsx)(SchemaDiffView, {
                                 check: R
-                            }), R && "lineage_diff" === R.type && (0, i.jsx)(LineageDiffView, {
+                            }), R && "lineage_diff" === R.type && (0, r.jsx)(LineageDiffView, {
                                 check: R
                             })]
                         })]
                     })
                 };
 
             function buildMarkdown(e) {
-                return (0, nx.Pn)(CheckDetail_templateObject(), buildTitle(e), buildBody(e))
+                return (0, ny.Pn)(CheckDetail_templateObject(), buildTitle(e), buildBody(e))
             }
 
             function buildBody(e) {
                 return "query" === e.type || "query_diff" === e.type ? "".concat(buildDescription(e), "\n\n").concat(buildQuery(e)) : buildDescription(e)
             }
-            var np = t(79648),
-                ng = t(38505);
+            var nC = t(79648),
+                nb = t(38505);
             let ChecklistItem = e => {
                     let {
                         check: n,
                         selected: t,
-                        onSelect: r
+                        onSelect: i
                     } = e, o = (0, H.NL)(), c = n.check_id, {
                         mutate: d
                     } = (0, eP.D)({
                         mutationFn: e => updateCheck(c, e),
                         onSuccess: () => {
                             o.invalidateQueries({
                                 queryKey: Z.check(c)
                             }), o.invalidateQueries({
                                 queryKey: Z.checks()
                             })
                         }
                     }), u = (e => {
                         switch (e) {
                             case "schema_diff":
-                                return e4.uhn;
+                                return ne.uhn;
                             case "query":
                             case "query_diff":
-                                return e4.r2i;
+                                return ne.r2i;
                             case "value_diff":
-                                return e4.pRi;
+                                return ne.pRi;
                             case "profile_diff":
-                                return e4.KA6;
+                                return ne.KA6;
                             case "row_count_diff":
                                 return B.SwK;
                             case "lineage_diff":
-                                return e4.Ks7;
+                                return ne.Ks7;
                             case "top_k_diff":
-                                return np.Pkc;
+                                return nC.Pkc;
                             case "histogram_diff":
-                                return e4.dku;
+                                return ne.dku;
                             default:
-                                return e4.WzH
+                                return ne.WzH
                         }
                     })(n.type);
-                    return (0, i.jsxs)(a.k, {
+                    return (0, r.jsxs)(a.k, {
                         width: "100%",
                         p: "10px 20px",
                         cursor: "pointer",
                         _hover: {
                             bg: "gray.200"
                         },
                         bg: t ? "gray.100" : "inherit",
-                        onClick: () => r(n.check_id),
+                        onClick: () => i(n.check_id),
                         alignItems: "center",
                         gap: "5px",
-                        children: [(0, i.jsx)(s.J, {
+                        children: [(0, r.jsx)(s.J, {
                             as: u
-                        }), (0, i.jsx)(l.xu, {
+                        }), (0, r.jsx)(l.xu, {
                             flex: "1",
                             textOverflow: "ellipsis",
                             whiteSpace: "nowrap",
                             overflow: "hidden",
                             children: n.name
-                        }), n.is_checked && (0, i.jsx)(s.J, {
+                        }), n.is_checked && (0, r.jsx)(s.J, {
                             color: "green",
                             as: I.FJM
                         })]
                     })
                 },
                 CheckList = e => {
                     let {
                         checks: n,
                         selectedItem: t,
-                        onCheckSelected: r,
+                        onCheckSelected: i,
                         onChecksReordered: l
                     } = e;
-                    return (0, i.jsx)(ng.Z5, {
+                    return (0, r.jsx)(nb.Z5, {
                         onDragEnd: e => {
                             e.destination && l(e.source.index, e.destination.index)
                         },
-                        children: (0, i.jsx)(ng.bK, {
+                        children: (0, r.jsx)(nb.bK, {
                             droppableId: "checklist",
-                            children: e => (0, i.jsxs)(h.g, {
+                            children: e => (0, r.jsxs)(h.g, {
                                 ...e.droppableProps,
                                 ref: e.innerRef,
                                 w: "full",
                                 spacing: "0",
                                 flex: "1",
-                                children: [n.map((e, n) => (0, i.jsx)(ng._l, {
+                                children: [n.map((e, n) => (0, r.jsx)(nb._l, {
                                     draggableId: e.check_id,
                                     index: n,
-                                    children: n => (0, i.jsx)(a.k, {
+                                    children: n => (0, r.jsx)(a.k, {
                                         ref: n.innerRef,
                                         ...n.draggableProps,
                                         ...n.dragHandleProps,
                                         w: "full",
-                                        children: (0, i.jsx)(ChecklistItem, {
+                                        children: (0, r.jsx)(ChecklistItem, {
                                             check: e,
                                             selected: e.check_id === t,
-                                            onSelect: r
+                                            onSelect: i
                                         }, e.check_id)
                                     })
                                 }, e.check_id)), e.placeholder]
                             })
                         })
                     })
                 };
-            var nv = t(73672),
-                nj = t(83561);
+            var nk = t(73672),
+                nw = t(83561);
 
             function CheckListInitLoader() {
                 let e = (0, eb.p)(),
                     n = (0, H.NL)(),
                     t = (0, S.useRef)(null),
-                    [r, l] = (0, S.useState)(null),
+                    [i, l] = (0, S.useState)(null),
                     o = (0, S.useCallback)(async () => {
-                        if (r) try {
+                        if (i) try {
                             let {
                                 checks: t
-                            } = await loadChecks(r);
+                            } = await loadChecks(i);
                             n.invalidateQueries({
                                 queryKey: Z.checks()
                             }), e({
                                 description: "".concat(t, " checks loaded successfully"),
                                 status: "info",
                                 variant: "left-accent",
                                 position: "bottom",
@@ -5328,24 +5444,24 @@
                                 status: "error",
                                 variant: "left-accent",
                                 position: "bottom",
                                 duration: 5e3,
                                 isClosable: !0
                             })
                         }
-                    }, [n, e, r]);
+                    }, [n, e, i]);
                 return (0, S.useEffect)(() => {
-                    r && o()
-                }, [r, o]), (0, i.jsxs)(i.Fragment, {
-                    children: [(0, i.jsx)(m.z, {
+                    i && o()
+                }, [i, o]), (0, r.jsxs)(r.Fragment, {
+                    children: [(0, r.jsx)(m.z, {
                         onClick: () => {
                             t.current && t.current.click()
                         },
                         children: "Load a checklist"
-                    }), (0, i.jsx)("input", {
+                    }), (0, r.jsx)("input", {
                         type: "file",
                         style: {
                             display: "none"
                         },
                         ref: t,
                         onChange: e => {
                             var n;
@@ -5355,22 +5471,22 @@
                 })
             }
 
             function CheckListLoader() {
                 let e = (0, eb.p)(),
                     n = (0, H.NL)(),
                     t = (0, S.useRef)(null),
-                    r = (0, S.useRef)(null),
+                    i = (0, S.useRef)(null),
                     [l, d] = (0, S.useState)(null),
                     {
                         isOpen: u,
                         onOpen: h,
                         onClose: x
                     } = (0, c.q)(),
-                    [, p] = (0, eT.TH)(),
+                    [, p] = (0, eN.TH)(),
                     g = (0, S.useCallback)(async () => {
                         if (l) {
                             try {
                                 let {
                                     checks: t
                                 } = await loadChecks(l);
                                 await n.invalidateQueries({
@@ -5393,286 +5509,286 @@
                                     duration: 5e3,
                                     isClosable: !0
                                 })
                             }
                             x()
                         }
                     }, [n, l, e, x, p]);
-                return (0, i.jsxs)(i.Fragment, {
-                    children: [(0, i.jsx)(o.u, {
+                return (0, r.jsxs)(r.Fragment, {
+                    children: [(0, r.jsx)(o.u, {
                         label: "Load checklist",
-                        children: (0, i.jsx)(P.h, {
+                        children: (0, r.jsx)(P.h, {
                             variant: "unstyled",
                             "aria-label": "Load checks",
                             mr: "10px",
                             onClick: () => {
                                 t.current && t.current.click()
                             },
-                            icon: (0, i.jsx)(s.J, {
+                            icon: (0, r.jsx)(s.J, {
                                 pt: "10px",
-                                as: nj._mA,
+                                as: nw._mA,
                                 boxSize: "2em"
                             })
                         })
-                    }), (0, i.jsx)("input", {
+                    }), (0, r.jsx)("input", {
                         type: "file",
                         style: {
                             display: "none"
                         },
                         ref: t,
                         onChange: e => {
                             var n;
                             (null === (n = e.target.files) || void 0 === n ? void 0 : n.length) === 1 && (d(e.target.files[0]), h())
                         }
-                    }), (0, i.jsx)(nv.a, {
+                    }), (0, r.jsx)(nk.a, {
                         isOpen: u,
-                        leastDestructiveRef: r,
+                        leastDestructiveRef: i,
                         onClose: x,
                         size: "lg",
-                        children: (0, i.jsx)(v.Z, {
-                            children: (0, i.jsxs)(nv._, {
-                                children: [(0, i.jsx)(es.x, {
+                        children: (0, r.jsx)(j.Z, {
+                            children: (0, r.jsxs)(nk._, {
+                                children: [(0, r.jsx)(es.x, {
                                     fontSize: "lg",
                                     fontWeight: "bold",
                                     children: "Load checklist"
-                                }), (0, i.jsx)(C.f, {
-                                    children: (0, i.jsxs)(a.k, {
+                                }), (0, r.jsx)(C.f, {
+                                    children: (0, r.jsxs)(a.k, {
                                         px: "5px",
                                         gap: "5px",
                                         rounded: "md",
                                         direction: "column",
-                                        children: [(0, i.jsxs)(a.k, {
+                                        children: [(0, r.jsxs)(a.k, {
                                             alignItems: "center",
                                             gap: "5px",
-                                            children: [(0, i.jsx)(et.s, {
+                                            children: [(0, r.jsx)(et.s, {
                                                 color: "red.600"
-                                            }), (0, i.jsx)(f.x, {
+                                            }), (0, r.jsx)(f.x, {
                                                 as: "span",
                                                 fontWeight: "500",
                                                 color: "red.600",
                                                 children: "Caution!"
                                             })]
-                                        }), (0, i.jsx)(a.k, {
-                                            children: (0, i.jsxs)(f.x, {
-                                                children: ["The checklist will be", " ", (0, i.jsx)(f.x, {
+                                        }), (0, r.jsx)(a.k, {
+                                            children: (0, r.jsxs)(f.x, {
+                                                children: ["The checklist will be", " ", (0, r.jsx)(f.x, {
                                                     as: "span",
                                                     fontWeight: "600",
                                                     children: "overwritten"
                                                 }), " ", "by the loaded checklist"]
                                             })
                                         })]
                                     })
-                                }), (0, i.jsxs)(eV.m, {
-                                    children: [(0, i.jsx)(m.z, {
-                                        ref: r,
+                                }), (0, r.jsxs)(eV.m, {
+                                    children: [(0, r.jsx)(m.z, {
+                                        ref: i,
                                         onClick: x,
                                         children: "Cancel"
-                                    }), (0, i.jsx)(m.z, {
+                                    }), (0, r.jsx)(m.z, {
                                         colorScheme: "blue",
                                         onClick: g,
                                         ml: "5px",
                                         children: "Load"
                                     })]
                                 })]
                             })
                         })
                     })]
                 })
             }
-            var ny = t(472),
-                nC = t(16062),
-                nb = t(68686),
-                nk = t.n(nb);
+            var nS = t(472),
+                n_ = t(16062),
+                nR = t(68686),
+                nD = t.n(nR);
 
             function CheckListExporter() {
                 let e = (0, eb.p)(),
                     handleExport = async () => {
                         try {
                             let e = await exportChecks(),
                                 n = JSON.stringify(e, null, 2),
                                 t = new Blob([n], {
                                     type: "application/json"
                                 }),
-                                i = new Date,
-                                r = "recce-state-".concat((0, nC.ZP)(i, "yyyy-MM-dd-HH-mm-ss"), ".json");
-                            nk()(t, r)
+                                r = new Date,
+                                i = "recce-state-".concat((0, n_.ZP)(r, "yyyy-MM-dd-HH-mm-ss"), ".json");
+                            nD()(t, i)
                         } catch (n) {
                             console.error("Export failed", n), e({
                                 title: "Export failed",
                                 description: "".concat(n),
                                 status: "error",
                                 variant: "left-accent",
                                 position: "bottom",
                                 duration: 5e3,
                                 isClosable: !0
                             })
                         }
                     };
-                return (0, i.jsx)(o.u, {
+                return (0, r.jsx)(o.u, {
                     label: "Export checklist",
-                    children: (0, i.jsx)(P.h, {
+                    children: (0, r.jsx)(P.h, {
                         variant: "unstyled",
                         "aria-label": "Export checks",
                         onClick: handleExport,
-                        icon: (0, i.jsx)(ny._, {})
+                        icon: (0, r.jsx)(nS._, {})
                     })
                 })
             }
 
             function CheckPage_templateObject() {
-                let e = (0, nn._)(["\n    <details><summary>", "</summary>\n\n    ", "\n\n    </details>"]);
+                let e = (0, no._)(["\n    <details><summary>", "</summary>\n\n    ", "\n\n    </details>"]);
                 return CheckPage_templateObject = function() {
                     return e
                 }, e
             }
             let CheckPage = () => {
                 let {
                     isDemoSite: e
-                } = useLineageGraphsContext(), [, n] = (0, eT.TH)(), [, t] = (0, eT.yj)("/checks/:checkId"), r = (0, H.NL)(), {
+                } = useLineageGraphsContext(), [, n] = (0, eN.TH)(), [, t] = (0, eN.yj)("/checks/:checkId"), i = (0, H.NL)(), {
                     successToast: s,
                     failToast: c
                 } = useClipBoardToast(), d = null == t ? void 0 : t.checkId, {
                     isLoading: f,
                     error: p,
                     data: g,
-                    status: v
+                    status: j
                 } = (0, ee.a)({
                     queryKey: Z.checks(),
                     queryFn: listChecks,
                     refetchOnMount: !0
-                }), j = (0, S.useCallback)(e => {
+                }), y = (0, S.useCallback)(e => {
                     n("/checks/".concat(e))
-                }, [n]), [y, C] = (0, S.useState)(g || []), {
+                }, [n]), [v, C] = (0, S.useState)(g || []), {
                     mutate: b
                 } = (0, eP.D)({
                     mutationFn: e => reorderChecks(e),
                     onSuccess: () => {
-                        r.invalidateQueries({
+                        i.invalidateQueries({
                             queryKey: Z.checks()
                         })
                     }
                 }), k = (0, S.useCallback)((e, n) => {
-                    let t = [...y],
-                        [i] = t.splice(e, 1);
-                    t.splice(n, 0, i), b({
+                    let t = [...v],
+                        [r] = t.splice(e, 1);
+                    t.splice(n, 0, r), b({
                         source: e,
                         destination: n
                     }), C(t)
-                }, [y, C, b]), w = (0, S.useCallback)(async () => {
+                }, [v, C, b]), w = (0, S.useCallback)(async () => {
                     let e = await createSimpleCheck();
-                    r.invalidateQueries({
+                    i.invalidateQueries({
                         queryKey: Z.checks()
-                    }), j(e.check_id)
-                }, [r, j]);
+                    }), y(e.check_id)
+                }, [i, y]);
                 return ((0, S.useEffect)(() => {
-                    "success" === v && (!d && g.length > 0 && n("/checks/".concat(g[0].check_id)), C(g))
-                }, [v, d, g, C, n]), f) ? (0, i.jsx)(i.Fragment, {
+                    "success" === j && (!d && g.length > 0 && n("/checks/".concat(g[0].check_id)), C(g))
+                }, [j, d, g, C, n]), f) ? (0, r.jsx)(r.Fragment, {
                     children: "Loading"
-                }) : p ? (0, i.jsxs)(i.Fragment, {
+                }) : p ? (0, r.jsxs)(r.Fragment, {
                     children: ["Error: ", p.message]
-                }) : (null == g ? void 0 : g.length) ? (0, i.jsxs)(a.k, {
+                }) : (null == g ? void 0 : g.length) ? (0, r.jsxs)(a.k, {
                     height: "100%",
-                    children: [(0, i.jsx)(l.xu, {
+                    children: [(0, r.jsx)(l.xu, {
                         flex: "0 0 400px",
                         borderRight: "lightgray solid 1px",
                         height: "100%",
                         style: {
                             contain: "size"
                         },
-                        children: (0, i.jsxs)(h.g, {
+                        children: (0, r.jsxs)(h.g, {
                             spacing: 0,
                             align: "flex-end",
                             h: "100%",
-                            children: [(0, i.jsxs)(x.U, {
+                            children: [(0, r.jsxs)(x.U, {
                                 gap: "0px",
-                                children: [(0, i.jsx)(o.u, {
+                                children: [(0, r.jsx)(o.u, {
                                     label: "Create a simple check",
-                                    children: (0, i.jsx)(P.h, {
+                                    children: (0, r.jsx)(P.h, {
                                         variant: "unstyled",
                                         "aria-label": "Create a simple check",
                                         onClick: w,
-                                        icon: (0, i.jsx)(eq.d, {})
+                                        icon: (0, r.jsx)(eq.d, {})
                                     })
-                                }), (0, i.jsx)(o.u, {
+                                }), (0, r.jsx)(o.u, {
                                     label: "Copy checklist to the clipboard",
-                                    children: (0, i.jsx)(P.h, {
+                                    children: (0, r.jsx)(P.h, {
                                         variant: "unstyled",
                                         "aria-label": "Copy checklist to the clipboard",
                                         onClick: async () => {
                                             let e = CheckPage_buildMarkdown(g);
                                             if (!navigator.clipboard) {
                                                 c("Failed to copy checklist to clipboard", Error("Copy to clipboard is available only in secure contexts (HTTPS)"));
                                                 return
                                             }
                                             try {
                                                 await navigator.clipboard.writeText(e), s("Copied ".concat(g.length, " checks to the clipboard"))
                                             } catch (e) {
                                                 c("Failed to copy checklist to clipboard", e)
                                             }
                                         },
-                                        icon: (0, i.jsx)(ej.T, {})
+                                        icon: (0, r.jsx)(ey.T, {})
                                     })
-                                }), !e && (0, i.jsxs)(i.Fragment, {
-                                    children: [(0, i.jsx)(CheckListExporter, {}), (0, i.jsx)(CheckListLoader, {})]
+                                }), !e && (0, r.jsxs)(r.Fragment, {
+                                    children: [(0, r.jsx)(CheckListExporter, {}), (0, r.jsx)(CheckListLoader, {})]
                                 })]
-                            }), (0, i.jsx)(eH.i, {
+                            }), (0, r.jsx)(eK.i, {
                                 mb: "8px"
-                            }), (0, i.jsx)(CheckList, {
-                                checks: y,
+                            }), (0, r.jsx)(CheckList, {
+                                checks: v,
                                 selectedItem: d,
-                                onCheckSelected: j,
+                                onCheckSelected: y,
                                 onChecksReordered: k
                             })]
                         })
-                    }), (0, i.jsx)(l.xu, {
+                    }), (0, r.jsx)(l.xu, {
                         flex: "1",
                         height: "100%",
                         width: "calc(100% - 400px)",
-                        children: (0, i.jsx)(eT.rs, {
-                            children: (0, i.jsx)(eT.AW, {
+                        children: (0, r.jsx)(eN.rs, {
+                            children: (0, r.jsx)(eN.AW, {
                                 path: "/checks/:checkId",
-                                children: e => (0, i.jsx)(CheckDetail, {
+                                children: e => (0, r.jsx)(CheckDetail, {
                                     checkId: e.checkId
                                 }, e.checkId)
                             })
                         })
                     })]
-                }) : (0, i.jsx)(u.M, {
+                }) : (0, r.jsx)(u.M, {
                     h: "100%",
-                    children: (0, i.jsxs)(h.g, {
-                        children: [(0, i.jsx)(l.xu, {
+                    children: (0, r.jsxs)(h.g, {
+                        children: [(0, r.jsx)(l.xu, {
                             children: "No checks"
-                        }), (0, i.jsxs)(a.k, {
+                        }), (0, r.jsxs)(a.k, {
                             gap: "5",
-                            children: [(0, i.jsx)(m.z, {
+                            children: [(0, r.jsx)(m.z, {
                                 colorScheme: "blue",
                                 onClick: w,
                                 children: "Create a simple check"
-                            }), !e && (0, i.jsx)(CheckListInitLoader, {})]
+                            }), !e && (0, r.jsx)(CheckListInitLoader, {})]
                         })]
                     })
                 })
             };
 
             function CheckPage_buildMarkdown(e) {
-                let n = e.map(e => (0, nx.Pn)(CheckPage_templateObject(), buildTitle(e), buildDescription(e)));
+                let n = e.map(e => (0, ny.Pn)(CheckPage_templateObject(), buildTitle(e), buildDescription(e)));
                 return n.join("\n\n")
             }
             async function submitQuery(e, n) {
                 return await submitRun("query", e, n)
             }
             async function submitQueryDiff(e, n) {
                 return await submitRun("query_diff", e, n)
             }
             let QueryPage = () => {
                 let {
                     sqlQuery: e,
                     setSqlQuery: n
-                } = useRecceQueryContext(), [t, r] = (0, S.useState)(), [o, s] = (0, S.useState)(), [c, d] = (0, S.useState)({}), u = (0, H.NL)(), [, h] = (0, eT.TH)(), queryFn = async n => {
-                    r(n);
+                } = useRecceQueryContext(), [t, i] = (0, S.useState)(), [o, s] = (0, S.useState)(), [c, d] = (0, S.useState)({}), u = (0, H.NL)(), [, h] = (0, eN.TH)(), queryFn = async n => {
+                    i(n);
                     let {
                         run_id: t
                     } = "query" === n ? await submitQuery({
                         sql_template: e
                     }, {
                         nowait: !0
                     }) : await submitQueryDiff({
@@ -5687,132 +5803,132 @@
                     error: p,
                     isPending: g
                 } = (0, eP.D)({
                     mutationFn: queryFn,
                     onSuccess: e => {
                         d({})
                     }
-                }), v = (0, S.useCallback)(async () => {
+                }), j = (0, S.useCallback)(async () => {
                     if (o) return await cancelRun(o)
-                }, [o]), j = (0, S.useCallback)(async e => {
+                }, [o]), y = (0, S.useCallback)(async e => {
                     if (!(null == e ? void 0 : e.run_id)) return;
                     let n = await checks_createCheckByRun(e.run_id, c);
                     u.invalidateQueries({
                         queryKey: Z.checks()
                     }), h("/checks/".concat(n.check_id))
                 }, [h, c, u]);
-                return !g && (null == x ? void 0 : x.run_id) && (null == x || x.error), (0, i.jsxs)(a.k, {
+                return !g && (null == x ? void 0 : x.run_id) && (null == x || x.error), (0, r.jsxs)(a.k, {
                     direction: "column",
                     height: "100%",
-                    children: [(0, i.jsxs)(a.k, {
+                    children: [(0, r.jsxs)(a.k, {
                         justifyContent: "right",
                         padding: "5px",
                         gap: "5px",
-                        children: [(0, i.jsx)(m.z, {
+                        children: [(0, r.jsx)(m.z, {
                             colorScheme: "blue",
                             onClick: () => f("query_diff"),
                             isDisabled: g,
                             size: "sm",
                             children: "Run Diff"
-                        }), (0, i.jsx)(m.z, {
+                        }), (0, r.jsx)(m.z, {
                             colorScheme: "blue",
                             onClick: () => f("query"),
                             isDisabled: g,
                             size: "sm",
                             children: "Run"
                         })]
-                    }), (0, i.jsx)(l.xu, {
+                    }), (0, r.jsx)(l.xu, {
                         flex: "1",
                         border: "1px solid #CBD5E0",
                         height: "200px",
                         width: "100%",
-                        children: (0, i.jsx)(query_SqlEditor, {
+                        children: (0, r.jsx)(query_SqlEditor, {
                             value: e,
                             onChange: n,
                             onRun: () => f("query"),
                             onRunDiff: () => f("query_diff")
                         })
-                    }), (0, i.jsx)(a.k, {
+                    }), (0, r.jsx)(a.k, {
                         height: "50vh",
                         direction: "column",
-                        children: "query" === t ? (0, i.jsx)(RunView, {
+                        children: "query" === t ? (0, r.jsx)(RunView, {
                             run: x,
                             error: p,
                             isPending: g,
-                            onCancel: v,
-                            children: e => (0, i.jsx)(QueryResultView, {
+                            onCancel: j,
+                            children: e => (0, r.jsx)(QueryResultView, {
                                 ...e,
-                                onAddToChecklist: j
+                                onAddToChecklist: y
                             })
-                        }, o) : (0, i.jsx)(RunView, {
+                        }, o) : (0, r.jsx)(RunView, {
                             isPending: g,
                             run: x,
                             error: p,
                             viewOptions: c,
                             onViewOptionsChanged: d,
-                            onCancel: v,
-                            children: e => (0, i.jsx)(QueryDiffResultView, {
+                            onCancel: j,
+                            children: e => (0, r.jsx)(QueryDiffResultView, {
                                 ...e,
-                                onAddToChecklist: j
+                                onAddToChecklist: y
                             })
                         }, o)
                     })]
                 })
             };
-            var nw = t(72952);
-            let hashNavigate = e => (0, nw.c4)("#!" + e),
+            var nN = t(72952);
+            let hashNavigate = e => (0, nN.c4)("#!" + e),
                 useHashLocation = () => {
-                    let e = (0, nw.LD)(() => window.location.hash.replace(/^#!/, "") || "/", () => "/ssr");
+                    let e = (0, nN.LD)(() => window.location.hash.replace(/^#!/, "") || "/", () => "/ssr");
                     return [e, hashNavigate]
                 };
-            var nS = t(82017),
-                n_ = t(41546);
+            var nT = t(82017),
+                nE = t(41546);
             let RunPage = e => {
                 let {
                     runId: n
                 } = e, {
                     isPending: t,
-                    error: r,
+                    error: i,
                     data: l
                 } = (0, ee.a)({
                     queryKey: Z.run(n),
                     queryFn: async () => waitRun(n)
                 });
-                return (0, i.jsx)(RunView, {
+                return (0, r.jsx)(RunView, {
                     isPending: t,
-                    error: r,
+                    error: i,
                     run: l,
                     RunResultView: ValueDiffResultView
                 })
             };
-            var nR = t(26954);
+            var nL = t(26954);
             let Fallback = e => {
                     let {
                         error: n,
                         resetError: t
                     } = e;
-                    return (0, i.jsx)(u.M, {
+                    return (0, r.jsx)(u.M, {
                         height: "100%",
                         backgroundColor: "gray.50",
-                        children: (0, i.jsxs)(a.k, {
+                        children: (0, r.jsxs)(a.k, {
                             p: 4,
                             direction: "column",
                             justifyContent: "flex-start",
                             backgroundColor: "white",
                             border: "solid lightgray 1px",
                             minHeight: "200px",
-                            children: [(0, i.jsx)(ea.X, {
+                            children: [(0, r.jsx)(ea.X, {
                                 width: "800px",
                                 size: "md",
                                 children: "You have encountered an error"
-                            }), (0, i.jsx)(l.xu, {
+                            }), (0, r.jsx)(l.xu, {
                                 flex: "1",
                                 fontSize: "10pt",
                                 children: n.toString()
-                            }), (0, i.jsx)(m.z, {
+                            }), (0, r.jsx)(m.z, {
                                 justifySelf: "center",
                                 alignSelf: "center",
                                 mt: "20px",
                                 colorScheme: "blue",
                                 size: "sm",
                                 onClick: () => {
                                     t()
@@ -5822,81 +5938,81 @@
                         })
                     })
                 },
                 ErrorBoundary = e => {
                     let {
                         children: n
                     } = e;
-                    return (0, i.jsx)(nR.SV, {
+                    return (0, r.jsx)(nL.SV, {
                         fallback: Fallback,
                         children: n
                     })
                 };
 
             function getCookie(e) {
                 var n = document.cookie.match("(^|;)\\s*" + e + "\\s*=\\s*([^;]+)");
                 return n ? n.pop() : ""
             }
             let RouteAlwaysMount = e => {
                 let {
                     children: n,
                     path: t
-                } = e, [r] = (0, eT.yj)(t);
-                return (0, i.jsx)(l.xu, {
-                    display: r ? "block" : "none",
+                } = e, [i] = (0, eN.yj)(t);
+                return (0, r.jsx)(l.xu, {
+                    display: i ? "block" : "none",
                     height: "100%",
                     children: n
                 })
             };
 
             function TopBar() {
                 let {
                     metadata: e
                 } = useLineageGraphsContext(), n = null == e ? void 0 : e.pr_url;
-                return n && null !== n ? (0, i.jsxs)(a.k, {
+                return n && null !== n ? (0, r.jsxs)(a.k, {
                     gap: "5px",
                     minHeight: "35px",
                     alignItems: "center",
                     justifyContent: "center",
                     bg: "orange.300",
-                    children: [(0, i.jsx)(et.s, {
+                    children: [(0, r.jsx)(et.s, {
                         color: "orange.600"
-                    }), (0, i.jsxs)(f.x, {
-                        children: ["Please check", " ", (0, i.jsx)(eK.r, {
+                    }), (0, r.jsxs)(f.x, {
+                        children: ["Please check", " ", (0, r.jsx)(eH.r, {
                             textDecoration: "underline",
                             fontWeight: "600",
                             href: n,
                             isExternal: !0,
                             children: "this Pull Request"
                         }), " ", "comment for context about this Recce instance"]
                     })]
-                }) : (0, i.jsx)(i.Fragment, {})
+                }) : (0, r.jsx)(r.Fragment, {})
             }
 
             function NavBar() {
-                let [e, n] = (0, eT.TH)(), t = useVersionNumber(), r = [
+                let [e, n] = (0, eN.TH)(), t = useVersionNumber(), i = [
                     ["Lineage", "/lineage"],
                     ["Query", "/query"],
                     ["Checklist", "/checks"]
-                ], o = eA().findIndex(r, n => {
+                ], o = eA().findIndex(i, n => {
                     let [, t] = n;
                     return e.startsWith(t)
                 });
-                return (0, i.jsx)(ed.m, {
+                return (0, r.jsx)(ed.m, {
                     index: o,
-                    children: (0, i.jsxs)(eu.t, {
-                        children: [r.map(e => {
-                            let [t, r] = e;
-                            return (0, i.jsx)(eh.O, {
+                    children: (0, r.jsxs)(eu.t, {
+                        children: [i.map(e => {
+                            let [t, i] = e;
+                            return (0, r.jsx)(eh.O, {
                                 onClick: () => {
-                                    n(r)
+                                    n(i)
                                 },
                                 children: t
                             }, t)
-                        }), (0, i.jsx)(l.xu, {
+                        }), (0, r.jsx)(l.xu, {
                             position: "absolute",
                             right: "0",
                             top: "0",
                             p: "2",
                             color: "gray.500",
                             children: t
                         })]
@@ -5904,78 +6020,78 @@
                 })
             }
 
             function Home() {
                 (0, S.useLayoutEffect)(() => {
                     let e = getCookie("recce_user_id");
                     if (e) try {
-                        ne.S1("b1ea2155354b7e1e41981715f16599f2", e, {
+                        nl.S1("b1ea2155354b7e1e41981715f16599f2", e, {
                             defaultTracking: !0
                         })
                     } catch (e) {
                         console.error(e)
                     }
                 }, []);
-                let e = (0, nS.Z)({
+                let e = (0, nT.Z)({
                     components: {
                         MuiTooltip: {
                             styleOverrides: {
                                 tooltip: {
                                     zIndex: 1500
                                 }
                             }
                         }
                     }
                 });
-                return (0, i.jsx)(n_.Z, {
+                return (0, r.jsx)(nE.Z, {
                     theme: e,
-                    children: (0, i.jsx)(e7.x, {
-                        children: (0, i.jsx)(H.aH, {
+                    children: (0, r.jsx)(ni.x, {
+                        children: (0, r.jsx)(H.aH, {
                             client: J,
-                            children: (0, i.jsx)(eT.F0, {
+                            children: (0, r.jsx)(eN.F0, {
                                 hook: useHashLocation,
-                                children: (0, i.jsx)(RecceContextProvider, {
-                                    children: (0, i.jsxs)(a.k, {
+                                children: (0, r.jsx)(RecceContextProvider, {
+                                    children: (0, r.jsxs)(a.k, {
                                         direction: "column",
                                         height: "100vh",
-                                        children: [(0, i.jsx)(TopBar, {}), (0, i.jsx)(NavBar, {}), (0, i.jsx)(ErrorBoundary, {
-                                            children: (0, i.jsxs)(l.xu, {
+                                        children: [(0, r.jsx)(TopBar, {}), (0, r.jsx)(NavBar, {}), (0, r.jsx)(ErrorBoundary, {
+                                            children: (0, r.jsxs)(l.xu, {
                                                 p: 0,
                                                 overflow: "auto",
                                                 flex: "1",
                                                 style: {
                                                     contain: "size"
                                                 },
-                                                children: [(0, i.jsx)(RouteAlwaysMount, {
+                                                children: [(0, r.jsx)(RouteAlwaysMount, {
                                                     path: "/lineage",
-                                                    children: (0, i.jsx)(LineageView, {})
-                                                }), (0, i.jsxs)(eT.rs, {
-                                                    children: [(0, i.jsx)(eT.AW, {
+                                                    children: (0, r.jsx)(LineageView, {})
+                                                }), (0, r.jsxs)(eN.rs, {
+                                                    children: [(0, r.jsx)(eN.AW, {
                                                         path: "/query",
-                                                        children: (0, i.jsx)(QueryPage, {})
-                                                    }), (0, i.jsx)(eT.AW, {
+                                                        children: (0, r.jsx)(QueryPage, {})
+                                                    }), (0, r.jsx)(eN.AW, {
                                                         path: "/checks/:slug*",
-                                                        children: (0, i.jsx)(CheckPage, {})
-                                                    }), (0, i.jsx)(eT.AW, {
+                                                        children: (0, r.jsx)(CheckPage, {})
+                                                    }), (0, r.jsx)(eN.AW, {
                                                         path: "/runs/:runId",
                                                         children: e => {
                                                             let {
                                                                 runId: n
                                                             } = e;
-                                                            return (0, i.jsx)(RunPage, {
+                                                            return (0, r.jsx)(RunPage, {
                                                                 runId: n
                                                             })
                                                         }
-                                                    }), (0, i.jsx)(eT.AW, {
+                                                    }), (0, r.jsx)(eN.AW, {
                                                         path: "/ssr",
-                                                        children: (0, i.jsx)(i.Fragment, {
+                                                        children: (0, r.jsx)(r.Fragment, {
                                                             children: "Loading"
                                                         })
-                                                    }), (0, i.jsx)(eT.AW, {
-                                                        children: (0, i.jsx)(eT.l_, {
+                                                    }), (0, r.jsx)(eN.AW, {
+                                                        children: (0, r.jsx)(eN.l_, {
                                                             to: "/lineage"
                                                         })
                                                     })]
                                                 })]
                                             })
                                         })]
                                     })
```

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/c132bf7d-fca1bc3c8aa231eb.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/c132bf7d-fca1bc3c8aa231eb.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/f0cfc0e7-bb82a3d2a10fc463.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/f0cfc0e7-bb82a3d2a10fc463.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/f6be744d-5973a409ea097354.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/f6be744d-5973a409ea097354.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/f78b7092-bf8a8853eef36a4c.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/f78b7092-bf8a8853eef36a4c.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/fb2d5402-0ccc92fc728c2993.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/fb2d5402-0ccc92fc728c2993.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/framework-f780fd9bae3b8c58.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/framework-f780fd9bae3b8c58.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/main-01494d5774218692.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/main-01494d5774218692.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/main-app-3297e27de57b3a96.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/main-app-3297e27de57b3a96.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/chunks/webpack-2d4823656eaa7d1c.js` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/chunks/webpack-2d4823656eaa7d1c.js`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/_next/static/css/6d0611c21a82d0bb.css` & `recce-nightly-0.9.0.20240313/recce/data/_next/static/css/6d0611c21a82d0bb.css`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/favicon.ico` & `recce-nightly-0.9.0.20240313/recce/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/data/index.html` & `recce-nightly-0.9.0.20240313/recce/data/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width, initial-scale=1"/><link rel="stylesheet" href="/_next/static/css/6d0611c21a82d0bb.css" crossorigin="" data-precedence="next"/><link rel="preload" as="script" fetchPriority="low" href="/_next/static/chunks/webpack-2d4823656eaa7d1c.js" crossorigin=""/><script src="/_next/static/chunks/f0cfc0e7-bb82a3d2a10fc463.js" async="" crossorigin=""></script><script src="/_next/static/chunks/62-fe89bcbd7de7edb6.js" async="" crossorigin=""></script><script src="/_next/static/chunks/main-app-3297e27de57b3a96.js" async="" crossorigin=""></script><script src="/_next/static/chunks/7c9ab469-732af37965d79ccf.js" async=""></script><script src="/_next/static/chunks/fb2d5402-0ccc92fc728c2993.js" async=""></script><script src="/_next/static/chunks/526a6206-7ccbd30e159c1652.js" async=""></script><script src="/_next/static/chunks/607285b2-dadd48144d45dbcf.js" async=""></script><script src="/_next/static/chunks/f6be744d-5973a409ea097354.js" async=""></script><script src="/_next/static/chunks/f78b7092-bf8a8853eef36a4c.js" async=""></script><script src="/_next/static/chunks/6af6e714-6003aba9c53d2dcd.js" async=""></script><script src="/_next/static/chunks/030e0bea-59754f62ad2a287c.js" async=""></script><script src="/_next/static/chunks/5e9a126f-da62af62011c0643.js" async=""></script><script src="/_next/static/chunks/2d02f0f7-ed3b4e4daa7c5d22.js" async=""></script><script src="/_next/static/chunks/49348413-7aacf235ca16afb9.js" async=""></script><script src="/_next/static/chunks/6dc81886-a3fa8efdc3652e8f.js" async=""></script><script src="/_next/static/chunks/c132bf7d-fca1bc3c8aa231eb.js" async=""></script><script src="/_next/static/chunks/4b89641d-a80e6024cd2468dc.js" async=""></script><script src="/_next/static/chunks/354-d94f5f7615bdde2d.js" async=""></script><script src="/_next/static/chunks/app/page-11d757976ef71345.js" async=""></script><title>recce</title><meta name="description" content="Recce: a dbt tool"/><link rel="icon" href="/favicon.ico" type="image/x-icon" sizes="16x16"/><script src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js" crossorigin="" noModule=""></script></head><body><style data-emotion="css-global 1b7scut">:host,:root,[data-theme]{--chakra-ring-inset:var(--chakra-empty,/*!*/ /*!*/);--chakra-ring-offset-width:0px;--chakra-ring-offset-color:#fff;--chakra-ring-color:rgba(66, 153, 225, 0.6);--chakra-ring-offset-shadow:0 0 #0000;--chakra-ring-shadow:0 0 #0000;--chakra-space-x-reverse:0;--chakra-space-y-reverse:0;--chakra-colors-transparent:transparent;--chakra-colors-current:currentColor;--chakra-colors-black:#000000;--chakra-colors-white:#FFFFFF;--chakra-colors-whiteAlpha-50:rgba(255, 255, 255, 0.04);--chakra-colors-whiteAlpha-100:rgba(255, 255, 255, 0.06);--chakra-colors-whiteAlpha-200:rgba(255, 255, 255, 0.08);--chakra-colors-whiteAlpha-300:rgba(255, 255, 255, 0.16);--chakra-colors-whiteAlpha-400:rgba(255, 255, 255, 0.24);--chakra-colors-whiteAlpha-500:rgba(255, 255, 255, 0.36);--chakra-colors-whiteAlpha-600:rgba(255, 255, 255, 0.48);--chakra-colors-whiteAlpha-700:rgba(255, 255, 255, 0.64);--chakra-colors-whiteAlpha-800:rgba(255, 255, 255, 0.80);--chakra-colors-whiteAlpha-900:rgba(255, 255, 255, 0.92);--chakra-colors-blackAlpha-50:rgba(0, 0, 0, 0.04);--chakra-colors-blackAlpha-100:rgba(0, 0, 0, 0.06);--chakra-colors-blackAlpha-200:rgba(0, 0, 0, 0.08);--chakra-colors-blackAlpha-300:rgba(0, 0, 0, 0.16);--chakra-colors-blackAlpha-400:rgba(0, 0, 0, 0.24);--chakra-colors-blackAlpha-500:rgba(0, 0, 0, 0.36);--chakra-colors-blackAlpha-600:rgba(0, 0, 0, 0.48);--chakra-colors-blackAlpha-700:rgba(0, 0, 0, 0.64);--chakra-colors-blackAlpha-800:rgba(0, 0, 0, 0.80);--chakra-colors-blackAlpha-900:rgba(0, 0, 0, 0.92);--chakra-colors-gray-50:#F7FAFC;--chakra-colors-gray-100:#EDF2F7;--chakra-colors-gray-200:#E2E8F0;--chakra-colors-gray-300:#CBD5E0;--chakra-colors-gray-400:#A0AEC0;--chakra-colors-gray-500:#718096;--chakra-colors-gray-600:#4A5568;--chakra-colors-gray-700:#2D3748;--chakra-colors-gray-800:#1A202C;--chakra-colors-gray-900:#171923;--chakra-colors-red-50:#FFF5F5;--chakra-colors-red-100:#FED7D7;--chakra-colors-red-200:#FEB2B2;--chakra-colors-red-300:#FC8181;--chakra-colors-red-400:#F56565;--chakra-colors-red-500:#E53E3E;--chakra-colors-red-600:#C53030;--chakra-colors-red-700:#9B2C2C;--chakra-colors-red-800:#822727;--chakra-colors-red-900:#63171B;--chakra-colors-orange-50:#FFFAF0;--chakra-colors-orange-100:#FEEBC8;--chakra-colors-orange-200:#FBD38D;--chakra-colors-orange-300:#F6AD55;--chakra-colors-orange-400:#ED8936;--chakra-colors-orange-500:#DD6B20;--chakra-colors-orange-600:#C05621;--chakra-colors-orange-700:#9C4221;--chakra-colors-orange-800:#7B341E;--chakra-colors-orange-900:#652B19;--chakra-colors-yellow-50:#FFFFF0;--chakra-colors-yellow-100:#FEFCBF;--chakra-colors-yellow-200:#FAF089;--chakra-colors-yellow-300:#F6E05E;--chakra-colors-yellow-400:#ECC94B;--chakra-colors-yellow-500:#D69E2E;--chakra-colors-yellow-600:#B7791F;--chakra-colors-yellow-700:#975A16;--chakra-colors-yellow-800:#744210;--chakra-colors-yellow-900:#5F370E;--chakra-colors-green-50:#F0FFF4;--chakra-colors-green-100:#C6F6D5;--chakra-colors-green-200:#9AE6B4;--chakra-colors-green-300:#68D391;--chakra-colors-green-400:#48BB78;--chakra-colors-green-500:#38A169;--chakra-colors-green-600:#2F855A;--chakra-colors-green-700:#276749;--chakra-colors-green-800:#22543D;--chakra-colors-green-900:#1C4532;--chakra-colors-teal-50:#E6FFFA;--chakra-colors-teal-100:#B2F5EA;--chakra-colors-teal-200:#81E6D9;--chakra-colors-teal-300:#4FD1C5;--chakra-colors-teal-400:#38B2AC;--chakra-colors-teal-500:#319795;--chakra-colors-teal-600:#2C7A7B;--chakra-colors-teal-700:#285E61;--chakra-colors-teal-800:#234E52;--chakra-colors-teal-900:#1D4044;--chakra-colors-blue-50:#ebf8ff;--chakra-colors-blue-100:#bee3f8;--chakra-colors-blue-200:#90cdf4;--chakra-colors-blue-300:#63b3ed;--chakra-colors-blue-400:#4299e1;--chakra-colors-blue-500:#3182ce;--chakra-colors-blue-600:#2b6cb0;--chakra-colors-blue-700:#2c5282;--chakra-colors-blue-800:#2a4365;--chakra-colors-blue-900:#1A365D;--chakra-colors-cyan-50:#EDFDFD;--chakra-colors-cyan-100:#C4F1F9;--chakra-colors-cyan-200:#9DECF9;--chakra-colors-cyan-300:#76E4F7;--chakra-colors-cyan-400:#0BC5EA;--chakra-colors-cyan-500:#00B5D8;--chakra-colors-cyan-600:#00A3C4;--chakra-colors-cyan-700:#0987A0;--chakra-colors-cyan-800:#086F83;--chakra-colors-cyan-900:#065666;--chakra-colors-purple-50:#FAF5FF;--chakra-colors-purple-100:#E9D8FD;--chakra-colors-purple-200:#D6BCFA;--chakra-colors-purple-300:#B794F4;--chakra-colors-purple-400:#9F7AEA;--chakra-colors-purple-500:#805AD5;--chakra-colors-purple-600:#6B46C1;--chakra-colors-purple-700:#553C9A;--chakra-colors-purple-800:#44337A;--chakra-colors-purple-900:#322659;--chakra-colors-pink-50:#FFF5F7;--chakra-colors-pink-100:#FED7E2;--chakra-colors-pink-200:#FBB6CE;--chakra-colors-pink-300:#F687B3;--chakra-colors-pink-400:#ED64A6;--chakra-colors-pink-500:#D53F8C;--chakra-colors-pink-600:#B83280;--chakra-colors-pink-700:#97266D;--chakra-colors-pink-800:#702459;--chakra-colors-pink-900:#521B41;--chakra-colors-linkedin-50:#E8F4F9;--chakra-colors-linkedin-100:#CFEDFB;--chakra-colors-linkedin-200:#9BDAF3;--chakra-colors-linkedin-300:#68C7EC;--chakra-colors-linkedin-400:#34B3E4;--chakra-colors-linkedin-500:#00A0DC;--chakra-colors-linkedin-600:#008CC9;--chakra-colors-linkedin-700:#0077B5;--chakra-colors-linkedin-800:#005E93;--chakra-colors-linkedin-900:#004471;--chakra-colors-facebook-50:#E8F4F9;--chakra-colors-facebook-100:#D9DEE9;--chakra-colors-facebook-200:#B7C2DA;--chakra-colors-facebook-300:#6482C0;--chakra-colors-facebook-400:#4267B2;--chakra-colors-facebook-500:#385898;--chakra-colors-facebook-600:#314E89;--chakra-colors-facebook-700:#29487D;--chakra-colors-facebook-800:#223B67;--chakra-colors-facebook-900:#1E355B;--chakra-colors-messenger-50:#D0E6FF;--chakra-colors-messenger-100:#B9DAFF;--chakra-colors-messenger-200:#A2CDFF;--chakra-colors-messenger-300:#7AB8FF;--chakra-colors-messenger-400:#2E90FF;--chakra-colors-messenger-500:#0078FF;--chakra-colors-messenger-600:#0063D1;--chakra-colors-messenger-700:#0052AC;--chakra-colors-messenger-800:#003C7E;--chakra-colors-messenger-900:#002C5C;--chakra-colors-whatsapp-50:#dffeec;--chakra-colors-whatsapp-100:#b9f5d0;--chakra-colors-whatsapp-200:#90edb3;--chakra-colors-whatsapp-300:#65e495;--chakra-colors-whatsapp-400:#3cdd78;--chakra-colors-whatsapp-500:#22c35e;--chakra-colors-whatsapp-600:#179848;--chakra-colors-whatsapp-700:#0c6c33;--chakra-colors-whatsapp-800:#01421c;--chakra-colors-whatsapp-900:#001803;--chakra-colors-twitter-50:#E5F4FD;--chakra-colors-twitter-100:#C8E9FB;--chakra-colors-twitter-200:#A8DCFA;--chakra-colors-twitter-300:#83CDF7;--chakra-colors-twitter-400:#57BBF5;--chakra-colors-twitter-500:#1DA1F2;--chakra-colors-twitter-600:#1A94DA;--chakra-colors-twitter-700:#1681BF;--chakra-colors-twitter-800:#136B9E;--chakra-colors-twitter-900:#0D4D71;--chakra-colors-telegram-50:#E3F2F9;--chakra-colors-telegram-100:#C5E4F3;--chakra-colors-telegram-200:#A2D4EC;--chakra-colors-telegram-300:#7AC1E4;--chakra-colors-telegram-400:#47A9DA;--chakra-colors-telegram-500:#0088CC;--chakra-colors-telegram-600:#007AB8;--chakra-colors-telegram-700:#006BA1;--chakra-colors-telegram-800:#005885;--chakra-colors-telegram-900:#003F5E;--chakra-borders-none:0;--chakra-borders-1px:1px solid;--chakra-borders-2px:2px solid;--chakra-borders-4px:4px solid;--chakra-borders-8px:8px solid;--chakra-fonts-heading:-apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol";--chakra-fonts-body:-apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol";--chakra-fonts-mono:SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;--chakra-fontSizes-3xs:0.45rem;--chakra-fontSizes-2xs:0.625rem;--chakra-fontSizes-xs:0.75rem;--chakra-fontSizes-sm:0.875rem;--chakra-fontSizes-md:1rem;--chakra-fontSizes-lg:1.125rem;--chakra-fontSizes-xl:1.25rem;--chakra-fontSizes-2xl:1.5rem;--chakra-fontSizes-3xl:1.875rem;--chakra-fontSizes-4xl:2.25rem;--chakra-fontSizes-5xl:3rem;--chakra-fontSizes-6xl:3.75rem;--chakra-fontSizes-7xl:4.5rem;--chakra-fontSizes-8xl:6rem;--chakra-fontSizes-9xl:8rem;--chakra-fontWeights-hairline:100;--chakra-fontWeights-thin:200;--chakra-fontWeights-light:300;--chakra-fontWeights-normal:400;--chakra-fontWeights-medium:500;--chakra-fontWeights-semibold:600;--chakra-fontWeights-bold:700;--chakra-fontWeights-extrabold:800;--chakra-fontWeights-black:900;--chakra-letterSpacings-tighter:-0.05em;--chakra-letterSpacings-tight:-0.025em;--chakra-letterSpacings-normal:0;--chakra-letterSpacings-wide:0.025em;--chakra-letterSpacings-wider:0.05em;--chakra-letterSpacings-widest:0.1em;--chakra-lineHeights-3:.75rem;--chakra-lineHeights-4:1rem;--chakra-lineHeights-5:1.25rem;--chakra-lineHeights-6:1.5rem;--chakra-lineHeights-7:1.75rem;--chakra-lineHeights-8:2rem;--chakra-lineHeights-9:2.25rem;--chakra-lineHeights-10:2.5rem;--chakra-lineHeights-normal:normal;--chakra-lineHeights-none:1;--chakra-lineHeights-shorter:1.25;--chakra-lineHeights-short:1.375;--chakra-lineHeights-base:1.5;--chakra-lineHeights-tall:1.625;--chakra-lineHeights-taller:2;--chakra-radii-none:0;--chakra-radii-sm:0.125rem;--chakra-radii-base:0.25rem;--chakra-radii-md:0.375rem;--chakra-radii-lg:0.5rem;--chakra-radii-xl:0.75rem;--chakra-radii-2xl:1rem;--chakra-radii-3xl:1.5rem;--chakra-radii-full:9999px;--chakra-space-1:0.25rem;--chakra-space-2:0.5rem;--chakra-space-3:0.75rem;--chakra-space-4:1rem;--chakra-space-5:1.25rem;--chakra-space-6:1.5rem;--chakra-space-7:1.75rem;--chakra-space-8:2rem;--chakra-space-9:2.25rem;--chakra-space-10:2.5rem;--chakra-space-12:3rem;--chakra-space-14:3.5rem;--chakra-space-16:4rem;--chakra-space-20:5rem;--chakra-space-24:6rem;--chakra-space-28:7rem;--chakra-space-32:8rem;--chakra-space-36:9rem;--chakra-space-40:10rem;--chakra-space-44:11rem;--chakra-space-48:12rem;--chakra-space-52:13rem;--chakra-space-56:14rem;--chakra-space-60:15rem;--chakra-space-64:16rem;--chakra-space-72:18rem;--chakra-space-80:20rem;--chakra-space-96:24rem;--chakra-space-px:1px;--chakra-space-0-5:0.125rem;--chakra-space-1-5:0.375rem;--chakra-space-2-5:0.625rem;--chakra-space-3-5:0.875rem;--chakra-shadows-xs:0 0 0 1px rgba(0, 0, 0, 0.05);--chakra-shadows-sm:0 1px 2px 0 rgba(0, 0, 0, 0.05);--chakra-shadows-base:0 1px 3px 0 rgba(0, 0, 0, 0.1),0 1px 2px 0 rgba(0, 0, 0, 0.06);--chakra-shadows-md:0 4px 6px -1px rgba(0, 0, 0, 0.1),0 2px 4px -1px rgba(0, 0, 0, 0.06);--chakra-shadows-lg:0 10px 15px -3px rgba(0, 0, 0, 0.1),0 4px 6px -2px rgba(0, 0, 0, 0.05);--chakra-shadows-xl:0 20px 25px -5px rgba(0, 0, 0, 0.1),0 10px 10px -5px rgba(0, 0, 0, 0.04);--chakra-shadows-2xl:0 25px 50px -12px rgba(0, 0, 0, 0.25);--chakra-shadows-outline:0 0 0 3px rgba(66, 153, 225, 0.6);--chakra-shadows-inner:inset 0 2px 4px 0 rgba(0,0,0,0.06);--chakra-shadows-none:none;--chakra-shadows-dark-lg:rgba(0, 0, 0, 0.1) 0px 0px 0px 1px,rgba(0, 0, 0, 0.2) 0px 5px 10px,rgba(0, 0, 0, 0.4) 0px 15px 40px;--chakra-sizes-1:0.25rem;--chakra-sizes-2:0.5rem;--chakra-sizes-3:0.75rem;--chakra-sizes-4:1rem;--chakra-sizes-5:1.25rem;--chakra-sizes-6:1.5rem;--chakra-sizes-7:1.75rem;--chakra-sizes-8:2rem;--chakra-sizes-9:2.25rem;--chakra-sizes-10:2.5rem;--chakra-sizes-12:3rem;--chakra-sizes-14:3.5rem;--chakra-sizes-16:4rem;--chakra-sizes-20:5rem;--chakra-sizes-24:6rem;--chakra-sizes-28:7rem;--chakra-sizes-32:8rem;--chakra-sizes-36:9rem;--chakra-sizes-40:10rem;--chakra-sizes-44:11rem;--chakra-sizes-48:12rem;--chakra-sizes-52:13rem;--chakra-sizes-56:14rem;--chakra-sizes-60:15rem;--chakra-sizes-64:16rem;--chakra-sizes-72:18rem;--chakra-sizes-80:20rem;--chakra-sizes-96:24rem;--chakra-sizes-px:1px;--chakra-sizes-0-5:0.125rem;--chakra-sizes-1-5:0.375rem;--chakra-sizes-2-5:0.625rem;--chakra-sizes-3-5:0.875rem;--chakra-sizes-max:max-content;--chakra-sizes-min:min-content;--chakra-sizes-full:100%;--chakra-sizes-3xs:14rem;--chakra-sizes-2xs:16rem;--chakra-sizes-xs:20rem;--chakra-sizes-sm:24rem;--chakra-sizes-md:28rem;--chakra-sizes-lg:32rem;--chakra-sizes-xl:36rem;--chakra-sizes-2xl:42rem;--chakra-sizes-3xl:48rem;--chakra-sizes-4xl:56rem;--chakra-sizes-5xl:64rem;--chakra-sizes-6xl:72rem;--chakra-sizes-7xl:80rem;--chakra-sizes-8xl:90rem;--chakra-sizes-prose:60ch;--chakra-sizes-container-sm:640px;--chakra-sizes-container-md:768px;--chakra-sizes-container-lg:1024px;--chakra-sizes-container-xl:1280px;--chakra-zIndices-hide:-1;--chakra-zIndices-auto:auto;--chakra-zIndices-base:0;--chakra-zIndices-docked:10;--chakra-zIndices-dropdown:1000;--chakra-zIndices-sticky:1100;--chakra-zIndices-banner:1200;--chakra-zIndices-overlay:1300;--chakra-zIndices-modal:1400;--chakra-zIndices-popover:1500;--chakra-zIndices-skipLink:1600;--chakra-zIndices-toast:1700;--chakra-zIndices-tooltip:1800;--chakra-transition-property-common:background-color,border-color,color,fill,stroke,opacity,box-shadow,transform;--chakra-transition-property-colors:background-color,border-color,color,fill,stroke;--chakra-transition-property-dimensions:width,height;--chakra-transition-property-position:left,right,top,bottom;--chakra-transition-property-background:background-color,background-image,background-position;--chakra-transition-easing-ease-in:cubic-bezier(0.4, 0, 1, 1);--chakra-transition-easing-ease-out:cubic-bezier(0, 0, 0.2, 1);--chakra-transition-easing-ease-in-out:cubic-bezier(0.4, 0, 0.2, 1);--chakra-transition-duration-ultra-fast:50ms;--chakra-transition-duration-faster:100ms;--chakra-transition-duration-fast:150ms;--chakra-transition-duration-normal:200ms;--chakra-transition-duration-slow:300ms;--chakra-transition-duration-slower:400ms;--chakra-transition-duration-ultra-slow:500ms;--chakra-blur-none:0;--chakra-blur-sm:4px;--chakra-blur-base:8px;--chakra-blur-md:12px;--chakra-blur-lg:16px;--chakra-blur-xl:24px;--chakra-blur-2xl:40px;--chakra-blur-3xl:64px;--chakra-breakpoints-base:0em;--chakra-breakpoints-sm:30em;--chakra-breakpoints-md:48em;--chakra-breakpoints-lg:62em;--chakra-breakpoints-xl:80em;--chakra-breakpoints-2xl:96em;}.chakra-ui-light :host:not([data-theme]),.chakra-ui-light :root:not([data-theme]),.chakra-ui-light [data-theme]:not([data-theme]),[data-theme=light] :host:not([data-theme]),[data-theme=light] :root:not([data-theme]),[data-theme=light] [data-theme]:not([data-theme]),:host[data-theme=light],:root[data-theme=light],[data-theme][data-theme=light]{--chakra-colors-chakra-body-text:var(--chakra-colors-gray-800);--chakra-colors-chakra-body-bg:var(--chakra-colors-white);--chakra-colors-chakra-border-color:var(--chakra-colors-gray-200);--chakra-colors-chakra-inverse-text:var(--chakra-colors-white);--chakra-colors-chakra-subtle-bg:var(--chakra-colors-gray-100);--chakra-colors-chakra-subtle-text:var(--chakra-colors-gray-600);--chakra-colors-chakra-placeholder-color:var(--chakra-colors-gray-500);}.chakra-ui-dark :host:not([data-theme]),.chakra-ui-dark :root:not([data-theme]),.chakra-ui-dark [data-theme]:not([data-theme]),[data-theme=dark] :host:not([data-theme]),[data-theme=dark] :root:not([data-theme]),[data-theme=dark] [data-theme]:not([data-theme]),:host[data-theme=dark],:root[data-theme=dark],[data-theme][data-theme=dark]{--chakra-colors-chakra-body-text:var(--chakra-colors-whiteAlpha-900);--chakra-colors-chakra-body-bg:var(--chakra-colors-gray-800);--chakra-colors-chakra-border-color:var(--chakra-colors-whiteAlpha-300);--chakra-colors-chakra-inverse-text:var(--chakra-colors-gray-800);--chakra-colors-chakra-subtle-bg:var(--chakra-colors-gray-700);--chakra-colors-chakra-subtle-text:var(--chakra-colors-gray-400);--chakra-colors-chakra-placeholder-color:var(--chakra-colors-whiteAlpha-400);}</style><style data-emotion="css-global fubdgu">html{line-height:1.5;-webkit-text-size-adjust:100%;font-family:system-ui,sans-serif;-webkit-font-smoothing:antialiased;text-rendering:optimizeLegibility;-moz-osx-font-smoothing:grayscale;touch-action:manipulation;}body{position:relative;min-height:100%;margin:0;font-feature-settings:"kern";}:where(*, *::before, *::after){border-width:0;border-style:solid;box-sizing:border-box;word-wrap:break-word;}main{display:block;}hr{border-top-width:1px;box-sizing:content-box;height:0;overflow:visible;}:where(pre, code, kbd,samp){font-family:SFMono-Regular,Menlo,Monaco,Consolas,monospace;font-size:1em;}a{background-color:transparent;color:inherit;-webkit-text-decoration:inherit;text-decoration:inherit;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;-webkit-text-decoration:underline dotted;-webkit-text-decoration:underline dotted;text-decoration:underline dotted;}:where(b, strong){font-weight:bold;}small{font-size:80%;}:where(sub,sup){font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sub{bottom:-0.25em;}sup{top:-0.5em;}img{border-style:none;}:where(button, input, optgroup, select, textarea){font-family:inherit;font-size:100%;line-height:1.15;margin:0;}:where(button, input){overflow:visible;}:where(button, select){text-transform:none;}:where(
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width, initial-scale=1"/><link rel="stylesheet" href="/_next/static/css/6d0611c21a82d0bb.css" crossorigin="" data-precedence="next"/><link rel="preload" as="script" fetchPriority="low" href="/_next/static/chunks/webpack-2d4823656eaa7d1c.js" crossorigin=""/><script src="/_next/static/chunks/f0cfc0e7-bb82a3d2a10fc463.js" async="" crossorigin=""></script><script src="/_next/static/chunks/62-fe89bcbd7de7edb6.js" async="" crossorigin=""></script><script src="/_next/static/chunks/main-app-3297e27de57b3a96.js" async="" crossorigin=""></script><script src="/_next/static/chunks/7c9ab469-732af37965d79ccf.js" async=""></script><script src="/_next/static/chunks/fb2d5402-0ccc92fc728c2993.js" async=""></script><script src="/_next/static/chunks/526a6206-7ccbd30e159c1652.js" async=""></script><script src="/_next/static/chunks/607285b2-dadd48144d45dbcf.js" async=""></script><script src="/_next/static/chunks/f6be744d-5973a409ea097354.js" async=""></script><script src="/_next/static/chunks/f78b7092-bf8a8853eef36a4c.js" async=""></script><script src="/_next/static/chunks/6af6e714-6003aba9c53d2dcd.js" async=""></script><script src="/_next/static/chunks/030e0bea-59754f62ad2a287c.js" async=""></script><script src="/_next/static/chunks/5e9a126f-da62af62011c0643.js" async=""></script><script src="/_next/static/chunks/2d02f0f7-ed3b4e4daa7c5d22.js" async=""></script><script src="/_next/static/chunks/49348413-7aacf235ca16afb9.js" async=""></script><script src="/_next/static/chunks/6dc81886-a3fa8efdc3652e8f.js" async=""></script><script src="/_next/static/chunks/c132bf7d-fca1bc3c8aa231eb.js" async=""></script><script src="/_next/static/chunks/4b89641d-a80e6024cd2468dc.js" async=""></script><script src="/_next/static/chunks/354-d94f5f7615bdde2d.js" async=""></script><script src="/_next/static/chunks/app/page-2e986eecfb9156dd.js" async=""></script><title>recce</title><meta name="description" content="Recce: a dbt tool"/><link rel="icon" href="/favicon.ico" type="image/x-icon" sizes="16x16"/><script src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js" crossorigin="" noModule=""></script></head><body><style data-emotion="css-global 1b7scut">:host,:root,[data-theme]{--chakra-ring-inset:var(--chakra-empty,/*!*/ /*!*/);--chakra-ring-offset-width:0px;--chakra-ring-offset-color:#fff;--chakra-ring-color:rgba(66, 153, 225, 0.6);--chakra-ring-offset-shadow:0 0 #0000;--chakra-ring-shadow:0 0 #0000;--chakra-space-x-reverse:0;--chakra-space-y-reverse:0;--chakra-colors-transparent:transparent;--chakra-colors-current:currentColor;--chakra-colors-black:#000000;--chakra-colors-white:#FFFFFF;--chakra-colors-whiteAlpha-50:rgba(255, 255, 255, 0.04);--chakra-colors-whiteAlpha-100:rgba(255, 255, 255, 0.06);--chakra-colors-whiteAlpha-200:rgba(255, 255, 255, 0.08);--chakra-colors-whiteAlpha-300:rgba(255, 255, 255, 0.16);--chakra-colors-whiteAlpha-400:rgba(255, 255, 255, 0.24);--chakra-colors-whiteAlpha-500:rgba(255, 255, 255, 0.36);--chakra-colors-whiteAlpha-600:rgba(255, 255, 255, 0.48);--chakra-colors-whiteAlpha-700:rgba(255, 255, 255, 0.64);--chakra-colors-whiteAlpha-800:rgba(255, 255, 255, 0.80);--chakra-colors-whiteAlpha-900:rgba(255, 255, 255, 0.92);--chakra-colors-blackAlpha-50:rgba(0, 0, 0, 0.04);--chakra-colors-blackAlpha-100:rgba(0, 0, 0, 0.06);--chakra-colors-blackAlpha-200:rgba(0, 0, 0, 0.08);--chakra-colors-blackAlpha-300:rgba(0, 0, 0, 0.16);--chakra-colors-blackAlpha-400:rgba(0, 0, 0, 0.24);--chakra-colors-blackAlpha-500:rgba(0, 0, 0, 0.36);--chakra-colors-blackAlpha-600:rgba(0, 0, 0, 0.48);--chakra-colors-blackAlpha-700:rgba(0, 0, 0, 0.64);--chakra-colors-blackAlpha-800:rgba(0, 0, 0, 0.80);--chakra-colors-blackAlpha-900:rgba(0, 0, 0, 0.92);--chakra-colors-gray-50:#F7FAFC;--chakra-colors-gray-100:#EDF2F7;--chakra-colors-gray-200:#E2E8F0;--chakra-colors-gray-300:#CBD5E0;--chakra-colors-gray-400:#A0AEC0;--chakra-colors-gray-500:#718096;--chakra-colors-gray-600:#4A5568;--chakra-colors-gray-700:#2D3748;--chakra-colors-gray-800:#1A202C;--chakra-colors-gray-900:#171923;--chakra-colors-red-50:#FFF5F5;--chakra-colors-red-100:#FED7D7;--chakra-colors-red-200:#FEB2B2;--chakra-colors-red-300:#FC8181;--chakra-colors-red-400:#F56565;--chakra-colors-red-500:#E53E3E;--chakra-colors-red-600:#C53030;--chakra-colors-red-700:#9B2C2C;--chakra-colors-red-800:#822727;--chakra-colors-red-900:#63171B;--chakra-colors-orange-50:#FFFAF0;--chakra-colors-orange-100:#FEEBC8;--chakra-colors-orange-200:#FBD38D;--chakra-colors-orange-300:#F6AD55;--chakra-colors-orange-400:#ED8936;--chakra-colors-orange-500:#DD6B20;--chakra-colors-orange-600:#C05621;--chakra-colors-orange-700:#9C4221;--chakra-colors-orange-800:#7B341E;--chakra-colors-orange-900:#652B19;--chakra-colors-yellow-50:#FFFFF0;--chakra-colors-yellow-100:#FEFCBF;--chakra-colors-yellow-200:#FAF089;--chakra-colors-yellow-300:#F6E05E;--chakra-colors-yellow-400:#ECC94B;--chakra-colors-yellow-500:#D69E2E;--chakra-colors-yellow-600:#B7791F;--chakra-colors-yellow-700:#975A16;--chakra-colors-yellow-800:#744210;--chakra-colors-yellow-900:#5F370E;--chakra-colors-green-50:#F0FFF4;--chakra-colors-green-100:#C6F6D5;--chakra-colors-green-200:#9AE6B4;--chakra-colors-green-300:#68D391;--chakra-colors-green-400:#48BB78;--chakra-colors-green-500:#38A169;--chakra-colors-green-600:#2F855A;--chakra-colors-green-700:#276749;--chakra-colors-green-800:#22543D;--chakra-colors-green-900:#1C4532;--chakra-colors-teal-50:#E6FFFA;--chakra-colors-teal-100:#B2F5EA;--chakra-colors-teal-200:#81E6D9;--chakra-colors-teal-300:#4FD1C5;--chakra-colors-teal-400:#38B2AC;--chakra-colors-teal-500:#319795;--chakra-colors-teal-600:#2C7A7B;--chakra-colors-teal-700:#285E61;--chakra-colors-teal-800:#234E52;--chakra-colors-teal-900:#1D4044;--chakra-colors-blue-50:#ebf8ff;--chakra-colors-blue-100:#bee3f8;--chakra-colors-blue-200:#90cdf4;--chakra-colors-blue-300:#63b3ed;--chakra-colors-blue-400:#4299e1;--chakra-colors-blue-500:#3182ce;--chakra-colors-blue-600:#2b6cb0;--chakra-colors-blue-700:#2c5282;--chakra-colors-blue-800:#2a4365;--chakra-colors-blue-900:#1A365D;--chakra-colors-cyan-50:#EDFDFD;--chakra-colors-cyan-100:#C4F1F9;--chakra-colors-cyan-200:#9DECF9;--chakra-colors-cyan-300:#76E4F7;--chakra-colors-cyan-400:#0BC5EA;--chakra-colors-cyan-500:#00B5D8;--chakra-colors-cyan-600:#00A3C4;--chakra-colors-cyan-700:#0987A0;--chakra-colors-cyan-800:#086F83;--chakra-colors-cyan-900:#065666;--chakra-colors-purple-50:#FAF5FF;--chakra-colors-purple-100:#E9D8FD;--chakra-colors-purple-200:#D6BCFA;--chakra-colors-purple-300:#B794F4;--chakra-colors-purple-400:#9F7AEA;--chakra-colors-purple-500:#805AD5;--chakra-colors-purple-600:#6B46C1;--chakra-colors-purple-700:#553C9A;--chakra-colors-purple-800:#44337A;--chakra-colors-purple-900:#322659;--chakra-colors-pink-50:#FFF5F7;--chakra-colors-pink-100:#FED7E2;--chakra-colors-pink-200:#FBB6CE;--chakra-colors-pink-300:#F687B3;--chakra-colors-pink-400:#ED64A6;--chakra-colors-pink-500:#D53F8C;--chakra-colors-pink-600:#B83280;--chakra-colors-pink-700:#97266D;--chakra-colors-pink-800:#702459;--chakra-colors-pink-900:#521B41;--chakra-colors-linkedin-50:#E8F4F9;--chakra-colors-linkedin-100:#CFEDFB;--chakra-colors-linkedin-200:#9BDAF3;--chakra-colors-linkedin-300:#68C7EC;--chakra-colors-linkedin-400:#34B3E4;--chakra-colors-linkedin-500:#00A0DC;--chakra-colors-linkedin-600:#008CC9;--chakra-colors-linkedin-700:#0077B5;--chakra-colors-linkedin-800:#005E93;--chakra-colors-linkedin-900:#004471;--chakra-colors-facebook-50:#E8F4F9;--chakra-colors-facebook-100:#D9DEE9;--chakra-colors-facebook-200:#B7C2DA;--chakra-colors-facebook-300:#6482C0;--chakra-colors-facebook-400:#4267B2;--chakra-colors-facebook-500:#385898;--chakra-colors-facebook-600:#314E89;--chakra-colors-facebook-700:#29487D;--chakra-colors-facebook-800:#223B67;--chakra-colors-facebook-900:#1E355B;--chakra-colors-messenger-50:#D0E6FF;--chakra-colors-messenger-100:#B9DAFF;--chakra-colors-messenger-200:#A2CDFF;--chakra-colors-messenger-300:#7AB8FF;--chakra-colors-messenger-400:#2E90FF;--chakra-colors-messenger-500:#0078FF;--chakra-colors-messenger-600:#0063D1;--chakra-colors-messenger-700:#0052AC;--chakra-colors-messenger-800:#003C7E;--chakra-colors-messenger-900:#002C5C;--chakra-colors-whatsapp-50:#dffeec;--chakra-colors-whatsapp-100:#b9f5d0;--chakra-colors-whatsapp-200:#90edb3;--chakra-colors-whatsapp-300:#65e495;--chakra-colors-whatsapp-400:#3cdd78;--chakra-colors-whatsapp-500:#22c35e;--chakra-colors-whatsapp-600:#179848;--chakra-colors-whatsapp-700:#0c6c33;--chakra-colors-whatsapp-800:#01421c;--chakra-colors-whatsapp-900:#001803;--chakra-colors-twitter-50:#E5F4FD;--chakra-colors-twitter-100:#C8E9FB;--chakra-colors-twitter-200:#A8DCFA;--chakra-colors-twitter-300:#83CDF7;--chakra-colors-twitter-400:#57BBF5;--chakra-colors-twitter-500:#1DA1F2;--chakra-colors-twitter-600:#1A94DA;--chakra-colors-twitter-700:#1681BF;--chakra-colors-twitter-800:#136B9E;--chakra-colors-twitter-900:#0D4D71;--chakra-colors-telegram-50:#E3F2F9;--chakra-colors-telegram-100:#C5E4F3;--chakra-colors-telegram-200:#A2D4EC;--chakra-colors-telegram-300:#7AC1E4;--chakra-colors-telegram-400:#47A9DA;--chakra-colors-telegram-500:#0088CC;--chakra-colors-telegram-600:#007AB8;--chakra-colors-telegram-700:#006BA1;--chakra-colors-telegram-800:#005885;--chakra-colors-telegram-900:#003F5E;--chakra-borders-none:0;--chakra-borders-1px:1px solid;--chakra-borders-2px:2px solid;--chakra-borders-4px:4px solid;--chakra-borders-8px:8px solid;--chakra-fonts-heading:-apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol";--chakra-fonts-body:-apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol";--chakra-fonts-mono:SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;--chakra-fontSizes-3xs:0.45rem;--chakra-fontSizes-2xs:0.625rem;--chakra-fontSizes-xs:0.75rem;--chakra-fontSizes-sm:0.875rem;--chakra-fontSizes-md:1rem;--chakra-fontSizes-lg:1.125rem;--chakra-fontSizes-xl:1.25rem;--chakra-fontSizes-2xl:1.5rem;--chakra-fontSizes-3xl:1.875rem;--chakra-fontSizes-4xl:2.25rem;--chakra-fontSizes-5xl:3rem;--chakra-fontSizes-6xl:3.75rem;--chakra-fontSizes-7xl:4.5rem;--chakra-fontSizes-8xl:6rem;--chakra-fontSizes-9xl:8rem;--chakra-fontWeights-hairline:100;--chakra-fontWeights-thin:200;--chakra-fontWeights-light:300;--chakra-fontWeights-normal:400;--chakra-fontWeights-medium:500;--chakra-fontWeights-semibold:600;--chakra-fontWeights-bold:700;--chakra-fontWeights-extrabold:800;--chakra-fontWeights-black:900;--chakra-letterSpacings-tighter:-0.05em;--chakra-letterSpacings-tight:-0.025em;--chakra-letterSpacings-normal:0;--chakra-letterSpacings-wide:0.025em;--chakra-letterSpacings-wider:0.05em;--chakra-letterSpacings-widest:0.1em;--chakra-lineHeights-3:.75rem;--chakra-lineHeights-4:1rem;--chakra-lineHeights-5:1.25rem;--chakra-lineHeights-6:1.5rem;--chakra-lineHeights-7:1.75rem;--chakra-lineHeights-8:2rem;--chakra-lineHeights-9:2.25rem;--chakra-lineHeights-10:2.5rem;--chakra-lineHeights-normal:normal;--chakra-lineHeights-none:1;--chakra-lineHeights-shorter:1.25;--chakra-lineHeights-short:1.375;--chakra-lineHeights-base:1.5;--chakra-lineHeights-tall:1.625;--chakra-lineHeights-taller:2;--chakra-radii-none:0;--chakra-radii-sm:0.125rem;--chakra-radii-base:0.25rem;--chakra-radii-md:0.375rem;--chakra-radii-lg:0.5rem;--chakra-radii-xl:0.75rem;--chakra-radii-2xl:1rem;--chakra-radii-3xl:1.5rem;--chakra-radii-full:9999px;--chakra-space-1:0.25rem;--chakra-space-2:0.5rem;--chakra-space-3:0.75rem;--chakra-space-4:1rem;--chakra-space-5:1.25rem;--chakra-space-6:1.5rem;--chakra-space-7:1.75rem;--chakra-space-8:2rem;--chakra-space-9:2.25rem;--chakra-space-10:2.5rem;--chakra-space-12:3rem;--chakra-space-14:3.5rem;--chakra-space-16:4rem;--chakra-space-20:5rem;--chakra-space-24:6rem;--chakra-space-28:7rem;--chakra-space-32:8rem;--chakra-space-36:9rem;--chakra-space-40:10rem;--chakra-space-44:11rem;--chakra-space-48:12rem;--chakra-space-52:13rem;--chakra-space-56:14rem;--chakra-space-60:15rem;--chakra-space-64:16rem;--chakra-space-72:18rem;--chakra-space-80:20rem;--chakra-space-96:24rem;--chakra-space-px:1px;--chakra-space-0-5:0.125rem;--chakra-space-1-5:0.375rem;--chakra-space-2-5:0.625rem;--chakra-space-3-5:0.875rem;--chakra-shadows-xs:0 0 0 1px rgba(0, 0, 0, 0.05);--chakra-shadows-sm:0 1px 2px 0 rgba(0, 0, 0, 0.05);--chakra-shadows-base:0 1px 3px 0 rgba(0, 0, 0, 0.1),0 1px 2px 0 rgba(0, 0, 0, 0.06);--chakra-shadows-md:0 4px 6px -1px rgba(0, 0, 0, 0.1),0 2px 4px -1px rgba(0, 0, 0, 0.06);--chakra-shadows-lg:0 10px 15px -3px rgba(0, 0, 0, 0.1),0 4px 6px -2px rgba(0, 0, 0, 0.05);--chakra-shadows-xl:0 20px 25px -5px rgba(0, 0, 0, 0.1),0 10px 10px -5px rgba(0, 0, 0, 0.04);--chakra-shadows-2xl:0 25px 50px -12px rgba(0, 0, 0, 0.25);--chakra-shadows-outline:0 0 0 3px rgba(66, 153, 225, 0.6);--chakra-shadows-inner:inset 0 2px 4px 0 rgba(0,0,0,0.06);--chakra-shadows-none:none;--chakra-shadows-dark-lg:rgba(0, 0, 0, 0.1) 0px 0px 0px 1px,rgba(0, 0, 0, 0.2) 0px 5px 10px,rgba(0, 0, 0, 0.4) 0px 15px 40px;--chakra-sizes-1:0.25rem;--chakra-sizes-2:0.5rem;--chakra-sizes-3:0.75rem;--chakra-sizes-4:1rem;--chakra-sizes-5:1.25rem;--chakra-sizes-6:1.5rem;--chakra-sizes-7:1.75rem;--chakra-sizes-8:2rem;--chakra-sizes-9:2.25rem;--chakra-sizes-10:2.5rem;--chakra-sizes-12:3rem;--chakra-sizes-14:3.5rem;--chakra-sizes-16:4rem;--chakra-sizes-20:5rem;--chakra-sizes-24:6rem;--chakra-sizes-28:7rem;--chakra-sizes-32:8rem;--chakra-sizes-36:9rem;--chakra-sizes-40:10rem;--chakra-sizes-44:11rem;--chakra-sizes-48:12rem;--chakra-sizes-52:13rem;--chakra-sizes-56:14rem;--chakra-sizes-60:15rem;--chakra-sizes-64:16rem;--chakra-sizes-72:18rem;--chakra-sizes-80:20rem;--chakra-sizes-96:24rem;--chakra-sizes-px:1px;--chakra-sizes-0-5:0.125rem;--chakra-sizes-1-5:0.375rem;--chakra-sizes-2-5:0.625rem;--chakra-sizes-3-5:0.875rem;--chakra-sizes-max:max-content;--chakra-sizes-min:min-content;--chakra-sizes-full:100%;--chakra-sizes-3xs:14rem;--chakra-sizes-2xs:16rem;--chakra-sizes-xs:20rem;--chakra-sizes-sm:24rem;--chakra-sizes-md:28rem;--chakra-sizes-lg:32rem;--chakra-sizes-xl:36rem;--chakra-sizes-2xl:42rem;--chakra-sizes-3xl:48rem;--chakra-sizes-4xl:56rem;--chakra-sizes-5xl:64rem;--chakra-sizes-6xl:72rem;--chakra-sizes-7xl:80rem;--chakra-sizes-8xl:90rem;--chakra-sizes-prose:60ch;--chakra-sizes-container-sm:640px;--chakra-sizes-container-md:768px;--chakra-sizes-container-lg:1024px;--chakra-sizes-container-xl:1280px;--chakra-zIndices-hide:-1;--chakra-zIndices-auto:auto;--chakra-zIndices-base:0;--chakra-zIndices-docked:10;--chakra-zIndices-dropdown:1000;--chakra-zIndices-sticky:1100;--chakra-zIndices-banner:1200;--chakra-zIndices-overlay:1300;--chakra-zIndices-modal:1400;--chakra-zIndices-popover:1500;--chakra-zIndices-skipLink:1600;--chakra-zIndices-toast:1700;--chakra-zIndices-tooltip:1800;--chakra-transition-property-common:background-color,border-color,color,fill,stroke,opacity,box-shadow,transform;--chakra-transition-property-colors:background-color,border-color,color,fill,stroke;--chakra-transition-property-dimensions:width,height;--chakra-transition-property-position:left,right,top,bottom;--chakra-transition-property-background:background-color,background-image,background-position;--chakra-transition-easing-ease-in:cubic-bezier(0.4, 0, 1, 1);--chakra-transition-easing-ease-out:cubic-bezier(0, 0, 0.2, 1);--chakra-transition-easing-ease-in-out:cubic-bezier(0.4, 0, 0.2, 1);--chakra-transition-duration-ultra-fast:50ms;--chakra-transition-duration-faster:100ms;--chakra-transition-duration-fast:150ms;--chakra-transition-duration-normal:200ms;--chakra-transition-duration-slow:300ms;--chakra-transition-duration-slower:400ms;--chakra-transition-duration-ultra-slow:500ms;--chakra-blur-none:0;--chakra-blur-sm:4px;--chakra-blur-base:8px;--chakra-blur-md:12px;--chakra-blur-lg:16px;--chakra-blur-xl:24px;--chakra-blur-2xl:40px;--chakra-blur-3xl:64px;--chakra-breakpoints-base:0em;--chakra-breakpoints-sm:30em;--chakra-breakpoints-md:48em;--chakra-breakpoints-lg:62em;--chakra-breakpoints-xl:80em;--chakra-breakpoints-2xl:96em;}.chakra-ui-light :host:not([data-theme]),.chakra-ui-light :root:not([data-theme]),.chakra-ui-light [data-theme]:not([data-theme]),[data-theme=light] :host:not([data-theme]),[data-theme=light] :root:not([data-theme]),[data-theme=light] [data-theme]:not([data-theme]),:host[data-theme=light],:root[data-theme=light],[data-theme][data-theme=light]{--chakra-colors-chakra-body-text:var(--chakra-colors-gray-800);--chakra-colors-chakra-body-bg:var(--chakra-colors-white);--chakra-colors-chakra-border-color:var(--chakra-colors-gray-200);--chakra-colors-chakra-inverse-text:var(--chakra-colors-white);--chakra-colors-chakra-subtle-bg:var(--chakra-colors-gray-100);--chakra-colors-chakra-subtle-text:var(--chakra-colors-gray-600);--chakra-colors-chakra-placeholder-color:var(--chakra-colors-gray-500);}.chakra-ui-dark :host:not([data-theme]),.chakra-ui-dark :root:not([data-theme]),.chakra-ui-dark [data-theme]:not([data-theme]),[data-theme=dark] :host:not([data-theme]),[data-theme=dark] :root:not([data-theme]),[data-theme=dark] [data-theme]:not([data-theme]),:host[data-theme=dark],:root[data-theme=dark],[data-theme][data-theme=dark]{--chakra-colors-chakra-body-text:var(--chakra-colors-whiteAlpha-900);--chakra-colors-chakra-body-bg:var(--chakra-colors-gray-800);--chakra-colors-chakra-border-color:var(--chakra-colors-whiteAlpha-300);--chakra-colors-chakra-inverse-text:var(--chakra-colors-gray-800);--chakra-colors-chakra-subtle-bg:var(--chakra-colors-gray-700);--chakra-colors-chakra-subtle-text:var(--chakra-colors-gray-400);--chakra-colors-chakra-placeholder-color:var(--chakra-colors-whiteAlpha-400);}</style><style data-emotion="css-global fubdgu">html{line-height:1.5;-webkit-text-size-adjust:100%;font-family:system-ui,sans-serif;-webkit-font-smoothing:antialiased;text-rendering:optimizeLegibility;-moz-osx-font-smoothing:grayscale;touch-action:manipulation;}body{position:relative;min-height:100%;margin:0;font-feature-settings:"kern";}:where(*, *::before, *::after){border-width:0;border-style:solid;box-sizing:border-box;word-wrap:break-word;}main{display:block;}hr{border-top-width:1px;box-sizing:content-box;height:0;overflow:visible;}:where(pre, code, kbd,samp){font-family:SFMono-Regular,Menlo,Monaco,Consolas,monospace;font-size:1em;}a{background-color:transparent;color:inherit;-webkit-text-decoration:inherit;text-decoration:inherit;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;-webkit-text-decoration:underline dotted;-webkit-text-decoration:underline dotted;text-decoration:underline dotted;}:where(b, strong){font-weight:bold;}small{font-size:80%;}:where(sub,sup){font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sub{bottom:-0.25em;}sup{top:-0.5em;}img{border-style:none;}:where(button, input, optgroup, select, textarea){font-family:inherit;font-size:100%;line-height:1.15;margin:0;}:where(button, input){overflow:visible;}:where(button, select){text-transform:none;}:where(
           button::-moz-focus-inner,
           [type="button"]::-moz-focus-inner,
           [type="reset"]::-moz-focus-inner,
           [type="submit"]::-moz-focus-inner
         ){border-style:none;padding:0;}fieldset{padding:0.35em 0.75em 0.625em;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{vertical-align:baseline;}textarea{overflow:auto;}:where([type="checkbox"], [type="radio"]){box-sizing:border-box;padding:0;}input[type="number"]::-webkit-inner-spin-button,input[type="number"]::-webkit-outer-spin-button{-webkit-appearance:none!important;}input[type="number"]{-moz-appearance:textfield;}input[type="search"]{-webkit-appearance:textfield;outline-offset:-2px;}input[type="search"]::-webkit-search-decoration{-webkit-appearance:none!important;}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit;}details{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}template{display:none;}[hidden]{display:none!important;}:where(
           blockquote,
           dl,
@@ -15,8 +15,8 @@
           h6,
           hr,
           figure,
           p,
           pre
         ){margin:0;}button{background:transparent;padding:0;}fieldset{margin:0;padding:0;}:where(ol, ul){margin:0;padding:0;}textarea{resize:vertical;}:where(button, [role="button"]){cursor:pointer;}button::-moz-focus-inner{border:0!important;}table{border-collapse:collapse;}:where(h1, h2, h3, h4, h5, h6){font-size:inherit;font-weight:inherit;}:where(button, input, optgroup, select, textarea){padding:0;line-height:inherit;color:inherit;}:where(img, svg, video, canvas, audio, iframe, embed, object){display:block;}:where(img, video){max-width:100%;height:auto;}[data-js-focus-visible] :focus:not([data-focus-visible-added]):not(
           [data-focus-visible-disabled]
-        ){outline:none;box-shadow:none;}select::-ms-expand{display:none;}:root,:host{--chakra-vh:100vh;}@supports (height: -webkit-fill-available){:root,:host{--chakra-vh:-webkit-fill-available;}}@supports (height: -moz-fill-available){:root,:host{--chakra-vh:-moz-fill-available;}}@supports (height: 100dvh){:root,:host{--chakra-vh:100dvh;}}</style><style data-emotion="css-global 1cgn62j">body{font-family:var(--chakra-fonts-body);color:var(--chakra-colors-chakra-body-text);background:var(--chakra-colors-chakra-body-bg);transition-property:background-color;transition-duration:var(--chakra-transition-duration-normal);line-height:var(--chakra-lineHeights-base);}*::-webkit-input-placeholder{color:var(--chakra-colors-chakra-placeholder-color);}*::-moz-placeholder{color:var(--chakra-colors-chakra-placeholder-color);}*:-ms-input-placeholder{color:var(--chakra-colors-chakra-placeholder-color);}*::placeholder{color:var(--chakra-colors-chakra-placeholder-color);}*,*::before,::after{border-color:var(--chakra-colors-chakra-border-color);}</style><style data-emotion="css s92abg">.css-s92abg{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;height:100vh;}</style><div class="css-s92abg"><style data-emotion="css 1xpribl">.css-1xpribl{position:relative;display:block;}</style><div class="chakra-tabs css-1xpribl"><style data-emotion="css 1xhq01z">.css-1xhq01z{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;border-bottom:2px solid;border-color:inherit;}</style><div role="tablist" aria-orientation="horizontal" class="chakra-tabs__tablist css-1xhq01z"><style data-emotion="css 52dxnr">.css-52dxnr{outline:2px solid transparent;outline-offset:2px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;transition-property:var(--chakra-transition-property-common);transition-duration:var(--chakra-transition-duration-normal);font-size:var(--chakra-fontSizes-md);padding-top:var(--chakra-space-2);padding-bottom:var(--chakra-space-2);-webkit-padding-start:var(--chakra-space-4);padding-inline-start:var(--chakra-space-4);-webkit-padding-end:var(--chakra-space-4);padding-inline-end:var(--chakra-space-4);border-bottom:2px solid;border-color:var(--chakra-colors-transparent);margin-bottom:-2px;color:var(--tabs-color);background:var(--tabs-bg);}.css-52dxnr:focus-visible,.css-52dxnr[data-focus-visible]{z-index:1;box-shadow:var(--chakra-shadows-outline);}.css-52dxnr:disabled,.css-52dxnr[disabled],.css-52dxnr[aria-disabled=true],.css-52dxnr[data-disabled]{cursor:not-allowed;opacity:0.4;}.css-52dxnr:disabled:active,.css-52dxnr[disabled]:active,.css-52dxnr[aria-disabled=true]:active,.css-52dxnr[data-disabled]:active,.css-52dxnr:disabled[data-active],.css-52dxnr[disabled][data-active],.css-52dxnr[aria-disabled=true][data-active],.css-52dxnr[data-disabled][data-active]{background:none;}.css-52dxnr[aria-selected=true],.css-52dxnr[data-selected]{--tabs-color:var(--chakra-colors-blue-600);border-color:currentColor;}.chakra-ui-dark .css-52dxnr[aria-selected=true]:not([data-theme]),.chakra-ui-dark .css-52dxnr[data-selected]:not([data-theme]),[data-theme=dark] .css-52dxnr[aria-selected=true]:not([data-theme]),[data-theme=dark] .css-52dxnr[data-selected]:not([data-theme]),.css-52dxnr[aria-selected=true][data-theme=dark],.css-52dxnr[data-selected][data-theme=dark]{--tabs-color:var(--chakra-colors-blue-300);}.css-52dxnr:active,.css-52dxnr[data-active]{--tabs-bg:var(--chakra-colors-gray-200);}.chakra-ui-dark .css-52dxnr:active:not([data-theme]),.chakra-ui-dark .css-52dxnr[data-active]:not([data-theme]),[data-theme=dark] .css-52dxnr:active:not([data-theme]),[data-theme=dark] .css-52dxnr[data-active]:not([data-theme]),.css-52dxnr:active[data-theme=dark],.css-52dxnr[data-active][data-theme=dark]{--tabs-bg:var(--chakra-colors-whiteAlpha-300);}</style><button type="button" aria-disabled="false" id="tabs-:R2liunla:--tab--1" role="tab" tabindex="0" aria-selected="true" aria-controls="tabs-:R2liunla:--tabpanel--1" class="chakra-tabs__tab css-52dxnr">Lineage</button><button type="button" aria-disabled="false" id="tabs-:R2liunla:--tab--1" role="tab" tabindex="0" aria-selected="true" aria-controls="tabs-:R2liunla:--tabpanel--1" class="chakra-tabs__tab css-52dxnr">Query</button><button type="button" aria-disabled="false" id="tabs-:R2liunla:--tab--1" role="tab" tabindex="0" aria-selected="true" aria-controls="tabs-:R2liunla:--tabpanel--1" class="chakra-tabs__tab css-52dxnr">Checklist</button><style data-emotion="css 1g340lv">.css-1g340lv{position:absolute;right:0px;top:0px;padding:var(--chakra-space-2);color:var(--chakra-colors-gray-500);}</style><div class="css-1g340lv"></div></div></div><style data-emotion="css ene2ut">.css-ene2ut{padding:0px;overflow:auto;-webkit-flex:1;-ms-flex:1;flex:1;}</style><div style="contain:size" class="css-ene2ut"><style data-emotion="css 1s3dmby">.css-1s3dmby{display:none;height:100%;}</style><div class="css-1s3dmby"><style data-emotion="css 1r1bp18">.css-1r1bp18{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;width:100%;height:100%;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}</style><div class="css-1r1bp18"><style data-emotion="css jmuyva animation-b7n1on">.css-jmuyva{display:inline-block;border-color:currentColor;border-style:solid;border-radius:99999px;border-width:2px;border-bottom-color:var(--chakra-colors-transparent);border-left-color:var(--chakra-colors-transparent);-webkit-animation:animation-b7n1on 0.45s linear infinite;animation:animation-b7n1on 0.45s linear infinite;width:var(--spinner-size);height:var(--spinner-size);--spinner-size:var(--chakra-sizes-12);}@-webkit-keyframes animation-b7n1on{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-b7n1on{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><div class="chakra-spinner css-jmuyva"><style data-emotion="css 8b45rq">.css-8b45rq{border:0px;clip:rect(0, 0, 0, 0);width:1px;height:1px;margin:-1px;padding:0px;overflow:hidden;white-space:nowrap;position:absolute;}</style><span class="css-8b45rq">Loading...</span></div></div></div>Loading</div></div><span></span><span id="__chakra_env" hidden=""></span><script src="/_next/static/chunks/webpack-2d4823656eaa7d1c.js" crossorigin="" async=""></script><script>(self.__next_f=self.__next_f||[]).push([0]);self.__next_f.push([2,null])</script><script>self.__next_f.push([1,"0:\"$L1\"\n"])</script><script>self.__next_f.push([1,"2:HL[\"/_next/static/css/6d0611c21a82d0bb.css\",\"style\",{\"crossOrigin\":\"\"}]\n"])</script><script>self.__next_f.push([1,"3:I[61886,[],\"\"]\n5:I[35774,[],\"\"]\n6:I[44813,[],\"\"]\n7:I[82593,[],\"\"]\n9:I[32658,[],\"\"]\n"])</script><script>self.__next_f.push([1,"a:I[26331,[\"634\",\"static/chunks/7c9ab469-732af37965d79ccf.js\",\"145\",\"static/chunks/fb2d5402-0ccc92fc728c2993.js\",\"170\",\"static/chunks/526a6206-7ccbd30e159c1652.js\",\"521\",\"static/chunks/607285b2-dadd48144d45dbcf.js\",\"462\",\"static/chunks/f6be744d-5973a409ea097354.js\",\"531\",\"static/chunks/f78b7092-bf8a8853eef36a4c.js\",\"498\",\"static/chunks/6af6e714-6003aba9c53d2dcd.js\",\"685\",\"static/chunks/030e0bea-59754f62ad2a287c.js\",\"182\",\"static/chunks/5e9a126f-da62af62011c0643.js\",\"710\",\"static/chunks/2d02f0f7-ed3b4e4daa7c5d22.js\",\"971\",\"static/chunks/49348413-7aacf235ca16afb9.js\",\"495\",\"static/chunks/6dc81886-a3fa8efdc3652e8f.js\",\"599\",\"static/chunks/c132bf7d-fca1bc3c8aa231eb.js\",\"512\",\"static/chunks/4b89641d-a80e6024cd2468dc.js\",\"354\",\"static/chunks/354-d94f5f7615bdde2d.js\",\"931\",\"static/chunks/app/page-11d757976ef71345.js\"],\"\"]\n"])</script><script>self.__next_f.push([1,"1:[null,[\"$\",\"$L3\",null,{\"buildId\":\"OSDAXs6UrZSM40dV34eY3\",\"assetPrefix\":\"\",\"initialCanonicalUrl\":\"/\",\"initialTree\":[\"\",{\"children\":[\"__PAGE__\",{}]},\"$undefined\",\"$undefined\",true],\"initialHead\":[false,\"$L4\"],\"globalErrorComponent\":\"$5\",\"children\":[null,[\"$\",\"html\",null,{\"lang\":\"en\",\"children\":[\"$\",\"body\",null,{\"suppressHydrationWarning\":true,\"children\":[\"$\",\"$L6\",null,{\"parallelRouterKey\":\"children\",\"segmentPath\":[\"children\"],\"loading\":\"$undefined\",\"loadingStyles\":\"$undefined\",\"loadingScripts\":\"$undefined\",\"hasLoading\":false,\"error\":\"$undefined\",\"errorStyles\":\"$undefined\",\"errorScripts\":\"$undefined\",\"template\":[\"$\",\"$L7\",null,{}],\"templateStyles\":\"$undefined\",\"templateScripts\":\"$undefined\",\"notFound\":[[\"$\",\"title\",null,{\"children\":\"404: This page could not be found.\"}],[\"$\",\"div\",null,{\"style\":{\"fontFamily\":\"system-ui,\\\"Segoe UI\\\",Roboto,Helvetica,Arial,sans-serif,\\\"Apple Color Emoji\\\",\\\"Segoe UI Emoji\\\"\",\"height\":\"100vh\",\"textAlign\":\"center\",\"display\":\"flex\",\"flexDirection\":\"column\",\"alignItems\":\"center\",\"justifyContent\":\"center\"},\"children\":[\"$\",\"div\",null,{\"children\":[[\"$\",\"style\",null,{\"dangerouslySetInnerHTML\":{\"__html\":\"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}\"}}],[\"$\",\"h1\",null,{\"className\":\"next-error-h1\",\"style\":{\"display\":\"inline-block\",\"margin\":\"0 20px 0 0\",\"padding\":\"0 23px 0 0\",\"fontSize\":24,\"fontWeight\":500,\"verticalAlign\":\"top\",\"lineHeight\":\"49px\"},\"children\":\"404\"}],[\"$\",\"div\",null,{\"style\":{\"display\":\"inline-block\"},\"children\":[\"$\",\"h2\",null,{\"style\":{\"fontSize\":14,\"fontWeight\":400,\"lineHeight\":\"49px\",\"margin\":0},\"children\":\"This page could not be found.\"}]}]]}]}]],\"notFoundStyles\":[],\"childProp\":{\"current\":[\"$L8\",[\"$\",\"$L9\",null,{\"propsForComponent\":{\"params\":{}},\"Component\":\"$a\",\"isStaticGeneration\":true}],null],\"segment\":\"__PAGE__\"},\"styles\":[[\"$\",\"link\",\"0\",{\"rel\":\"stylesheet\",\"href\":\"/_next/static/css/6d0611c21a82d0bb.css\",\"precedence\":\"next\",\"crossOrigin\":\"\"}]]}]}]}],null]}]]\n"])</script><script>self.__next_f.push([1,"4:[[\"$\",\"meta\",\"0\",{\"name\":\"viewport\",\"content\":\"width=device-width, initial-scale=1\"}],[\"$\",\"meta\",\"1\",{\"charSet\":\"utf-8\"}],[\"$\",\"title\",\"2\",{\"children\":\"recce\"}],[\"$\",\"meta\",\"3\",{\"name\":\"description\",\"content\":\"Recce: a dbt tool\"}],[\"$\",\"link\",\"4\",{\"rel\":\"icon\",\"href\":\"/favicon.ico\",\"type\":\"image/x-icon\",\"sizes\":\"16x16\"}]]\n8:null\n"])</script><script>self.__next_f.push([1,""])</script></body></html>
+        ){outline:none;box-shadow:none;}select::-ms-expand{display:none;}:root,:host{--chakra-vh:100vh;}@supports (height: -webkit-fill-available){:root,:host{--chakra-vh:-webkit-fill-available;}}@supports (height: -moz-fill-available){:root,:host{--chakra-vh:-moz-fill-available;}}@supports (height: 100dvh){:root,:host{--chakra-vh:100dvh;}}</style><style data-emotion="css-global 1cgn62j">body{font-family:var(--chakra-fonts-body);color:var(--chakra-colors-chakra-body-text);background:var(--chakra-colors-chakra-body-bg);transition-property:background-color;transition-duration:var(--chakra-transition-duration-normal);line-height:var(--chakra-lineHeights-base);}*::-webkit-input-placeholder{color:var(--chakra-colors-chakra-placeholder-color);}*::-moz-placeholder{color:var(--chakra-colors-chakra-placeholder-color);}*:-ms-input-placeholder{color:var(--chakra-colors-chakra-placeholder-color);}*::placeholder{color:var(--chakra-colors-chakra-placeholder-color);}*,*::before,::after{border-color:var(--chakra-colors-chakra-border-color);}</style><style data-emotion="css s92abg">.css-s92abg{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;height:100vh;}</style><div class="css-s92abg"><style data-emotion="css 1xpribl">.css-1xpribl{position:relative;display:block;}</style><div class="chakra-tabs css-1xpribl"><style data-emotion="css 1xhq01z">.css-1xhq01z{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;border-bottom:2px solid;border-color:inherit;}</style><div role="tablist" aria-orientation="horizontal" class="chakra-tabs__tablist css-1xhq01z"><style data-emotion="css 52dxnr">.css-52dxnr{outline:2px solid transparent;outline-offset:2px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;transition-property:var(--chakra-transition-property-common);transition-duration:var(--chakra-transition-duration-normal);font-size:var(--chakra-fontSizes-md);padding-top:var(--chakra-space-2);padding-bottom:var(--chakra-space-2);-webkit-padding-start:var(--chakra-space-4);padding-inline-start:var(--chakra-space-4);-webkit-padding-end:var(--chakra-space-4);padding-inline-end:var(--chakra-space-4);border-bottom:2px solid;border-color:var(--chakra-colors-transparent);margin-bottom:-2px;color:var(--tabs-color);background:var(--tabs-bg);}.css-52dxnr:focus-visible,.css-52dxnr[data-focus-visible]{z-index:1;box-shadow:var(--chakra-shadows-outline);}.css-52dxnr:disabled,.css-52dxnr[disabled],.css-52dxnr[aria-disabled=true],.css-52dxnr[data-disabled]{cursor:not-allowed;opacity:0.4;}.css-52dxnr:disabled:active,.css-52dxnr[disabled]:active,.css-52dxnr[aria-disabled=true]:active,.css-52dxnr[data-disabled]:active,.css-52dxnr:disabled[data-active],.css-52dxnr[disabled][data-active],.css-52dxnr[aria-disabled=true][data-active],.css-52dxnr[data-disabled][data-active]{background:none;}.css-52dxnr[aria-selected=true],.css-52dxnr[data-selected]{--tabs-color:var(--chakra-colors-blue-600);border-color:currentColor;}.chakra-ui-dark .css-52dxnr[aria-selected=true]:not([data-theme]),.chakra-ui-dark .css-52dxnr[data-selected]:not([data-theme]),[data-theme=dark] .css-52dxnr[aria-selected=true]:not([data-theme]),[data-theme=dark] .css-52dxnr[data-selected]:not([data-theme]),.css-52dxnr[aria-selected=true][data-theme=dark],.css-52dxnr[data-selected][data-theme=dark]{--tabs-color:var(--chakra-colors-blue-300);}.css-52dxnr:active,.css-52dxnr[data-active]{--tabs-bg:var(--chakra-colors-gray-200);}.chakra-ui-dark .css-52dxnr:active:not([data-theme]),.chakra-ui-dark .css-52dxnr[data-active]:not([data-theme]),[data-theme=dark] .css-52dxnr:active:not([data-theme]),[data-theme=dark] .css-52dxnr[data-active]:not([data-theme]),.css-52dxnr:active[data-theme=dark],.css-52dxnr[data-active][data-theme=dark]{--tabs-bg:var(--chakra-colors-whiteAlpha-300);}</style><button type="button" aria-disabled="false" id="tabs-:R2liunla:--tab--1" role="tab" tabindex="0" aria-selected="true" aria-controls="tabs-:R2liunla:--tabpanel--1" class="chakra-tabs__tab css-52dxnr">Lineage</button><button type="button" aria-disabled="false" id="tabs-:R2liunla:--tab--1" role="tab" tabindex="0" aria-selected="true" aria-controls="tabs-:R2liunla:--tabpanel--1" class="chakra-tabs__tab css-52dxnr">Query</button><button type="button" aria-disabled="false" id="tabs-:R2liunla:--tab--1" role="tab" tabindex="0" aria-selected="true" aria-controls="tabs-:R2liunla:--tabpanel--1" class="chakra-tabs__tab css-52dxnr">Checklist</button><style data-emotion="css 1g340lv">.css-1g340lv{position:absolute;right:0px;top:0px;padding:var(--chakra-space-2);color:var(--chakra-colors-gray-500);}</style><div class="css-1g340lv"></div></div></div><style data-emotion="css ene2ut">.css-ene2ut{padding:0px;overflow:auto;-webkit-flex:1;-ms-flex:1;flex:1;}</style><div style="contain:size" class="css-ene2ut"><style data-emotion="css 1s3dmby">.css-1s3dmby{display:none;height:100%;}</style><div class="css-1s3dmby"><style data-emotion="css 1r1bp18">.css-1r1bp18{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;width:100%;height:100%;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}</style><div class="css-1r1bp18"><style data-emotion="css jmuyva animation-b7n1on">.css-jmuyva{display:inline-block;border-color:currentColor;border-style:solid;border-radius:99999px;border-width:2px;border-bottom-color:var(--chakra-colors-transparent);border-left-color:var(--chakra-colors-transparent);-webkit-animation:animation-b7n1on 0.45s linear infinite;animation:animation-b7n1on 0.45s linear infinite;width:var(--spinner-size);height:var(--spinner-size);--spinner-size:var(--chakra-sizes-12);}@-webkit-keyframes animation-b7n1on{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-b7n1on{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><div class="chakra-spinner css-jmuyva"><style data-emotion="css 8b45rq">.css-8b45rq{border:0px;clip:rect(0, 0, 0, 0);width:1px;height:1px;margin:-1px;padding:0px;overflow:hidden;white-space:nowrap;position:absolute;}</style><span class="css-8b45rq">Loading...</span></div></div></div>Loading</div></div><span></span><span id="__chakra_env" hidden=""></span><script src="/_next/static/chunks/webpack-2d4823656eaa7d1c.js" crossorigin="" async=""></script><script>(self.__next_f=self.__next_f||[]).push([0]);self.__next_f.push([2,null])</script><script>self.__next_f.push([1,"0:\"$L1\"\n"])</script><script>self.__next_f.push([1,"2:HL[\"/_next/static/css/6d0611c21a82d0bb.css\",\"style\",{\"crossOrigin\":\"\"}]\n"])</script><script>self.__next_f.push([1,"3:I[61886,[],\"\"]\n5:I[35774,[],\"\"]\n6:I[44813,[],\"\"]\n7:I[82593,[],\"\"]\n9:I[32658,[],\"\"]\n"])</script><script>self.__next_f.push([1,"a:I[13512,[\"634\",\"static/chunks/7c9ab469-732af37965d79ccf.js\",\"145\",\"static/chunks/fb2d5402-0ccc92fc728c2993.js\",\"170\",\"static/chunks/526a6206-7ccbd30e159c1652.js\",\"521\",\"static/chunks/607285b2-dadd48144d45dbcf.js\",\"462\",\"static/chunks/f6be744d-5973a409ea097354.js\",\"531\",\"static/chunks/f78b7092-bf8a8853eef36a4c.js\",\"498\",\"static/chunks/6af6e714-6003aba9c53d2dcd.js\",\"685\",\"static/chunks/030e0bea-59754f62ad2a287c.js\",\"182\",\"static/chunks/5e9a126f-da62af62011c0643.js\",\"710\",\"static/chunks/2d02f0f7-ed3b4e4daa7c5d22.js\",\"971\",\"static/chunks/49348413-7aacf235ca16afb9.js\",\"495\",\"static/chunks/6dc81886-a3fa8efdc3652e8f.js\",\"599\",\"static/chunks/c132bf7d-fca1bc3c8aa231eb.js\",\"512\",\"static/chunks/4b89641d-a80e6024cd2468dc.js\",\"354\",\"static/chunks/354-d94f5f7615bdde2d.js\",\"931\",\"static/chunks/app/page-2e986eecfb9156dd.js\"],\"\"]\n"])</script><script>self.__next_f.push([1,"1:[null,[\"$\",\"$L3\",null,{\"buildId\":\"k9hThvy5xnFYnWlSYKB0A\",\"assetPrefix\":\"\",\"initialCanonicalUrl\":\"/\",\"initialTree\":[\"\",{\"children\":[\"__PAGE__\",{}]},\"$undefined\",\"$undefined\",true],\"initialHead\":[false,\"$L4\"],\"globalErrorComponent\":\"$5\",\"children\":[null,[\"$\",\"html\",null,{\"lang\":\"en\",\"children\":[\"$\",\"body\",null,{\"suppressHydrationWarning\":true,\"children\":[\"$\",\"$L6\",null,{\"parallelRouterKey\":\"children\",\"segmentPath\":[\"children\"],\"loading\":\"$undefined\",\"loadingStyles\":\"$undefined\",\"loadingScripts\":\"$undefined\",\"hasLoading\":false,\"error\":\"$undefined\",\"errorStyles\":\"$undefined\",\"errorScripts\":\"$undefined\",\"template\":[\"$\",\"$L7\",null,{}],\"templateStyles\":\"$undefined\",\"templateScripts\":\"$undefined\",\"notFound\":[[\"$\",\"title\",null,{\"children\":\"404: This page could not be found.\"}],[\"$\",\"div\",null,{\"style\":{\"fontFamily\":\"system-ui,\\\"Segoe UI\\\",Roboto,Helvetica,Arial,sans-serif,\\\"Apple Color Emoji\\\",\\\"Segoe UI Emoji\\\"\",\"height\":\"100vh\",\"textAlign\":\"center\",\"display\":\"flex\",\"flexDirection\":\"column\",\"alignItems\":\"center\",\"justifyContent\":\"center\"},\"children\":[\"$\",\"div\",null,{\"children\":[[\"$\",\"style\",null,{\"dangerouslySetInnerHTML\":{\"__html\":\"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}\"}}],[\"$\",\"h1\",null,{\"className\":\"next-error-h1\",\"style\":{\"display\":\"inline-block\",\"margin\":\"0 20px 0 0\",\"padding\":\"0 23px 0 0\",\"fontSize\":24,\"fontWeight\":500,\"verticalAlign\":\"top\",\"lineHeight\":\"49px\"},\"children\":\"404\"}],[\"$\",\"div\",null,{\"style\":{\"display\":\"inline-block\"},\"children\":[\"$\",\"h2\",null,{\"style\":{\"fontSize\":14,\"fontWeight\":400,\"lineHeight\":\"49px\",\"margin\":0},\"children\":\"This page could not be found.\"}]}]]}]}]],\"notFoundStyles\":[],\"childProp\":{\"current\":[\"$L8\",[\"$\",\"$L9\",null,{\"propsForComponent\":{\"params\":{}},\"Component\":\"$a\",\"isStaticGeneration\":true}],null],\"segment\":\"__PAGE__\"},\"styles\":[[\"$\",\"link\",\"0\",{\"rel\":\"stylesheet\",\"href\":\"/_next/static/css/6d0611c21a82d0bb.css\",\"precedence\":\"next\",\"crossOrigin\":\"\"}]]}]}]}],null]}]]\n"])</script><script>self.__next_f.push([1,"4:[[\"$\",\"meta\",\"0\",{\"name\":\"viewport\",\"content\":\"width=device-width, initial-scale=1\"}],[\"$\",\"meta\",\"1\",{\"charSet\":\"utf-8\"}],[\"$\",\"title\",\"2\",{\"children\":\"recce\"}],[\"$\",\"meta\",\"3\",{\"name\":\"description\",\"content\":\"Recce: a dbt tool\"}],[\"$\",\"link\",\"4\",{\"rel\":\"icon\",\"href\":\"/favicon.ico\",\"type\":\"image/x-icon\",\"sizes\":\"16x16\"}]]\n8:null\n"])</script><script>self.__next_f.push([1,""])</script></body></html>
```

### Comparing `recce-nightly-0.9.0.20240312/recce/data/index.txt` & `recce-nightly-0.9.0.20240313/recce/data/index.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-0:["OSDAXs6UrZSM40dV34eY3",[[["",{"children":["__PAGE__",{}]},"$undefined","$undefined",true],"$L1",[null,"$L2"]]]]
+0:["k9hThvy5xnFYnWlSYKB0A",[[["",{"children":["__PAGE__",{}]},"$undefined","$undefined",true],"$L1",[null,"$L2"]]]]
 3:HL["/_next/static/css/6d0611c21a82d0bb.css","style",{"crossOrigin":""}]
 4:I[44813,[],""]
 5:I[82593,[],""]
 7:I[32658,[],""]
-8:I[26331,["634","static/chunks/7c9ab469-732af37965d79ccf.js","145","static/chunks/fb2d5402-0ccc92fc728c2993.js","170","static/chunks/526a6206-7ccbd30e159c1652.js","521","static/chunks/607285b2-dadd48144d45dbcf.js","462","static/chunks/f6be744d-5973a409ea097354.js","531","static/chunks/f78b7092-bf8a8853eef36a4c.js","498","static/chunks/6af6e714-6003aba9c53d2dcd.js","685","static/chunks/030e0bea-59754f62ad2a287c.js","182","static/chunks/5e9a126f-da62af62011c0643.js","710","static/chunks/2d02f0f7-ed3b4e4daa7c5d22.js","971","static/chunks/49348413-7aacf235ca16afb9.js","495","static/chunks/6dc81886-a3fa8efdc3652e8f.js","599","static/chunks/c132bf7d-fca1bc3c8aa231eb.js","512","static/chunks/4b89641d-a80e6024cd2468dc.js","354","static/chunks/354-d94f5f7615bdde2d.js","931","static/chunks/app/page-11d757976ef71345.js"],""]
+8:I[13512,["634","static/chunks/7c9ab469-732af37965d79ccf.js","145","static/chunks/fb2d5402-0ccc92fc728c2993.js","170","static/chunks/526a6206-7ccbd30e159c1652.js","521","static/chunks/607285b2-dadd48144d45dbcf.js","462","static/chunks/f6be744d-5973a409ea097354.js","531","static/chunks/f78b7092-bf8a8853eef36a4c.js","498","static/chunks/6af6e714-6003aba9c53d2dcd.js","685","static/chunks/030e0bea-59754f62ad2a287c.js","182","static/chunks/5e9a126f-da62af62011c0643.js","710","static/chunks/2d02f0f7-ed3b4e4daa7c5d22.js","971","static/chunks/49348413-7aacf235ca16afb9.js","495","static/chunks/6dc81886-a3fa8efdc3652e8f.js","599","static/chunks/c132bf7d-fca1bc3c8aa231eb.js","512","static/chunks/4b89641d-a80e6024cd2468dc.js","354","static/chunks/354-d94f5f7615bdde2d.js","931","static/chunks/app/page-2e986eecfb9156dd.js"],""]
 1:[null,["$","html",null,{"lang":"en","children":["$","body",null,{"suppressHydrationWarning":true,"children":["$","$L4",null,{"parallelRouterKey":"children","segmentPath":["children"],"loading":"$undefined","loadingStyles":"$undefined","loadingScripts":"$undefined","hasLoading":false,"error":"$undefined","errorStyles":"$undefined","errorScripts":"$undefined","template":["$","$L5",null,{}],"templateStyles":"$undefined","templateScripts":"$undefined","notFound":[["$","title",null,{"children":"404: This page could not be found."}],["$","div",null,{"style":{"fontFamily":"system-ui,\"Segoe UI\",Roboto,Helvetica,Arial,sans-serif,\"Apple Color Emoji\",\"Segoe UI Emoji\"","height":"100vh","textAlign":"center","display":"flex","flexDirection":"column","alignItems":"center","justifyContent":"center"},"children":["$","div",null,{"children":[["$","style",null,{"dangerouslySetInnerHTML":{"__html":"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}"}}],["$","h1",null,{"className":"next-error-h1","style":{"display":"inline-block","margin":"0 20px 0 0","padding":"0 23px 0 0","fontSize":24,"fontWeight":500,"verticalAlign":"top","lineHeight":"49px"},"children":"404"}],["$","div",null,{"style":{"display":"inline-block"},"children":["$","h2",null,{"style":{"fontSize":14,"fontWeight":400,"lineHeight":"49px","margin":0},"children":"This page could not be found."}]}]]}]}]],"notFoundStyles":[],"childProp":{"current":["$L6",["$","$L7",null,{"propsForComponent":{"params":{}},"Component":"$8","isStaticGeneration":true}],null],"segment":"__PAGE__"},"styles":[["$","link","0",{"rel":"stylesheet","href":"/_next/static/css/6d0611c21a82d0bb.css","precedence":"next","crossOrigin":""}]]}]}]}],null]
 2:[["$","meta","0",{"name":"viewport","content":"width=device-width, initial-scale=1"}],["$","meta","1",{"charSet":"utf-8"}],["$","title","2",{"children":"recce"}],["$","meta","3",{"name":"description","content":"Recce: a dbt tool"}],["$","link","4",{"rel":"icon","href":"/favicon.ico","type":"image/x-icon","sizes":"16x16"}]]
 6:null
```

### Comparing `recce-nightly-0.9.0.20240312/recce/dbt.py` & `recce-nightly-0.9.0.20240313/recce/dbt.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/diff.py` & `recce-nightly-0.9.0.20240313/recce/diff.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/event/__init__.py` & `recce-nightly-0.9.0.20240313/recce/event/__init__.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/event/collector.py` & `recce-nightly-0.9.0.20240313/recce/event/collector.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/event/track.py` & `recce-nightly-0.9.0.20240313/recce/event/track.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/models/check.py` & `recce-nightly-0.9.0.20240313/recce/models/check.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/models/run.py` & `recce-nightly-0.9.0.20240313/recce/models/run.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/models/state.py` & `recce-nightly-0.9.0.20240313/recce/models/state.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/models/types.py` & `recce-nightly-0.9.0.20240313/recce/models/types.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/server.py` & `recce-nightly-0.9.0.20240313/recce/server.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/tasks/core.py` & `recce-nightly-0.9.0.20240313/recce/tasks/core.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/tasks/dataframe.py` & `recce-nightly-0.9.0.20240313/recce/tasks/dataframe.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/tasks/histogram.py` & `recce-nightly-0.9.0.20240313/recce/tasks/histogram.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/tasks/profile.py` & `recce-nightly-0.9.0.20240313/recce/tasks/profile.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/tasks/query.py` & `recce-nightly-0.9.0.20240313/recce/tasks/query.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/tasks/rowcount.py` & `recce-nightly-0.9.0.20240313/recce/tasks/rowcount.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/tasks/top_k.py` & `recce-nightly-0.9.0.20240313/recce/tasks/top_k.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/tasks/valuediff.py` & `recce-nightly-0.9.0.20240313/recce/tasks/valuediff.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/util/cache.py` & `recce-nightly-0.9.0.20240313/recce/util/cache.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce/yaml/__init__.py` & `recce-nightly-0.9.0.20240313/recce/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/recce_nightly.egg-info/PKG-INFO` & `recce-nightly-0.9.0.20240313/recce_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recce-nightly
-Version: 0.9.0.20240312
+Version: 0.9.0.20240313
 Summary: Environment diff tool for dbt
 Home-page: https://github.com/InfuseAI/recce
 Author: InfuseAI Dev Team
 Author-email: dev@infuseai.io
 Project-URL: Bug Tracker, https://github.com/InfuseAI/recce/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `recce-nightly-0.9.0.20240312/recce_nightly.egg-info/SOURCES.txt` & `recce-nightly-0.9.0.20240313/recce_nightly.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 recce/apis/check_func.py
 recce/apis/run_api.py
 recce/apis/run_func.py
 recce/data/404.html
 recce/data/favicon.ico
 recce/data/index.html
 recce/data/index.txt
-recce/data/_next/static/OSDAXs6UrZSM40dV34eY3/_buildManifest.js
-recce/data/_next/static/OSDAXs6UrZSM40dV34eY3/_ssgManifest.js
 recce/data/_next/static/chunks/030e0bea-59754f62ad2a287c.js
 recce/data/_next/static/chunks/2d02f0f7-ed3b4e4daa7c5d22.js
 recce/data/_next/static/chunks/354-d94f5f7615bdde2d.js
 recce/data/_next/static/chunks/49348413-7aacf235ca16afb9.js
 recce/data/_next/static/chunks/4b89641d-a80e6024cd2468dc.js
 recce/data/_next/static/chunks/526a6206-7ccbd30e159c1652.js
 recce/data/_next/static/chunks/5e9a126f-da62af62011c0643.js
@@ -39,18 +37,20 @@
 recce/data/_next/static/chunks/framework-f780fd9bae3b8c58.js
 recce/data/_next/static/chunks/main-01494d5774218692.js
 recce/data/_next/static/chunks/main-app-3297e27de57b3a96.js
 recce/data/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
 recce/data/_next/static/chunks/webpack-2d4823656eaa7d1c.js
 recce/data/_next/static/chunks/app/_not-found-51ab6491960b0490.js
 recce/data/_next/static/chunks/app/layout-c159ba5715e8f184.js
-recce/data/_next/static/chunks/app/page-11d757976ef71345.js
+recce/data/_next/static/chunks/app/page-2e986eecfb9156dd.js
 recce/data/_next/static/chunks/pages/_app-97b950e56cb06d37.js
 recce/data/_next/static/chunks/pages/_error-53b6bd498e76608f.js
 recce/data/_next/static/css/6d0611c21a82d0bb.css
+recce/data/_next/static/k9hThvy5xnFYnWlSYKB0A/_buildManifest.js
+recce/data/_next/static/k9hThvy5xnFYnWlSYKB0A/_ssgManifest.js
 recce/event/CONFIG
 recce/event/SENTRY_DNS
 recce/event/__init__.py
 recce/event/collector.py
 recce/event/track.py
 recce/models/__init__.py
 recce/models/check.py
```

### Comparing `recce-nightly-0.9.0.20240312/setup.py` & `recce-nightly-0.9.0.20240313/setup.py`

 * *Files identical despite different names*

### Comparing `recce-nightly-0.9.0.20240312/tests/test_dbt.py` & `recce-nightly-0.9.0.20240313/tests/test_dbt.py`

 * *Files identical despite different names*


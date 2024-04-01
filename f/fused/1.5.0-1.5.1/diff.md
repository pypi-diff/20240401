# Comparing `tmp/fused-1.5.0.tar.gz` & `tmp/fused-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fused-1.5.0.tar", max compression
+gzip compressed data, was "fused-1.5.1.tar", max compression
```

## Comparing `fused-1.5.0.tar` & `fused-1.5.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0     1144 2024-03-14 18:20:20.452694 fused-1.5.0/README.md
--rw-r--r--   0        0        0        6 2023-10-13 17:39:24.936083 fused-1.5.0/fused/MIGRATION_VERSION
--rw-r--r--   0        0        0     1111 2024-03-25 21:04:32.932521 fused-1.5.0/fused/__init__.py
--rw-r--r--   0        0        0       66 2023-08-29 21:43:53.192271 fused-1.5.0/fused/__main__.py
--rw-r--r--   0        0        0    10367 2024-03-01 23:09:39.488200 fused-1.5.0/fused/_auth.py
--rw-r--r--   0        0        0       66 2023-10-13 17:39:24.936596 fused-1.5.0/fused/_cache/__init__.py
--rw-r--r--   0        0        0     1401 2023-10-13 17:39:24.936653 fused-1.5.0/fused/_cache/memory.py
--rw-r--r--   0        0        0       77 2023-10-13 17:39:24.936726 fused-1.5.0/fused/_constants.py
--rw-r--r--   0        0        0     4181 2023-10-13 17:39:24.936791 fused-1.5.0/fused/_deserialize.py
--rw-r--r--   0        0        0      287 2023-10-13 17:39:24.937361 fused-1.5.0/fused/_deserialize_parquet.py
--rw-r--r--   0        0        0     2504 2023-10-13 17:39:24.937551 fused-1.5.0/fused/_environment.py
--rw-r--r--   0        0        0      357 2024-02-29 19:31:09.757442 fused-1.5.0/fused/_experimental.py
--rw-r--r--   0        0        0     2364 2024-02-29 19:31:09.757801 fused-1.5.0/fused/_formatter/common.py
--rw-r--r--   0        0        0    14878 2024-02-27 23:12:15.998414 fused-1.5.0/fused/_formatter/formatter_dataset.py
--rw-r--r--   0        0        0    11761 2024-01-03 19:21:18.331904 fused-1.5.0/fused/_formatter/formatter_eval_result.py
--rw-r--r--   0        0        0    16550 2023-10-13 20:24:00.322327 fused-1.5.0/fused/_formatter/formatter_job_config.py
--rw-r--r--   0        0        0     6962 2024-02-27 23:12:15.998885 fused-1.5.0/fused/_formatter/formatter_jobs.py
--rw-r--r--   0        0        0     2020 2023-10-13 17:39:24.939257 fused-1.5.0/fused/_formatter/formatter_options.py
--rw-r--r--   0        0        0     7031 2023-10-13 17:39:24.939757 fused-1.5.0/fused/_formatter/formatter_project.py
--rw-r--r--   0        0        0     1939 2024-02-29 19:31:09.758102 fused-1.5.0/fused/_formatter/formatter_templates.py
--rw-r--r--   0        0        0     5370 2024-02-16 20:07:37.387760 fused-1.5.0/fused/_formatter/formatter_udf_access_token.py
--rw-r--r--   0        0        0     1013 2023-10-13 17:39:24.940039 fused-1.5.0/fused/_formatter/noraise.py
--rw-r--r--   0        0        0     5379 2024-02-29 19:31:09.758573 fused-1.5.0/fused/_formatter/template.py
--rw-r--r--   0        0        0    11611 2024-02-07 21:35:13.328473 fused-1.5.0/fused/_formatter/udf.py
--rw-r--r--   0        0        0      905 2023-10-13 17:39:24.940709 fused-1.5.0/fused/_global_api.py
--rw-r--r--   0        0        0     2785 2024-03-04 19:13:44.140834 fused-1.5.0/fused/_load_udf.py
--rw-r--r--   0        0        0      721 2023-10-13 17:39:24.940878 fused-1.5.0/fused/_magic/__init__.py
--rw-r--r--   0        0        0     2853 2024-02-27 23:12:15.999392 fused-1.5.0/fused/_magic/magics.py
--rw-r--r--   0        0        0      608 2023-10-13 17:39:24.941393 fused-1.5.0/fused/_magic/output.py
--rw-r--r--   0        0        0     7779 2024-03-11 21:21:34.934302 fused-1.5.0/fused/_options.py
--rw-r--r--   0        0        0    39510 2024-03-25 21:04:06.812548 fused-1.5.0/fused/_project.py
--rw-r--r--   0        0        0    32872 2024-03-25 21:04:06.813201 fused-1.5.0/fused/_public_api.py
--rw-r--r--   0        0        0       40 2024-02-29 19:31:09.759028 fused-1.5.0/fused/_quick/__init__.py
--rw-r--r--   0        0        0    16830 2024-03-04 22:08:50.310839 fused-1.5.0/fused/_quick/udf.py
--rw-r--r--   0        0        0      118 2024-02-29 19:31:09.759558 fused-1.5.0/fused/_raster/__init__.py
--rw-r--r--   0        0        0     1431 2024-02-29 19:31:09.759769 fused-1.5.0/fused/_raster/signer.py
--rw-r--r--   0        0        0     4213 2024-02-29 19:31:09.759965 fused-1.5.0/fused/_raster/stac.py
--rw-r--r--   0        0        0     1015 2023-10-13 17:39:24.943010 fused-1.5.0/fused/_registry.py
--rw-r--r--   0        0        0      995 2023-10-13 17:39:24.943187 fused-1.5.0/fused/_request.py
--rw-r--r--   0        0        0    13366 2024-03-25 21:04:06.813505 fused-1.5.0/fused/_run.py
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.759996 fused-1.5.0/fused/_static/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.760075 fused-1.5.0/fused/_static/css/__init__.py
--rw-r--r--   0        0        0     7272 2024-02-29 19:31:09.762187 fused-1.5.0/fused/_static/css/style.css
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762251 fused-1.5.0/fused/_static/html/__init__.py
--rw-r--r--   0        0        0     3891 2024-02-29 19:31:09.762366 fused-1.5.0/fused/_static/html/icons-svg-inline.html
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762441 fused-1.5.0/fused/_static/templates/__init__.py
--rw-r--r--   0        0        0     1495 2023-10-18 19:12:32.880479 fused-1.5.0/fused/_str_utils.py
--rw-r--r--   0        0        0      176 2024-02-29 19:31:09.762566 fused-1.5.0/fused/_templates/__init__.py
--rw-r--r--   0        0        0      396 2024-02-29 19:31:09.762690 fused-1.5.0/fused/_templates/loaders.py
--rw-r--r--   0        0        0    15844 2024-02-29 19:31:09.763050 fused-1.5.0/fused/_templates/templates.py
--rw-r--r--   0        0        0      126 2023-10-13 17:39:24.943664 fused-1.5.0/fused/_udf/__init__.py
--rw-r--r--   0        0        0     1522 2023-10-13 17:39:24.943754 fused-1.5.0/fused/_udf/coerce.py
--rw-r--r--   0        0        0      790 2023-10-13 17:39:24.943812 fused-1.5.0/fused/_udf/context.py
--rw-r--r--   0        0        0     9116 2024-03-04 19:13:44.145677 fused-1.5.0/fused/_udf/decorators.py
--rw-r--r--   0        0        0     9049 2024-03-04 17:12:17.771016 fused-1.5.0/fused/_udf/execute_v2.py
--rw-r--r--   0        0        0    14851 2024-02-08 00:33:54.700810 fused-1.5.0/fused/_udf/load.py
--rw-r--r--   0        0        0      225 2023-10-13 17:39:24.944631 fused-1.5.0/fused/_udf/noop_decorators.py
--rw-r--r--   0        0        0      659 2023-10-13 17:39:24.944746 fused-1.5.0/fused/_udf/state.py
--rw-r--r--   0        0        0     3145 2024-03-25 21:04:06.814168 fused-1.5.0/fused/_utils.py
--rw-r--r--   0        0        0      404 2024-02-27 23:12:16.001476 fused-1.5.0/fused/api/__init__.py
--rw-r--r--   0        0        0      975 2023-10-13 17:39:24.945994 fused-1.5.0/fused/api/_open_dataset.py
--rw-r--r--   0        0        0     3586 2023-10-13 17:39:24.946052 fused-1.5.0/fused/api/_public_api.py
--rw-r--r--   0        0        0    48799 2024-03-25 21:04:06.815296 fused-1.5.0/fused/api/api.py
--rw-r--r--   0        0        0     3363 2024-03-11 21:21:34.935322 fused-1.5.0/fused/api/credentials.py
--rw-r--r--   0        0        0    25923 2024-03-25 21:04:06.816158 fused-1.5.0/fused/api/docker_api.py
--rw-r--r--   0        0        0    16521 2024-03-25 21:04:06.816775 fused-1.5.0/fused/api/docker_http_api.py
--rw-r--r--   0        0        0      290 2024-02-27 23:12:16.002737 fused-1.5.0/fused/cli.py
--rw-r--r--   0        0        0      492 2024-03-04 16:53:04.882953 fused-1.5.0/fused/core/__init__.py
--rw-r--r--   0        0        0    10226 2024-03-25 21:04:06.817593 fused-1.5.0/fused/core/_cache.py
--rw-r--r--   0        0        0     6484 2024-03-25 21:04:06.818258 fused-1.5.0/fused/core/_download.py
--rw-r--r--   0        0        0      509 2024-03-01 23:09:39.489541 fused-1.5.0/fused/core/_impl/_context_impl.py
--rw-r--r--   0        0        0     2995 2024-02-27 23:12:16.003344 fused-1.5.0/fused/core/_impl/_download_impl.py
--rw-r--r--   0        0        0     1022 2024-03-02 00:21:59.447576 fused-1.5.0/fused/core/_impl/_realtime_ops_impl.py
--rw-r--r--   0        0        0      254 2024-03-04 16:53:04.883231 fused-1.5.0/fused/core/_impl/_reimports.py
--rw-r--r--   0        0        0     2427 2024-03-14 21:19:20.148282 fused-1.5.0/fused/core/_impl/_table_ops_impl.py
--rw-r--r--   0        0        0     1369 2024-03-04 16:53:04.883573 fused-1.5.0/fused/core/_impl/_udf_ops_impl.py
--rw-r--r--   0        0        0    23387 2024-03-01 23:09:39.489874 fused-1.5.0/fused/core/_realtime_ops.py
--rw-r--r--   0        0        0     1086 2024-02-27 23:12:16.004574 fused-1.5.0/fused/core/_table_ops.py
--rw-r--r--   0        0        0     1767 2024-03-04 16:53:04.883828 fused-1.5.0/fused/core/_udf_ops.py
--rw-r--r--   0        0        0      795 2024-02-16 20:07:37.390060 fused-1.5.0/fused/models/__init__.py
--rw-r--r--   0        0        0      298 2023-10-13 17:39:24.948177 fused-1.5.0/fused/models/_codegen/__init__.py
--rw-r--r--   0        0        0     4861 2024-03-04 02:10:26.519019 fused-1.5.0/fused/models/_codegen/job.py
--rw-r--r--   0        0        0     4280 2024-02-08 00:33:54.701166 fused-1.5.0/fused/models/_codegen/udf.py
--rw-r--r--   0        0        0      224 2023-10-13 17:39:24.948705 fused-1.5.0/fused/models/_inplace.py
--rw-r--r--   0        0        0      250 2023-10-13 17:39:24.948775 fused-1.5.0/fused/models/_project_aware.py
--rw-r--r--   0        0        0      506 2024-02-16 20:07:37.390698 fused-1.5.0/fused/models/api/__init__.py
--rw-r--r--   0        0        0      221 2023-10-13 17:39:24.949226 fused-1.5.0/fused/models/api/_folder.py
--rw-r--r--   0        0        0    34461 2024-03-25 21:04:06.818813 fused-1.5.0/fused/models/api/dataset.py
--rw-r--r--   0        0        0       89 2023-05-12 15:11:04.143892 fused-1.5.0/fused/models/api/enums.py
--rw-r--r--   0        0        0    77407 2024-03-04 17:12:17.771506 fused-1.5.0/fused/models/api/job.py
--rw-r--r--   0        0        0     3235 2024-02-16 20:07:37.391066 fused-1.5.0/fused/models/api/udf_access_token.py
--rw-r--r--   0        0        0     3135 2023-10-13 17:39:24.950268 fused-1.5.0/fused/models/base.py
--rw-r--r--   0        0        0     1616 2024-03-04 16:53:04.884210 fused-1.5.0/fused/models/coerce_dataset.py
--rw-r--r--   0        0        0     3223 2024-02-08 20:07:13.852325 fused-1.5.0/fused/models/input.py
--rw-r--r--   0        0        0      330 2023-10-13 17:39:24.950681 fused-1.5.0/fused/models/internal/__init__.py
--rw-r--r--   0        0        0     8519 2023-10-13 17:39:24.951254 fused-1.5.0/fused/models/internal/dataset.py
--rw-r--r--   0        0        0    12158 2023-11-01 00:31:41.970766 fused-1.5.0/fused/models/internal/job.py
--rw-r--r--   0        0        0     1434 2023-10-13 17:39:24.952019 fused-1.5.0/fused/models/migrations.py
--rw-r--r--   0        0        0     5221 2024-02-16 20:07:37.391813 fused-1.5.0/fused/models/request.py
--rw-r--r--   0        0        0    29988 2024-03-25 21:04:06.819025 fused-1.5.0/fused/models/schema.py
--rw-r--r--   0        0        0      241 2023-10-13 17:39:24.953204 fused-1.5.0/fused/models/udf/__init__.py
--rw-r--r--   0        0        0     1432 2024-01-03 19:21:18.332999 fused-1.5.0/fused/models/udf/_eval_result.py
--rw-r--r--   0        0        0     8835 2024-03-04 16:53:21.723025 fused-1.5.0/fused/models/udf/_specialized_udfs.py
--rw-r--r--   0        0        0      781 2023-10-13 17:39:24.953888 fused-1.5.0/fused/models/udf/_udf_registry.py
--rw-r--r--   0        0        0    13495 2024-03-04 16:53:04.884708 fused-1.5.0/fused/models/udf/base_udf.py
--rw-r--r--   0        0        0     5358 2023-10-27 22:44:48.239852 fused-1.5.0/fused/models/udf/common.py
--rw-r--r--   0        0        0     5828 2024-02-12 23:41:47.582533 fused-1.5.0/fused/models/udf/header.py
--rw-r--r--   0        0        0     5564 2023-12-11 22:59:41.284263 fused-1.5.0/fused/models/udf/output.py
--rw-r--r--   0        0        0     3580 2024-03-04 17:12:17.771844 fused-1.5.0/fused/models/udf/udf.py
--rw-r--r--   0        0        0     1575 2023-10-13 17:39:24.955946 fused-1.5.0/fused/models/urls.py
--rw-r--r--   0        0        0     7940 2023-10-13 17:39:24.956442 fused-1.5.0/fused/models/viz.py
--rw-r--r--   0        0        0      671 2023-10-13 17:39:24.956576 fused-1.5.0/fused/models/viz_colors.py
--rw-r--r--   0        0        0     1126 2023-10-13 17:39:24.956677 fused-1.5.0/fused/models/viz_presets.py
--rw-r--r--   0        0        0      254 2024-03-11 20:54:28.030281 fused-1.5.0/fused/types.py
--rw-r--r--   0        0        0      675 2023-10-13 17:39:24.961379 fused-1.5.0/fused/warnings.py
--rw-r--r--   0        0        0     3111 2024-03-25 21:04:32.928247 fused-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 fused-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1144 2024-03-14 18:20:20.452694 fused-1.5.1/README.md
+-rw-r--r--   0        0        0        6 2023-10-13 17:39:24.936083 fused-1.5.1/fused/MIGRATION_VERSION
+-rw-r--r--   0        0        0     1111 2024-04-01 21:41:26.260985 fused-1.5.1/fused/__init__.py
+-rw-r--r--   0        0        0       66 2023-08-29 21:43:53.192271 fused-1.5.1/fused/__main__.py
+-rw-r--r--   0        0        0    10367 2024-03-01 23:09:39.488200 fused-1.5.1/fused/_auth.py
+-rw-r--r--   0        0        0       66 2023-10-13 17:39:24.936596 fused-1.5.1/fused/_cache/__init__.py
+-rw-r--r--   0        0        0     1401 2023-10-13 17:39:24.936653 fused-1.5.1/fused/_cache/memory.py
+-rw-r--r--   0        0        0       77 2023-10-13 17:39:24.936726 fused-1.5.1/fused/_constants.py
+-rw-r--r--   0        0        0     4181 2023-10-13 17:39:24.936791 fused-1.5.1/fused/_deserialize.py
+-rw-r--r--   0        0        0      287 2023-10-13 17:39:24.937361 fused-1.5.1/fused/_deserialize_parquet.py
+-rw-r--r--   0        0        0     2504 2023-10-13 17:39:24.937551 fused-1.5.1/fused/_environment.py
+-rw-r--r--   0        0        0      357 2024-02-29 19:31:09.757442 fused-1.5.1/fused/_experimental.py
+-rw-r--r--   0        0        0     2364 2024-02-29 19:31:09.757801 fused-1.5.1/fused/_formatter/common.py
+-rw-r--r--   0        0        0    14878 2024-02-27 23:12:15.998414 fused-1.5.1/fused/_formatter/formatter_dataset.py
+-rw-r--r--   0        0        0    11761 2024-01-03 19:21:18.331904 fused-1.5.1/fused/_formatter/formatter_eval_result.py
+-rw-r--r--   0        0        0    16550 2023-10-13 20:24:00.322327 fused-1.5.1/fused/_formatter/formatter_job_config.py
+-rw-r--r--   0        0        0     6962 2024-02-27 23:12:15.998885 fused-1.5.1/fused/_formatter/formatter_jobs.py
+-rw-r--r--   0        0        0     2020 2023-10-13 17:39:24.939257 fused-1.5.1/fused/_formatter/formatter_options.py
+-rw-r--r--   0        0        0     7031 2023-10-13 17:39:24.939757 fused-1.5.1/fused/_formatter/formatter_project.py
+-rw-r--r--   0        0        0     1939 2024-02-29 19:31:09.758102 fused-1.5.1/fused/_formatter/formatter_templates.py
+-rw-r--r--   0        0        0     5370 2024-02-16 20:07:37.387760 fused-1.5.1/fused/_formatter/formatter_udf_access_token.py
+-rw-r--r--   0        0        0     1013 2023-10-13 17:39:24.940039 fused-1.5.1/fused/_formatter/noraise.py
+-rw-r--r--   0        0        0     5379 2024-02-29 19:31:09.758573 fused-1.5.1/fused/_formatter/template.py
+-rw-r--r--   0        0        0    11611 2024-02-07 21:35:13.328473 fused-1.5.1/fused/_formatter/udf.py
+-rw-r--r--   0        0        0      905 2023-10-13 17:39:24.940709 fused-1.5.1/fused/_global_api.py
+-rw-r--r--   0        0        0     2752 2024-04-01 21:12:17.245535 fused-1.5.1/fused/_load_udf.py
+-rw-r--r--   0        0        0      721 2023-10-13 17:39:24.940878 fused-1.5.1/fused/_magic/__init__.py
+-rw-r--r--   0        0        0     2853 2024-02-27 23:12:15.999392 fused-1.5.1/fused/_magic/magics.py
+-rw-r--r--   0        0        0      608 2023-10-13 17:39:24.941393 fused-1.5.1/fused/_magic/output.py
+-rw-r--r--   0        0        0     7783 2024-04-01 21:12:17.246431 fused-1.5.1/fused/_options.py
+-rw-r--r--   0        0        0    39426 2024-04-01 21:12:17.247134 fused-1.5.1/fused/_project.py
+-rw-r--r--   0        0        0    32913 2024-04-01 21:12:17.247928 fused-1.5.1/fused/_public_api.py
+-rw-r--r--   0        0        0       40 2024-02-29 19:31:09.759028 fused-1.5.1/fused/_quick/__init__.py
+-rw-r--r--   0        0        0    16830 2024-03-04 22:08:50.310839 fused-1.5.1/fused/_quick/udf.py
+-rw-r--r--   0        0        0      118 2024-02-29 19:31:09.759558 fused-1.5.1/fused/_raster/__init__.py
+-rw-r--r--   0        0        0     1431 2024-02-29 19:31:09.759769 fused-1.5.1/fused/_raster/signer.py
+-rw-r--r--   0        0        0     4213 2024-02-29 19:31:09.759965 fused-1.5.1/fused/_raster/stac.py
+-rw-r--r--   0        0        0     1015 2023-10-13 17:39:24.943010 fused-1.5.1/fused/_registry.py
+-rw-r--r--   0        0        0      995 2023-10-13 17:39:24.943187 fused-1.5.1/fused/_request.py
+-rw-r--r--   0        0        0    13798 2024-04-01 21:12:17.248121 fused-1.5.1/fused/_run.py
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.759996 fused-1.5.1/fused/_static/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.760075 fused-1.5.1/fused/_static/css/__init__.py
+-rw-r--r--   0        0        0     7272 2024-02-29 19:31:09.762187 fused-1.5.1/fused/_static/css/style.css
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762251 fused-1.5.1/fused/_static/html/__init__.py
+-rw-r--r--   0        0        0     3891 2024-02-29 19:31:09.762366 fused-1.5.1/fused/_static/html/icons-svg-inline.html
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762441 fused-1.5.1/fused/_static/templates/__init__.py
+-rw-r--r--   0        0        0     1495 2023-10-18 19:12:32.880479 fused-1.5.1/fused/_str_utils.py
+-rw-r--r--   0        0        0      176 2024-02-29 19:31:09.762566 fused-1.5.1/fused/_templates/__init__.py
+-rw-r--r--   0        0        0      396 2024-02-29 19:31:09.762690 fused-1.5.1/fused/_templates/loaders.py
+-rw-r--r--   0        0        0    15844 2024-02-29 19:31:09.763050 fused-1.5.1/fused/_templates/templates.py
+-rw-r--r--   0        0        0      126 2023-10-13 17:39:24.943664 fused-1.5.1/fused/_udf/__init__.py
+-rw-r--r--   0        0        0     1522 2023-10-13 17:39:24.943754 fused-1.5.1/fused/_udf/coerce.py
+-rw-r--r--   0        0        0      790 2023-10-13 17:39:24.943812 fused-1.5.1/fused/_udf/context.py
+-rw-r--r--   0        0        0     9116 2024-03-04 19:13:44.145677 fused-1.5.1/fused/_udf/decorators.py
+-rw-r--r--   0        0        0     9049 2024-03-04 17:12:17.771016 fused-1.5.1/fused/_udf/execute_v2.py
+-rw-r--r--   0        0        0    14851 2024-02-08 00:33:54.700810 fused-1.5.1/fused/_udf/load.py
+-rw-r--r--   0        0        0      225 2023-10-13 17:39:24.944631 fused-1.5.1/fused/_udf/noop_decorators.py
+-rw-r--r--   0        0        0      659 2023-10-13 17:39:24.944746 fused-1.5.1/fused/_udf/state.py
+-rw-r--r--   0        0        0     3202 2024-04-01 21:12:17.248259 fused-1.5.1/fused/_utils.py
+-rw-r--r--   0        0        0      404 2024-02-27 23:12:16.001476 fused-1.5.1/fused/api/__init__.py
+-rw-r--r--   0        0        0      975 2023-10-13 17:39:24.945994 fused-1.5.1/fused/api/_open_dataset.py
+-rw-r--r--   0        0        0     3586 2023-10-13 17:39:24.946052 fused-1.5.1/fused/api/_public_api.py
+-rw-r--r--   0        0        0    48807 2024-04-01 21:12:17.248568 fused-1.5.1/fused/api/api.py
+-rw-r--r--   0        0        0     3363 2024-03-11 21:21:34.935322 fused-1.5.1/fused/api/credentials.py
+-rw-r--r--   0        0        0    25931 2024-04-01 21:12:17.249314 fused-1.5.1/fused/api/docker_api.py
+-rw-r--r--   0        0        0    16529 2024-04-01 21:12:17.249955 fused-1.5.1/fused/api/docker_http_api.py
+-rw-r--r--   0        0        0      290 2024-02-27 23:12:16.002737 fused-1.5.1/fused/cli.py
+-rw-r--r--   0        0        0      492 2024-03-04 16:53:04.882953 fused-1.5.1/fused/core/__init__.py
+-rw-r--r--   0        0        0    10279 2024-04-01 21:12:17.250418 fused-1.5.1/fused/core/_cache.py
+-rw-r--r--   0        0        0     6513 2024-04-01 21:12:17.250608 fused-1.5.1/fused/core/_download.py
+-rw-r--r--   0        0        0      509 2024-03-01 23:09:39.489541 fused-1.5.1/fused/core/_impl/_context_impl.py
+-rw-r--r--   0        0        0     2995 2024-02-27 23:12:16.003344 fused-1.5.1/fused/core/_impl/_download_impl.py
+-rw-r--r--   0        0        0     1022 2024-03-02 00:21:59.447576 fused-1.5.1/fused/core/_impl/_realtime_ops_impl.py
+-rw-r--r--   0        0        0      254 2024-03-04 16:53:04.883231 fused-1.5.1/fused/core/_impl/_reimports.py
+-rw-r--r--   0        0        0     2427 2024-03-14 21:19:20.148282 fused-1.5.1/fused/core/_impl/_table_ops_impl.py
+-rw-r--r--   0        0        0     1369 2024-03-04 16:53:04.883573 fused-1.5.1/fused/core/_impl/_udf_ops_impl.py
+-rw-r--r--   0        0        0    23387 2024-03-01 23:09:39.489874 fused-1.5.1/fused/core/_realtime_ops.py
+-rw-r--r--   0        0        0     1067 2024-04-01 21:12:17.251472 fused-1.5.1/fused/core/_table_ops.py
+-rw-r--r--   0        0        0     1767 2024-03-04 16:53:04.883828 fused-1.5.1/fused/core/_udf_ops.py
+-rw-r--r--   0        0        0      795 2024-02-16 20:07:37.390060 fused-1.5.1/fused/models/__init__.py
+-rw-r--r--   0        0        0      298 2023-10-13 17:39:24.948177 fused-1.5.1/fused/models/_codegen/__init__.py
+-rw-r--r--   0        0        0     4861 2024-03-04 02:10:26.519019 fused-1.5.1/fused/models/_codegen/job.py
+-rw-r--r--   0        0        0     4280 2024-02-08 00:33:54.701166 fused-1.5.1/fused/models/_codegen/udf.py
+-rw-r--r--   0        0        0      224 2023-10-13 17:39:24.948705 fused-1.5.1/fused/models/_inplace.py
+-rw-r--r--   0        0        0      250 2023-10-13 17:39:24.948775 fused-1.5.1/fused/models/_project_aware.py
+-rw-r--r--   0        0        0      506 2024-02-16 20:07:37.390698 fused-1.5.1/fused/models/api/__init__.py
+-rw-r--r--   0        0        0      221 2023-10-13 17:39:24.949226 fused-1.5.1/fused/models/api/_folder.py
+-rw-r--r--   0        0        0    34461 2024-03-25 21:04:06.818813 fused-1.5.1/fused/models/api/dataset.py
+-rw-r--r--   0        0        0       89 2023-05-12 15:11:04.143892 fused-1.5.1/fused/models/api/enums.py
+-rw-r--r--   0        0        0    77407 2024-03-04 17:12:17.771506 fused-1.5.1/fused/models/api/job.py
+-rw-r--r--   0        0        0     3235 2024-02-16 20:07:37.391066 fused-1.5.1/fused/models/api/udf_access_token.py
+-rw-r--r--   0        0        0     3135 2023-10-13 17:39:24.950268 fused-1.5.1/fused/models/base.py
+-rw-r--r--   0        0        0     1616 2024-03-04 16:53:04.884210 fused-1.5.1/fused/models/coerce_dataset.py
+-rw-r--r--   0        0        0     3223 2024-02-08 20:07:13.852325 fused-1.5.1/fused/models/input.py
+-rw-r--r--   0        0        0      330 2023-10-13 17:39:24.950681 fused-1.5.1/fused/models/internal/__init__.py
+-rw-r--r--   0        0        0     8519 2023-10-13 17:39:24.951254 fused-1.5.1/fused/models/internal/dataset.py
+-rw-r--r--   0        0        0    12158 2023-11-01 00:31:41.970766 fused-1.5.1/fused/models/internal/job.py
+-rw-r--r--   0        0        0     1434 2023-10-13 17:39:24.952019 fused-1.5.1/fused/models/migrations.py
+-rw-r--r--   0        0        0     5221 2024-02-16 20:07:37.391813 fused-1.5.1/fused/models/request.py
+-rw-r--r--   0        0        0    29988 2024-03-25 21:04:06.819025 fused-1.5.1/fused/models/schema.py
+-rw-r--r--   0        0        0      241 2023-10-13 17:39:24.953204 fused-1.5.1/fused/models/udf/__init__.py
+-rw-r--r--   0        0        0     1432 2024-01-03 19:21:18.332999 fused-1.5.1/fused/models/udf/_eval_result.py
+-rw-r--r--   0        0        0     8835 2024-03-04 16:53:21.723025 fused-1.5.1/fused/models/udf/_specialized_udfs.py
+-rw-r--r--   0        0        0      781 2023-10-13 17:39:24.953888 fused-1.5.1/fused/models/udf/_udf_registry.py
+-rw-r--r--   0        0        0    13495 2024-04-01 21:12:35.530426 fused-1.5.1/fused/models/udf/base_udf.py
+-rw-r--r--   0        0        0     5358 2023-10-27 22:44:48.239852 fused-1.5.1/fused/models/udf/common.py
+-rw-r--r--   0        0        0     5980 2024-04-01 21:12:17.251879 fused-1.5.1/fused/models/udf/header.py
+-rw-r--r--   0        0        0     5564 2023-12-11 22:59:41.284263 fused-1.5.1/fused/models/udf/output.py
+-rw-r--r--   0        0        0     3580 2024-03-04 17:12:17.771844 fused-1.5.1/fused/models/udf/udf.py
+-rw-r--r--   0        0        0     1575 2023-10-13 17:39:24.955946 fused-1.5.1/fused/models/urls.py
+-rw-r--r--   0        0        0     7940 2023-10-13 17:39:24.956442 fused-1.5.1/fused/models/viz.py
+-rw-r--r--   0        0        0      671 2023-10-13 17:39:24.956576 fused-1.5.1/fused/models/viz_colors.py
+-rw-r--r--   0        0        0     1126 2023-10-13 17:39:24.956677 fused-1.5.1/fused/models/viz_presets.py
+-rw-r--r--   0        0        0      254 2024-03-11 20:54:28.030281 fused-1.5.1/fused/types.py
+-rw-r--r--   0        0        0      675 2023-10-13 17:39:24.961379 fused-1.5.1/fused/warnings.py
+-rw-r--r--   0        0        0     3111 2024-04-01 21:41:26.254878 fused-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 fused-1.5.1/PKG-INFO
```

### Comparing `fused-1.5.0/README.md` & `fused-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/__init__.py` & `fused-1.5.1/fused/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 from .core import cache, download, get_chunk_from_table, get_chunks_metadata
 
 # Must be later so that models get imported first
 from . import _experimental as experimental  # isort:skip
 
 # Version is set to 0.0.0 as the version string is automatically generated by
 # https://github.com/mtkennerly/poetry-dynamic-versioning
-__version__ = "1.5.0"
+__version__ = "1.5.1"
```

### Comparing `fused-1.5.0/fused/_auth.py` & `fused-1.5.1/fused/_auth.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_cache/memory.py` & `fused-1.5.1/fused/_cache/memory.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_deserialize.py` & `fused-1.5.1/fused/_deserialize.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_environment.py` & `fused-1.5.1/fused/_environment.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_formatter/common.py` & `fused-1.5.1/fused/_formatter/common.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_formatter/formatter_dataset.py` & `fused-1.5.1/fused/_formatter/formatter_dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_formatter/formatter_eval_result.py` & `fused-1.5.1/fused/_formatter/formatter_eval_result.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_formatter/formatter_job_config.py` & `fused-1.5.1/fused/_formatter/formatter_job_config.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_formatter/formatter_jobs.py` & `fused-1.5.1/fused/_formatter/formatter_jobs.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_formatter/formatter_options.py` & `fused-1.5.1/fused/_formatter/formatter_options.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_formatter/formatter_project.py` & `fused-1.5.1/fused/_formatter/formatter_project.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_formatter/formatter_templates.py` & `fused-1.5.1/fused/_formatter/formatter_templates.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_formatter/formatter_udf_access_token.py` & `fused-1.5.1/fused/_formatter/formatter_udf_access_token.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_formatter/noraise.py` & `fused-1.5.1/fused/_formatter/noraise.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_formatter/template.py` & `fused-1.5.1/fused/_formatter/template.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_formatter/udf.py` & `fused-1.5.1/fused/_formatter/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_global_api.py` & `fused-1.5.1/fused/_global_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_load_udf.py` & `fused-1.5.1/fused/_load_udf.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from .core import load_udf_from_fused, load_udf_from_github
 from .core._impl._reimports import BaseUdf, load_job
 
 
 def load(url_or_udf: Union[str, Path], /, *, cache_key: Any = None) -> BaseUdf:
     """
-    Loads a UDF (User-Defined Function) from various sources including GitHub URLs,
+    Loads a UDF from various sources including GitHub URLs,
     local files, or directories, and a Fused platform-specific identifier.
 
     This function supports loading UDFs from a GitHub repository URL, a local file path,
     a directory containing UDF definitions, or a Fused platform-specific identifier
     composed of an email and UDF name. It intelligently determines the source type based
     on the format of the input and retrieves the UDF accordingly.
 
@@ -31,25 +31,25 @@
         FileNotFoundError: If a local file or directory path is provided but does not exist.
         ValueError: If the URL or Fused platform-specific identifier format is incorrect or
             cannot be parsed.
         Exception: For errors related to network issues, file access permissions, or other
             unforeseen errors during the loading process.
 
     Examples:
-        Loading a UDF from a GitHub URL:
+        Load a UDF from a GitHub URL:
         ```py
         udf = fused.load("https://github.com/fusedio/udfs/tree/main/public/REM_with_HyRiver/")
         ```
 
-        Loading a UDF from a local file:
+        Load a UDF from a local file:
         ```py
         udf = fused.load("/localpath/REM_with_HyRiver/")
         ```
 
-        Loading a UDF using a Fused platform-specific identifier:
+        Load a UDF using a Fused platform-specific identifier:
         ```py
         udf = fused.load("username@fused.io/REM_with_HyRiver")
         ```
     """
     maybe_path = Path(url_or_udf)
     if url_or_udf.startswith("https://github.com"):
         return load_udf_from_github(url_or_udf, cache_key=cache_key)
```

### Comparing `fused-1.5.0/fused/_magic/__init__.py` & `fused-1.5.1/fused/_magic/__init__.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_magic/magics.py` & `fused-1.5.1/fused/_magic/magics.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_magic/output.py` & `fused-1.5.1/fused/_magic/output.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_options.py` & `fused-1.5.1/fused/_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     Raises:
         AttributeError: If the specified attribute path is not valid, either because a part
                         of the path does not exist or the final attribute cannot be set with
                         the provided value.
 
     Examples:
         Set the `request_timeout` top-level option to 120 seconds:
-        ```py
+        ```python
         set_option('request_timeout', 120)
         ```
 
 
     """
     # Set a recursive option name
     # From https://stackoverflow.com/a/65355793 and comments
```

### Comparing `fused-1.5.0/fused/_project.py` & `fused-1.5.1/fused/_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,44 +330,34 @@
         gdal_config: Union[GDALOpenConfig, Dict[str, Any], None] = None,
     ) -> GeospatialPartitionJobStepConfig:
         """Ingest a dataset into the Fused partitioned format.
 
         Args:
             input: A GeoPandas `GeoDataFrame` or a path to file or files on S3 to ingest. Files may be Parquet or another geo data format.
             output: Location on S3 to write the `main` table to.
-
-        Keyword Args:
             output_metadata: Location on S3 to write the `fused` table to.
             schema: Schema of the data to be ingested. This is optional and will be inferred from the data if not provided.
             file_suffix: filter which files are used for ingestion. If `input` is a directory on S3, all files under that directory will be listed and used for ingestion. If `file_suffix` is not None, it will be used to filter paths by checking the trailing characters of each filename. E.g. pass `file_suffix=".geojson"` to include only GeoJSON files inside the directory.
             load_columns: Read only this set of columns when ingesting geospatial datasets. Defaults to all columns.
             remove_cols: The named columns to drop when ingesting geospatial datasets. Defaults to not drop any columns.
             explode_geometries: Whether to unpack multipart geometries to single geometries when ingesting geospatial datasets, saving each part as its own row. Defaults to `False`.
             drop_out_of_bounds: Whether to drop geometries outside of the expected WGS84 bounds. Defaults to True.
-            partitioning_method: The method to use for grouping rows into partitions.
-
+            partitioning_method: The method to use for grouping rows into partitions. Defaults to `"rows"`.
                 - `"area"`: Construct partitions where all contain a maximum total area among geometries.
                 - `"length"`: Construct partitions where all contain a maximum total length among geometries.
                 - `"coords"`: Construct partitions where all contain a maximum total number of coordinates among geometries.
                 - `"rows"`: Construct partitions where all contain a maximum number of rows.
-
-                Defaults to `"rows"`.
-
             partitioning_maximum_per_file: Maximum value for `partitioning_method` to use per file. If `None`, defaults to _1/10th_ of the total value of `partitioning_method`. So if the value is `None` and `partitioning_method` is `"area"`, then each file will be have no more than 1/10th the total area of all geometries. Defaults to `None`.
             partitioning_maximum_per_chunk: Maximum value for `partitioning_method` to use per chunk. If `None`, defaults to _1/100th_ of the total value of `partitioning_method`. So if the value is `None` and `partitioning_method` is `"area"`, then each file will be have no more than 1/100th the total area of all geometries. Defaults to `None`.
             partitioning_max_width_ratio: The maximum ratio of width to height of each partition to use in the ingestion process. So for example, if the value is `2`, then if the width divided by the height is greater than `2`, the box will be split in half along the horizontal axis. Defaults to `2`.
             partitioning_max_height_ratio: The maximum ratio of height to width of each partition to use in the ingestion process. So for example, if the value is `2`, then if the height divided by the width is greater than `2`, the box will be split in half along the vertical axis. Defaults to `2`.
             partitioning_force_utm: Whether to force partitioning within UTM zones. If set to `"file"`, this will ensure that the centroid of all geometries per _file_ are contained in the same UTM zone. If set to `"chunk"`, this will ensure that the centroid of all geometries per _chunk_ are contained in the same UTM zone. If set to `None`, then no UTM-based partitioning will be done. Defaults to "chunk".
-            partitioning_split_method: How to split one partition into children.
-
+            partitioning_split_method: How to split one partition into children. Defaults to `"mean"` (this may change in the future).
                 - `"mean"`: Split each axis according to the mean of the centroid values.
                 - `"median"`: Split each axis according to the median of the centroid values.
-
-                Defaults to `"mean"` (this may change in the future).
-
             subdivide_method: The method to use for subdividing large geometries into multiple rows. Currently the only option is `"area"`, where geometries will be subdivided based on their area (in WGS84 degrees).
             subdivide_start: The value above which geometries will be subdivided into smaller parts, according to `subdivide_method`.
             subdivide_stop: The value below which geometries will never be subdivided into smaller parts, according to `subdivide_method`.
             split_identical_centroids: If `True`, should split a partition that has
                 identical centroids (such as if all geometries in the partition are the
                 same) if there are more such rows than defined in "partitioning_maximum_per_file" and
                 "partitioning_maximum_per_chunk".
@@ -466,16 +456,14 @@
         partitioning_maximum_per_chunk: int = 65_000,
     ) -> NonGeospatialPartitionJobStepConfig:
         """Ingest a dataset into the Fused partitioned format.
 
         Args:
             input: A GeoPandas `GeoDataFrame` or a path to file or files on S3 to ingest. Files may be Parquet or another geo data format.
             output: Location on S3 to write the `main` table to.
-
-        Keyword Args:
             output_metadata: Location on S3 to write the `fused` table to.
             partition_col: Partition along this column for nongeospatial datasets.
             partitioning_maximum_per_file: Maximum number of items to store in a single file. Defaults to 2,500,000.
             partitioning_maximum_per_chunk: Maximum number of items to store in a single file. Defaults to 65,000.
 
         Returns:
```

### Comparing `fused-1.5.0/fused/_public_api.py` & `fused-1.5.1/fused/_public_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
     Returns:
         A list of UDFs.
 
     Examples:
         Fetch UDFs under the user account:
         ```py
-        get_udfs()
+        fused.get_udfs()
         ```
     """
     api = get_api()
     return api.get_udfs(
         n=n,
         skip=skip,
         per_request=per_request,
@@ -171,15 +171,14 @@
     Keyword Args:
         fetch_samples: If True, fetch sample on each table when getting dataset metadata.
     Returns:
         A Table object
 
     Examples:
         ```py
-        import fused
         table = fused.open_table("s3://my_bucket/path/to/dataset/table/")
         ```
     """
     if isinstance(path, DatasetOutputV2):
         path = path.url
 
     api = get_api()
@@ -216,44 +215,38 @@
     gdal_config: Union[GDALOpenConfig, Dict[str, Any], None] = None,
 ) -> GeospatialPartitionJobStepConfig:
     """Ingest a dataset into the Fused partitioned format.
 
     Args:
         input: A GeoPandas `GeoDataFrame` or a path to file or files on S3 to ingest. Files may be Parquet or another geo data format.
         output: Location on S3 to write the `main` table to.
-
-    Keyword Args:
         output_metadata: Location on S3 to write the `fused` table to.
         schema: Schema of the data to be ingested. This is optional and will be inferred from the data if not provided.
         file_suffix: filter which files are used for ingestion. If `input` is a directory on S3, all files under that directory will be listed and used for ingestion. If `file_suffix` is not None, it will be used to filter paths by checking the trailing characters of each filename. E.g. pass `file_suffix=".geojson"` to include only GeoJSON files inside the directory.
         load_columns: Read only this set of columns when ingesting geospatial datasets. Defaults to all columns.
         remove_cols: The named columns to drop when ingesting geospatial datasets. Defaults to not drop any columns.
         explode_geometries: Whether to unpack multipart geometries to single geometries when ingesting geospatial datasets, saving each part as its own row. Defaults to `False`.
         drop_out_of_bounds: Whether to drop geometries outside of the expected WGS84 bounds. Defaults to True.
-        partitioning_method: The method to use for grouping rows into partitions.
+        partitioning_method: The method to use for grouping rows into partitions. Defaults to `"rows"`.
 
             - `"area"`: Construct partitions where all contain a maximum total area among geometries.
             - `"length"`: Construct partitions where all contain a maximum total length among geometries.
             - `"coords"`: Construct partitions where all contain a maximum total number of coordinates among geometries.
             - `"rows"`: Construct partitions where all contain a maximum number of rows.
 
-            Defaults to `"rows"`.
-
         partitioning_maximum_per_file: Maximum value for `partitioning_method` to use per file. If `None`, defaults to _1/10th_ of the total value of `partitioning_method`. So if the value is `None` and `partitioning_method` is `"area"`, then each file will be have no more than 1/10th the total area of all geometries. Defaults to `None`.
         partitioning_maximum_per_chunk: Maximum value for `partitioning_method` to use per chunk. If `None`, defaults to _1/100th_ of the total value of `partitioning_method`. So if the value is `None` and `partitioning_method` is `"area"`, then each file will be have no more than 1/100th the total area of all geometries. Defaults to `None`.
         partitioning_max_width_ratio: The maximum ratio of width to height of each partition to use in the ingestion process. So for example, if the value is `2`, then if the width divided by the height is greater than `2`, the box will be split in half along the horizontal axis. Defaults to `2`.
         partitioning_max_height_ratio: The maximum ratio of height to width of each partition to use in the ingestion process. So for example, if the value is `2`, then if the height divided by the width is greater than `2`, the box will be split in half along the vertical axis. Defaults to `2`.
         partitioning_force_utm: Whether to force partitioning within UTM zones. If set to `"file"`, this will ensure that the centroid of all geometries per _file_ are contained in the same UTM zone. If set to `"chunk"`, this will ensure that the centroid of all geometries per _chunk_ are contained in the same UTM zone. If set to `None`, then no UTM-based partitioning will be done. Defaults to "chunk".
-        partitioning_split_method: How to split one partition into children.
+        partitioning_split_method: How to split one partition into children. Defaults to `"mean"` (this may change in the future).
 
             - `"mean"`: Split each axis according to the mean of the centroid values.
             - `"median"`: Split each axis according to the median of the centroid values.
 
-            Defaults to `"mean"` (this may change in the future).
-
         subdivide_method: The method to use for subdividing large geometries into multiple rows. Currently the only option is `"area"`, where geometries will be subdivided based on their area (in WGS84 degrees).
         subdivide_start: The value above which geometries will be subdivided into smaller parts, according to `subdivide_method`.
         subdivide_stop: The value below which geometries will never be subdivided into smaller parts, according to `subdivide_method`.
         split_identical_centroids: If `True`, should split a partition that has
             identical centroids (such as if all geometries in the partition are the
             same) if there are more such rows than defined in "partitioning_maximum_per_file" and
             "partitioning_maximum_per_chunk".
@@ -357,16 +350,14 @@
     partitioning_maximum_per_chunk: int = 65_000,
 ) -> NonGeospatialPartitionJobStepConfig:
     """Ingest a dataset into the Fused partitioned format.
 
     Args:
         input: A GeoPandas `GeoDataFrame` or a path to file or files on S3 to ingest. Files may be Parquet or another geo data format.
         output: Location on S3 to write the `main` table to.
-
-    Keyword Args:
         output_metadata: Location on S3 to write the `fused` table to.
         partition_col: Partition along this column for nongeospatial datasets.
         partitioning_maximum_per_file: Maximum number of items to store in a single file. Defaults to 2,500,000.
         partitioning_maximum_per_chunk: Maximum number of items to store in a single file. Defaults to 65,000.
 
     Returns:
 
@@ -590,16 +581,17 @@
         path: Directory or file to delete, like `fd://my-old-table/`
         max_deletion_depth: If set (defaults to 2), the maximum depth the operation will recurse to.
                             This option is to help avoid accidentally deleting more data that intended.
                             Pass `"unlimited"` for unlimited.
 
 
     Examples:
-
+        ```python
         fused.delete("fd://bucket-name/deprecated_table/")
+        ```
     """
     api = get_api()
     return api.delete(path, max_deletion_depth=max_deletion_depth)
 
 
 def list(path: str) -> List[str]:
     """List the files at the path.
@@ -607,16 +599,17 @@
     Args:
         path: Parent directory URL, like `fd://bucket-name/`
 
     Returns:
         A list of paths as URLs
 
     Examples:
-
+        ```python
         fused.list("fd://bucket-name/")
+        ```
     """
     api = get_api()
     return api.list(path)
 
 
 def get(path: str) -> bytes:
     """Download the contents at the path to memory.
@@ -624,16 +617,17 @@
     Args:
         path: URL to a file, like `fd://bucket-name/file.parquet`
 
     Returns:
         bytes of the file
 
     Examples:
-
+        ```python
         fused.get("fd://bucket-name/file.parquet")
+        ```
     """
     api = get_api()
     return api.get(path)
 
 
 def download(path: str, local_path: Union[str, Path]) -> None:
     """Download the contents at the path to disk.
@@ -684,16 +678,17 @@
     Args:
         path: URL to a file, like `fd://bucket-name/file.parquet`
 
     Returns:
         HTTPS URL to access the file using signed access.
 
     Examples:
-
+        ```python
         fused.sign_url("fd://bucket-name/table_directory/file.parquet")
+        ```
     """
     api = get_api()
     return api.sign_url(path)
 
 
 def sign_url_prefix(path: str) -> Dict[str, str]:
     """Create signed URLs to access all blobs under the path.
@@ -701,15 +696,15 @@
     Args:
         path: URL to a prefix, like `fd://bucket-name/some_directory/`
 
     Returns:
         Dictionary mapping from blob store key to signed HTTPS URL.
 
     Examples:
-        ```py
+        ```python
         fused.sign_url_prefix("fd://bucket-name/table_directory/")
         ```
     """
     api = get_api()
     return api.sign_url_prefix(path)
```

### Comparing `fused-1.5.0/fused/_quick/udf.py` & `fused-1.5.1/fused/_quick/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_raster/signer.py` & `fused-1.5.1/fused/_raster/signer.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_raster/stac.py` & `fused-1.5.1/fused/_raster/stac.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_registry.py` & `fused-1.5.1/fused/_registry.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_request.py` & `fused-1.5.1/fused/_request.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_run.py` & `fused-1.5.1/fused/_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import warnings
 from functools import partial
-from typing import Callable, Coroutine, Literal, Optional, Union, overload
+from typing import Any, Callable, Coroutine, Dict, Literal, Optional, Union, overload
 
 import geopandas as gpd
 import pandas as pd
 import shapely
 import xarray as xr
 
 from .core import (
@@ -32,21 +32,22 @@
     udf: Optional[GeoPandasUdfV2],
     job_step: Optional[UdfJobStepConfig],
     token: Optional[str],
     udf_email: Optional[str],
     x: Optional[int],
     y: Optional[int],
     z: Optional[int],
-    lat: Optional[float],
-    lng: Optional[float],
+    _lat: Optional[float],
+    _lng: Optional[float],
     bbox: Union[gpd.GeoDataFrame, shapely.Geometry, None],
     sync: bool = False,
     engine: Optional[Literal["realtime", "batch", "local"]],
     type: Optional[Literal["tile", "file"]],
-    **parameters,
+    parameters: Optional[Dict[str, Any]] = None,
+    **kw_parameters,
 ) -> Coroutine[ResultType, None, None]:
     ...
 
 
 @overload
 def run(
     email_or_udf_or_token: Union[str, None, UdfJobStepConfig, GeoPandasUdfV2],
@@ -56,21 +57,22 @@
     udf: Optional[GeoPandasUdfV2],
     job_step: Optional[UdfJobStepConfig],
     token: Optional[str],
     udf_email: Optional[str],
     x: Optional[int],
     y: Optional[int],
     z: Optional[int],
-    lat: Optional[float],
-    lng: Optional[float],
+    _lat: Optional[float],
+    _lng: Optional[float],
     bbox: Union[gpd.GeoDataFrame, shapely.Geometry, None],
     sync: bool,
     engine: Optional[Literal["realtime", "batch", "local"]],
     type: Optional[Literal["tile", "file"]],
-    **parameters,
+    parameters: Optional[Dict[str, Any]] = None,
+    **kw_parameters,
 ) -> ResultType:
     ...
 
 
 def run(
     email_or_udf_or_token: Union[str, None, UdfJobStepConfig, GeoPandasUdfV2] = None,
     /,
@@ -79,21 +81,22 @@
     udf: Optional[GeoPandasUdfV2] = None,
     job_step: Optional[UdfJobStepConfig] = None,
     token: Optional[str] = None,
     udf_email: Optional[str] = None,
     x: Optional[int] = None,
     y: Optional[int] = None,
     z: Optional[int] = None,
-    lat: Optional[float] = None,
-    lng: Optional[float] = None,
+    _lat: Optional[float] = None,
+    _lng: Optional[float] = None,
     bbox: Union[gpd.GeoDataFrame, shapely.Geometry, None] = None,
     sync: bool = True,
     engine: Optional[Literal["realtime", "batch", "local"]] = None,
     type: Optional[Literal["tile", "file"]] = None,
-    **parameters,
+    parameters: Optional[Dict[str, Any]] = None,
+    **kw_parameters,
 ):
     """
     Executes a user-defined function (UDF) with various execution and input options.
 
     This function supports executing UDFs in different environments (realtime, batch, local),
     with different types of inputs (tile coordinates, geographical bounding boxes, etc.), and
     allows for both synchronous and asynchronous execution. It dynamically determines the execution
@@ -105,41 +108,49 @@
             configuration, or None to specify UDF details in other parameters.
         udf_name: The name of the UDF to execute.
         udf: A GeoPandasUdfV2 object for direct execution.
         job_step: A UdfJobStepConfig object for detailed execution configuration.
         token: A token representing a shared UDF.
         udf_email: The email associated with the UDF.
         x, y, z: Tile coordinates for tile-based UDF execution.
-        lat, lng: Latitude and longitude for location-based UDF execution.
+        _lat, _lng: Latitude and longitude for tile-based UDF execution.
         bbox: A geographical bounding box (as a GeoDataFrame or shapely Geometry) defining the area of interest.
         sync: If True, execute the UDF synchronously. If False, execute asynchronously.
         engine: The execution engine to use ('realtime', 'batch', or 'local').
         type: The type of UDF execution ('tile' or 'file').
-        **parameters: Additional parameters to pass to the UDF.
+        parameters: Additional parameters to pass to the UDF.
+        **kw_parameters: Additional parameters to pass to the UDF.
 
     Raises:
         ValueError: If the UDF is not specified or is specified in more than one way.
         TypeError: If the first parameter is not of an expected type.
         Warning: Various warnings are issued for ignored parameters based on the execution path chosen.
 
     Returns:
         The result of the UDF execution, which varies based on the UDF and execution path.
 
     Examples:
 
-        # Run a UDF saved in the Fused system:
+
+        Run a UDF saved in the Fused system:
+        ```py
         fused.run(udf_email="username@fused.io", udf_name="my_udf_name")
+        ```
 
-        # Run a UDF saved in GitHub:
+        Run a UDF saved in GitHub:
+        ```py
         loaded_udf = fused.load("https://github.com/fusedio/udfs/tree/main/public/Building_Tile_Example")
         fused.run(udf=loaded_udf, bbox=bbox)
+        ```
 
-        # Run a UDF saved in a local directory:
+        Run a UDF saved in a local directory:
+        ```py
         loaded_udf = fused.load("/Users/local/dir/Building_Tile_Example")
         fused.run(udf=loaded_udf, bbox=bbox)
+        ```
 
     Note:
         This function dynamically determines the execution path and parameters based on the inputs.
         It is designed to be flexible and support various UDF execution scenarios.
     """
     if email_or_udf_or_token is not None:
         if udf is not None:
@@ -182,16 +193,16 @@
     if ways_of_specifying_udfs != 1:
         raise ValueError("UDF was specified in more than one way, which is invalid")
 
     local_tile_bbox: Optional[gpd.GeoDataFrame] = None
     if bbox is not None:
         if x is not None or y is not None or z is not None:
             warnings.warn("x, y, z arguments will be ignored in favor of bbox")
-        if lat is not None or lng is not None:
-            warnings.warn("lat, lng arguments will be ignored in favor of bbox")
+        if _lat is not None or _lng is not None:
+            warnings.warn("_lat, _lng arguments will be ignored in favor of bbox")
 
         if (
             "x" in bbox.columns
             and "y" in bbox.columns
             and "z" in bbox.columns
             and len(bbox) == 1
         ):
@@ -207,31 +218,31 @@
                 tile_bounds = shapely.bounds(bbox)
 
             tile = mercantile.bounding_tile(*tile_bounds)
             x, y, z = tile.x, tile.y, tile.z
             local_tile_bbox = gpd.GeoDataFrame(
                 {"x": [x], "y": [y], "z": [z]}, geometry=[shapely.box(*tile_bounds)]
             )
-    elif lat is not None and lng is not None:
+    elif _lat is not None and _lng is not None:
         if z is None:
             raise ValueError(
-                "Cannot compute x, y tile coordinates from lat, lng without z. You must specify z."
+                "Cannot compute x, y tile coordinates from _lat, _lng without z. You must specify z."
             )
         if x is not None or y is not None:
-            warnings.warn("x and y arguments will be ignored in favor of lat, lng")
+            warnings.warn("x and y arguments will be ignored in favor of _lat, _lng")
 
         import mercantile
 
-        tile = mercantile.tile(lng=lng, lat=lat, zoom=z)
+        tile = mercantile.tile(lng=_lng, lat=_lat, zoom=z)
         tile_bounds = mercantile.bounds(tile)
         x, y, z = tile.x, tile.y, tile.z
         local_tile_bbox = gpd.GeoDataFrame(
             {"x": [x], "y": [y], "z": [z]}, geometry=[shapely.box(*tile_bounds)]
         )
-    elif lat is not None or lng is not None:
+    elif _lat is not None or _lng is not None:
         warnings.warn("lat, lng arguments will be ignored because one of them is None")
     elif x is not None and y is not None and z is not None:
         import mercantile
 
         tile_bounds = mercantile.bounds(x, y, z)
         local_tile_bbox = gpd.GeoDataFrame(
             {"x": [x], "y": [y], "z": [z]}, geometry=[shapely.box(*tile_bounds)]
@@ -253,14 +264,19 @@
             raise ValueError(
                 "x, y, z not specified but type is 'tile', which is an invalid configuration. You must specify x, y, and z."
             )
 
     if udf is not None:
         job_step = UdfJobStepConfig(udf=udf)
 
+    parameters = {
+        **kw_parameters,
+        **(parameters if parameters is not None else {}),
+    }
+
     dispatch: dict[
         tuple[
             Literal["sync", "async"],
             Literal["tile", "file"],
             Literal["saved", "token", "local_job_step"],
             Literal["realtime", "local", "batch"],
         ],
```

### Comparing `fused-1.5.0/fused/_static/css/style.css` & `fused-1.5.1/fused/_static/css/style.css`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_static/html/icons-svg-inline.html` & `fused-1.5.1/fused/_static/html/icons-svg-inline.html`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_str_utils.py` & `fused-1.5.1/fused/_str_utils.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_templates/templates.py` & `fused-1.5.1/fused/_templates/templates.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_udf/coerce.py` & `fused-1.5.1/fused/_udf/coerce.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_udf/context.py` & `fused-1.5.1/fused/_udf/context.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_udf/decorators.py` & `fused-1.5.1/fused/_udf/decorators.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_udf/execute_v2.py` & `fused-1.5.1/fused/_udf/execute_v2.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_udf/load.py` & `fused-1.5.1/fused/_udf/load.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_udf/state.py` & `fused-1.5.1/fused/_udf/state.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/_utils.py` & `fused-1.5.1/fused/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,30 +60,33 @@
 - read_tiff_pc
 - table_to_tile
 - rasterize_geometry
 
 
 Examples:
 
-    # This example shows how to access the `geo_buffer` function from the `common` UDF.
+    This example shows how to access the `geo_buffer` function from the `common` UDF.
+    ```python
     import fused
     import geopandas as gpd
 
     gdf = gpd.read_file('https://www2.census.gov/geo/tiger/TIGER_RD18/STATE/11_DISTRICT_OF_COLUMBIA/11/tl_rd22_11_bg.zip')
     gdf_buffered = fused.public.common.geo_buffer(gdf, 10)
+    ```
 
-
-    # This example shows how to load a table with `table_to_tile`, which efficiently loads a table by filtering and adjusting based on the provided bounding box (bbox) and zoom level.
+    This example shows how to load a table with `table_to_tile`, which efficiently loads a table by filtering and adjusting based on the provided bounding box (bbox) and zoom level.
+    ```python
     table_path = "s3://fused-asset/infra/census_bg_us"
     gdf = fused.public.common.table_to_tile(
         bbox, table_path, use_columns=["GEOID", "geometry"], min_zoom=12
     )
+    ```
 
-
-    # This example shows how to use `rasterize_geometry` to place an input geometry within an image array.
+    This example shows how to use `rasterize_geometry` to place an input geometry within an image array.
+    ```python
     geom_masks = [
         rasterize_geometry(geom, arr.shape[-2:], transform) for geom in gdf.geometry
     ]
-
+    ```
 
 Public UDFs are listed at https://github.com/fusedio/udfs/tree/main/public
 """
```

### Comparing `fused-1.5.0/fused/api/_open_dataset.py` & `fused-1.5.1/fused/api/_open_dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/api/_public_api.py` & `fused-1.5.1/fused/api/_public_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/api/api.py` & `fused-1.5.1/fused/api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1155,17 +1155,17 @@
             path: The path to the root of the table on remote storage
 
         Keyword Args:
             fetch_samples: If True, fetch sample of each table when opening the dataset.
 
         Example:
 
-            table = fused.open_table(
-                path="s3://my_bucket/path/to/dataset/table/"
-            )
+            ```python
+            table = fused.open_table(path="s3://my_bucket/path/to/dataset/table/")
+            ```
 
         Returns:
             A Table object
         """
         request = request_models.OpenTableRequest(
             path=path,  # type: ignore
         )
```

### Comparing `fused-1.5.0/fused/api/credentials.py` & `fused-1.5.1/fused/api/credentials.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/api/docker_api.py` & `fused-1.5.1/fused/api/docker_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,17 +408,17 @@
             path: The path to the root of the table on remote storage
 
         Keyword Args:
             fetch_samples: If True, fetch sample of each table when opening the dataset.
 
         Example:
 
-            table = fused.open_table(
-                path="s3://my_bucket/path/to/dataset/table/"
-            )
+            ```python
+            table = fused.open_table(path="s3://my_bucket/path/to/dataset/table/")
+            ```
 
         Returns:
             A Table object
         """
         args = ["--base-path", path, "--output-to-stdout"]
 
         runnable = self._make_run_command("open-table", args)
```

### Comparing `fused-1.5.0/fused/api/docker_http_api.py` & `fused-1.5.1/fused/api/docker_http_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,17 +327,17 @@
             path: The path to the root of the table on remote storage
 
         Keyword Args:
             fetch_samples: If True, fetch sample of each table when opening the dataset.
 
         Example:
 
-            table = fused.open_table(
-                path="s3://my_bucket/path/to/dataset/table/"
-            )
+            ```python
+            table = fused.open_table(path="s3://my_bucket/path/to/dataset/table/")
+            ```
 
         Returns:
             A Table object
         """
         args = ["--base-path", path, "--output-to-stdout"]
 
         runnable = self._make_run_command("open-table", args)
```

### Comparing `fused-1.5.0/fused/core/_cache.py` & `fused-1.5.1/fused/core/_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,29 +257,33 @@
 
     Returns:
         Callable: A decorator that, when applied to a function, caches its
         return values according to the specified keyword arguments.
 
     Examples:
 
-        # Use the `@cache` decorator to cache the return value of a function in a custom path.
+        Use the `@cache` decorator to cache the return value of a function in a custom path.
 
+        ```py
         @cache(path="/tmp/custom_path/")
         def expensive_function():
             # Function implementation goes here
             return result
+        ```
 
-        # If the output of a cached function changes, for example if remote data is modified,
-        # it can be reset by running the function with the `reset` keyword argument. Afterward,
-        # the argument can be
+        If the output of a cached function changes, for example if remote data is modified,
+        it can be reset by running the function with the `reset` keyword argument. Afterward,
+        the argument can be cleared.
 
+        ```py
         @cache(path="/tmp/custom_path/", reset=True)
         def expensive_function():
             # Function implementation goes here
             return result
+        ```
     """
     return _cache_internal(func=func, **kwargs)
 
 
 T = TypeVar("T")
```

### Comparing `fused-1.5.0/fused/core/_download.py` & `fused-1.5.1/fused/core/_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,22 +78,23 @@
         url: The URL to download.
         file_path: The local path where to save the file.
 
     Returns:
         The function downloads the file only on the first execution, and returns the file path.
 
     Examples:
-
+        ```python
         @fused.udf
         def geodataframe_from_geojson():
             import geopandas as gpd
             url = "s3://sample_bucket/my_geojson.zip"
             path = fused.core.download(url, "tmp/my_geojson.zip")
             gdf = gpd.read_file(path)
             return gdf
+        ```
 
     """
 
     file_path = file_path.strip("/")
 
     # Cache in mounted drive if available & writable, else cache in /tmp
     base_path = data_path()
```

### Comparing `fused-1.5.0/fused/core/_impl/_download_impl.py` & `fused-1.5.1/fused/core/_impl/_download_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/core/_impl/_realtime_ops_impl.py` & `fused-1.5.1/fused/core/_impl/_realtime_ops_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/core/_impl/_table_ops_impl.py` & `fused-1.5.1/fused/core/_impl/_table_ops_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/core/_impl/_udf_ops_impl.py` & `fused-1.5.1/fused/core/_impl/_udf_ops_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/core/_realtime_ops.py` & `fused-1.5.1/fused/core/_realtime_ops.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/core/_table_ops.py` & `fused-1.5.1/fused/core/_table_ops.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 
     This can be called with file_id and chunk_id from `get_chunks_metadata`.
 
     Args:
         url: URL of the table.
         file_id: File ID to read.
         chunk_id: Chunk ID to read.
-
-    Keyword Args:
         columns: Read only the specified columns.
     """
     return _get_chunk_from_table(
         url=url,
         file_id=file_id,
         chunk_id=chunk_id,
         columns=columns,
```

### Comparing `fused-1.5.0/fused/core/_udf_ops.py` & `fused-1.5.1/fused/core/_udf_ops.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/__init__.py` & `fused-1.5.1/fused/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/_codegen/job.py` & `fused-1.5.1/fused/models/_codegen/job.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/_codegen/udf.py` & `fused-1.5.1/fused/models/_codegen/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/api/dataset.py` & `fused-1.5.1/fused/models/api/dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/api/job.py` & `fused-1.5.1/fused/models/api/job.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/api/udf_access_token.py` & `fused-1.5.1/fused/models/api/udf_access_token.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/base.py` & `fused-1.5.1/fused/models/base.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/coerce_dataset.py` & `fused-1.5.1/fused/models/coerce_dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/input.py` & `fused-1.5.1/fused/models/input.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/internal/dataset.py` & `fused-1.5.1/fused/models/internal/dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/internal/job.py` & `fused-1.5.1/fused/models/internal/job.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/migrations.py` & `fused-1.5.1/fused/models/migrations.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/request.py` & `fused-1.5.1/fused/models/request.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/schema.py` & `fused-1.5.1/fused/models/schema.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/udf/_eval_result.py` & `fused-1.5.1/fused/models/udf/_eval_result.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/udf/_specialized_udfs.py` & `fused-1.5.1/fused/models/udf/_specialized_udfs.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/udf/_udf_registry.py` & `fused-1.5.1/fused/models/udf/_udf_registry.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/udf/base_udf.py` & `fused-1.5.1/fused/models/udf/base_udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/udf/common.py` & `fused-1.5.1/fused/models/udf/common.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/udf/header.py` & `fused-1.5.1/fused/models/udf/header.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,17 +81,20 @@
     def write_to_gist(self):
         raise NotImplementedError
 
     def _exec(self) -> Dict[str, Any]:
         """
         Execute the header and return it's locals. This is comparable to importing the header.
         """
+        import fused
+
+        exec_globals = {"fused": fused}
         ret = {}
         # TODO: Does not raise HeaderSyntaxError here
-        exec(self.source_code, ret)
+        exec(self.source_code, exec_globals, ret)
         return ret
 
     def _register_custom_finder(self, preceding_sys_modules):
         module_name = self.module_name
         source_code = self.source_code
         self._preceding_sys_modules = preceding_sys_modules
 
@@ -157,9 +160,12 @@
         self.module_name = module_name
         self.source_code = source_code
 
     def create_module(self, spec):
         return None
 
     def exec_module(self, module):
+        import fused
+
+        exec_globals = {"fused": fused}
         # TODO: Does not raise HeaderSyntaxError here
-        exec(self.source_code, module.__dict__)
+        exec(self.source_code, exec_globals, module.__dict__)
```

### Comparing `fused-1.5.0/fused/models/udf/output.py` & `fused-1.5.1/fused/models/udf/output.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/udf/udf.py` & `fused-1.5.1/fused/models/udf/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/urls.py` & `fused-1.5.1/fused/models/urls.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/viz.py` & `fused-1.5.1/fused/models/viz.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/viz_colors.py` & `fused-1.5.1/fused/models/viz_colors.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/models/viz_presets.py` & `fused-1.5.1/fused/models/viz_presets.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/fused/warnings.py` & `fused-1.5.1/fused/warnings.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.0/pyproject.toml` & `fused-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "fused"
 # Version is set to 0.0.0 as the version string is automatically generated by
 # https://github.com/mtkennerly/poetry-dynamic-versioning
-version = "1.5.0"
+version = "1.5.1"
 description = ""
 authors = []
 readme = "README.md"
 packages = [{ include = "fused" }]
 
 [project.urls]
 Homepage = "https://www.fused.io"
```

### Comparing `fused-1.5.0/PKG-INFO` & `fused-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fused
-Version: 1.5.0
+Version: 1.5.1
 Summary: 
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


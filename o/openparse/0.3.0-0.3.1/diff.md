# Comparing `tmp/openparse-0.3.0.tar.gz` & `tmp/openparse-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openparse-0.3.0.tar", last modified: Sun Mar 31 21:57:02 2024, max compression
+gzip compressed data, was "openparse-0.3.1.tar", last modified: Mon Apr  1 21:30:39 2024, max compression
```

## Comparing `openparse-0.3.0.tar` & `openparse-0.3.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.631684 openparse-0.3.0/
--rw-r--r--   0 sergey     (501) staff       (20)     1072 2024-03-26 18:50:21.000000 openparse-0.3.0/LICENSE
--rw-r--r--   0 sergey     (501) staff       (20)     4577 2024-03-31 21:57:02.631434 openparse-0.3.0/PKG-INFO
--rw-r--r--   0 sergey     (501) staff       (20)     3968 2024-03-31 21:53:11.000000 openparse-0.3.0/README.md
--rw-r--r--   0 sergey     (501) staff       (20)       38 2024-03-31 21:57:02.631734 openparse-0.3.0/setup.cfg
--rw-r--r--   0 sergey     (501) staff       (20)      704 2024-03-31 21:56:10.000000 openparse-0.3.0/setup.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.613048 openparse-0.3.0/src/
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.614727 openparse-0.3.0/src/evals/
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-25 03:59:07.000000 openparse-0.3.0/src/evals/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      684 2024-03-31 16:14:48.000000 openparse-0.3.0/src/evals/run_evals.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.615431 openparse-0.3.0/src/notebooks/
--rw-r--r--   0 sergey     (501) staff       (20)       68 2024-03-25 18:09:44.000000 openparse-0.3.0/src/notebooks/config.py
--rw-r--r--   0 sergey     (501) staff       (20)    29161 2024-03-27 07:16:53.000000 openparse-0.3.0/src/notebooks/trash.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.617743 openparse-0.3.0/src/openparse/
--rw-r--r--   0 sergey     (501) staff       (20)      435 2024-03-27 22:22:49.000000 openparse-0.3.0/src/openparse/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      225 2024-03-31 17:51:39.000000 openparse-0.3.0/src/openparse/consts.py
--rw-r--r--   0 sergey     (501) staff       (20)     3190 2024-03-27 22:42:17.000000 openparse-0.3.0/src/openparse/main.py
--rw-r--r--   0 sergey     (501) staff       (20)     6095 2024-03-31 19:47:46.000000 openparse-0.3.0/src/openparse/pdf.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.619212 openparse-0.3.0/src/openparse/postprocessing/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-22 22:57:26.000000 openparse-0.3.0/src/openparse/postprocessing/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      478 2024-03-27 17:19:41.000000 openparse-0.3.0/src/openparse/postprocessing/ingest.py
--rw-r--r--   0 sergey     (501) staff       (20)      733 2024-03-27 17:19:41.000000 openparse-0.3.0/src/openparse/postprocessing/steps.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.620145 openparse-0.3.0/src/openparse/processing/
--rw-r--r--   0 sergey     (501) staff       (20)      609 2024-03-31 21:13:57.000000 openparse-0.3.0/src/openparse/processing/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      531 2024-03-27 22:41:54.000000 openparse-0.3.0/src/openparse/processing/ingest.py
--rw-r--r--   0 sergey     (501) staff       (20)    10136 2024-03-31 21:47:45.000000 openparse-0.3.0/src/openparse/processing/steps.py
--rw-r--r--   0 sergey     (501) staff       (20)    17544 2024-03-31 21:36:06.000000 openparse-0.3.0/src/openparse/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.621368 openparse-0.3.0/src/openparse/tables/
--rw-r--r--   0 sergey     (501) staff       (20)      124 2024-03-27 17:19:41.000000 openparse-0.3.0/src/openparse/tables/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     4933 2024-03-27 22:10:32.000000 openparse-0.3.0/src/openparse/tables/parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.622314 openparse-0.3.0/src/openparse/tables/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)      174 2024-03-27 17:19:41.000000 openparse-0.3.0/src/openparse/tables/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1199 2024-03-27 05:08:58.000000 openparse-0.3.0/src/openparse/tables/pymupdf/parse.py
--rw-r--r--   0 sergey     (501) staff       (20)     7727 2024-03-27 17:19:41.000000 openparse-0.3.0/src/openparse/tables/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.623643 openparse-0.3.0/src/openparse/tables/table_transformers/
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-27 16:25:28.000000 openparse-0.3.0/src/openparse/tables/table_transformers/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2700 2024-03-29 00:46:39.000000 openparse-0.3.0/src/openparse/tables/table_transformers/geometry.py
--rw-r--r--   0 sergey     (501) staff       (20)    10495 2024-03-29 00:46:39.000000 openparse-0.3.0/src/openparse/tables/table_transformers/ml.py
--rw-r--r--   0 sergey     (501) staff       (20)      950 2024-03-27 17:19:41.000000 openparse-0.3.0/src/openparse/tables/table_transformers/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.624027 openparse-0.3.0/src/openparse/tables/unitable/
--rw-r--r--   0 sergey     (501) staff       (20)     6849 2024-03-28 19:39:53.000000 openparse-0.3.0/src/openparse/tables/unitable/ml.py
--rw-r--r--   0 sergey     (501) staff       (20)     3424 2024-03-27 22:12:24.000000 openparse-0.3.0/src/openparse/tables/utils.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.624588 openparse-0.3.0/src/openparse/text/
--rw-r--r--   0 sergey     (501) staff       (20)       48 2024-03-27 17:16:27.000000 openparse-0.3.0/src/openparse/text/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      743 2024-03-27 17:19:41.000000 openparse-0.3.0/src/openparse/text/parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.625189 openparse-0.3.0/src/openparse/text/pdfminer/
--rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:16:32.000000 openparse-0.3.0/src/openparse/text/pdfminer/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     4484 2024-03-29 18:14:03.000000 openparse-0.3.0/src/openparse/text/pdfminer/core.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.625636 openparse-0.3.0/src/openparse/text/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:19:41.000000 openparse-0.3.0/src/openparse/text/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2815 2024-03-27 17:19:41.000000 openparse-0.3.0/src/openparse/text/pymupdf/core.py
--rw-r--r--   0 sergey     (501) staff       (20)      221 2024-03-27 17:19:41.000000 openparse-0.3.0/src/openparse/utils.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.630831 openparse-0.3.0/src/openparse.egg-info/
--rw-r--r--   0 sergey     (501) staff       (20)     4577 2024-03-31 21:57:02.000000 openparse-0.3.0/src/openparse.egg-info/PKG-INFO
--rw-r--r--   0 sergey     (501) staff       (20)     1767 2024-03-31 21:57:02.000000 openparse-0.3.0/src/openparse.egg-info/SOURCES.txt
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-31 21:57:02.000000 openparse-0.3.0/src/openparse.egg-info/dependency_links.txt
--rw-r--r--   0 sergey     (501) staff       (20)      127 2024-03-31 21:57:02.000000 openparse-0.3.0/src/openparse.egg-info/requires.txt
--rw-r--r--   0 sergey     (501) staff       (20)       32 2024-03-31 21:57:02.000000 openparse-0.3.0/src/openparse.egg-info/top_level.txt
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.626317 openparse-0.3.0/src/tests/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-23 00:56:45.000000 openparse-0.3.0/src/tests/__init__.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.628188 openparse-0.3.0/src/tests/processing/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 01:35:13.000000 openparse-0.3.0/src/tests/processing/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1085 2024-03-31 15:54:18.000000 openparse-0.3.0/src/tests/processing/test_pipeline.py
--rw-r--r--   0 sergey     (501) staff       (20)    16585 2024-03-31 21:47:11.000000 openparse-0.3.0/src/tests/processing/test_steps.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.628877 openparse-0.3.0/src/tests/tables/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 03:12:34.000000 openparse-0.3.0/src/tests/tables/__init__.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.629146 openparse-0.3.0/src/tests/tables/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 04:18:24.000000 openparse-0.3.0/src/tests/tables/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2765 2024-03-27 17:19:41.000000 openparse-0.3.0/src/tests/tables/pymupdf/test_parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.630052 openparse-0.3.0/src/tests/tables/transformers/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 03:41:31.000000 openparse-0.3.0/src/tests/tables/transformers/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2174 2024-03-29 00:46:39.000000 openparse-0.3.0/src/tests/tables/transformers/test_geometry.py
--rw-r--r--   0 sergey     (501) staff       (20)    10190 2024-03-27 17:17:26.000000 openparse-0.3.0/src/tests/tables/transformers/test_ml.py
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-28 23:19:06.000000 openparse-0.3.0/src/tests/test_main.py
--rw-r--r--   0 sergey     (501) staff       (20)    20672 2024-03-31 21:03:58.000000 openparse-0.3.0/src/tests/test_schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.613452 openparse-0.3.0/src/tests/text/
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-03-31 21:57:02.630494 openparse-0.3.0/src/tests/text/pdf_miner/
--rw-r--r--   0 sergey     (501) staff       (20)     4002 2024-03-27 17:19:41.000000 openparse-0.3.0/src/tests/text/pdf_miner/test_core.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.232764 openparse-0.3.1/
+-rw-r--r--   0 sergey     (501) staff       (20)     1072 2024-03-26 18:50:21.000000 openparse-0.3.1/LICENSE
+-rw-r--r--   0 sergey     (501) staff       (20)     4581 2024-04-01 21:30:39.232469 openparse-0.3.1/PKG-INFO
+-rw-r--r--   0 sergey     (501) staff       (20)     3970 2024-04-01 21:24:05.000000 openparse-0.3.1/README.md
+-rw-r--r--   0 sergey     (501) staff       (20)       38 2024-04-01 21:30:39.232818 openparse-0.3.1/setup.cfg
+-rw-r--r--   0 sergey     (501) staff       (20)      706 2024-04-01 21:28:49.000000 openparse-0.3.1/setup.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.215076 openparse-0.3.1/src/
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.216854 openparse-0.3.1/src/evals/
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-25 03:59:07.000000 openparse-0.3.1/src/evals/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)      684 2024-03-31 16:14:48.000000 openparse-0.3.1/src/evals/run_evals.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.217583 openparse-0.3.1/src/notebooks/
+-rw-r--r--   0 sergey     (501) staff       (20)       68 2024-03-25 18:09:44.000000 openparse-0.3.1/src/notebooks/config.py
+-rw-r--r--   0 sergey     (501) staff       (20)    29161 2024-03-27 07:16:53.000000 openparse-0.3.1/src/notebooks/trash.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.219991 openparse-0.3.1/src/openparse/
+-rw-r--r--   0 sergey     (501) staff       (20)      435 2024-03-27 22:22:49.000000 openparse-0.3.1/src/openparse/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)      225 2024-03-31 17:51:39.000000 openparse-0.3.1/src/openparse/consts.py
+-rw-r--r--   0 sergey     (501) staff       (20)     3190 2024-03-27 22:42:17.000000 openparse-0.3.1/src/openparse/main.py
+-rw-r--r--   0 sergey     (501) staff       (20)     6083 2024-04-01 21:28:09.000000 openparse-0.3.1/src/openparse/pdf.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.221513 openparse-0.3.1/src/openparse/postprocessing/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-22 22:57:26.000000 openparse-0.3.1/src/openparse/postprocessing/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)      478 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/postprocessing/ingest.py
+-rw-r--r--   0 sergey     (501) staff       (20)      733 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/postprocessing/steps.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.222315 openparse-0.3.1/src/openparse/processing/
+-rw-r--r--   0 sergey     (501) staff       (20)      609 2024-03-31 21:13:57.000000 openparse-0.3.1/src/openparse/processing/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)      531 2024-03-27 22:41:54.000000 openparse-0.3.1/src/openparse/processing/ingest.py
+-rw-r--r--   0 sergey     (501) staff       (20)    10136 2024-03-31 21:47:45.000000 openparse-0.3.1/src/openparse/processing/steps.py
+-rw-r--r--   0 sergey     (501) staff       (20)    17544 2024-03-31 21:36:06.000000 openparse-0.3.1/src/openparse/schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.223572 openparse-0.3.1/src/openparse/tables/
+-rw-r--r--   0 sergey     (501) staff       (20)      124 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/tables/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     4933 2024-03-27 22:10:32.000000 openparse-0.3.1/src/openparse/tables/parse.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.224132 openparse-0.3.1/src/openparse/tables/pymupdf/
+-rw-r--r--   0 sergey     (501) staff       (20)      174 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/tables/pymupdf/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1199 2024-03-27 05:08:58.000000 openparse-0.3.1/src/openparse/tables/pymupdf/parse.py
+-rw-r--r--   0 sergey     (501) staff       (20)     7727 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/tables/schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.225728 openparse-0.3.1/src/openparse/tables/table_transformers/
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-27 16:25:28.000000 openparse-0.3.1/src/openparse/tables/table_transformers/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2700 2024-03-29 00:46:39.000000 openparse-0.3.1/src/openparse/tables/table_transformers/geometry.py
+-rw-r--r--   0 sergey     (501) staff       (20)    10495 2024-03-29 00:46:39.000000 openparse-0.3.1/src/openparse/tables/table_transformers/ml.py
+-rw-r--r--   0 sergey     (501) staff       (20)      950 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/tables/table_transformers/schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.226211 openparse-0.3.1/src/openparse/tables/unitable/
+-rw-r--r--   0 sergey     (501) staff       (20)     6849 2024-03-28 19:39:53.000000 openparse-0.3.1/src/openparse/tables/unitable/ml.py
+-rw-r--r--   0 sergey     (501) staff       (20)     3424 2024-03-27 22:12:24.000000 openparse-0.3.1/src/openparse/tables/utils.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.226783 openparse-0.3.1/src/openparse/text/
+-rw-r--r--   0 sergey     (501) staff       (20)       48 2024-03-27 17:16:27.000000 openparse-0.3.1/src/openparse/text/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)      743 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/text/parse.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.227342 openparse-0.3.1/src/openparse/text/pdfminer/
+-rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:16:32.000000 openparse-0.3.1/src/openparse/text/pdfminer/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     4484 2024-03-29 18:14:03.000000 openparse-0.3.1/src/openparse/text/pdfminer/core.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.227834 openparse-0.3.1/src/openparse/text/pymupdf/
+-rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/text/pymupdf/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2815 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/text/pymupdf/core.py
+-rw-r--r--   0 sergey     (501) staff       (20)      221 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/utils.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.231632 openparse-0.3.1/src/openparse.egg-info/
+-rw-r--r--   0 sergey     (501) staff       (20)     4581 2024-04-01 21:30:39.000000 openparse-0.3.1/src/openparse.egg-info/PKG-INFO
+-rw-r--r--   0 sergey     (501) staff       (20)     1767 2024-04-01 21:30:39.000000 openparse-0.3.1/src/openparse.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-04-01 21:30:39.000000 openparse-0.3.1/src/openparse.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey     (501) staff       (20)      129 2024-04-01 21:30:39.000000 openparse-0.3.1/src/openparse.egg-info/requires.txt
+-rw-r--r--   0 sergey     (501) staff       (20)       32 2024-04-01 21:30:39.000000 openparse-0.3.1/src/openparse.egg-info/top_level.txt
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.228524 openparse-0.3.1/src/tests/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-23 00:56:45.000000 openparse-0.3.1/src/tests/__init__.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.229574 openparse-0.3.1/src/tests/processing/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 01:35:13.000000 openparse-0.3.1/src/tests/processing/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1085 2024-03-31 15:54:18.000000 openparse-0.3.1/src/tests/processing/test_pipeline.py
+-rw-r--r--   0 sergey     (501) staff       (20)    16585 2024-03-31 21:47:11.000000 openparse-0.3.1/src/tests/processing/test_steps.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.229941 openparse-0.3.1/src/tests/tables/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 03:12:34.000000 openparse-0.3.1/src/tests/tables/__init__.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.230162 openparse-0.3.1/src/tests/tables/pymupdf/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 04:18:24.000000 openparse-0.3.1/src/tests/tables/pymupdf/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2765 2024-03-27 17:19:41.000000 openparse-0.3.1/src/tests/tables/pymupdf/test_parse.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.230945 openparse-0.3.1/src/tests/tables/transformers/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 03:41:31.000000 openparse-0.3.1/src/tests/tables/transformers/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2174 2024-03-29 00:46:39.000000 openparse-0.3.1/src/tests/tables/transformers/test_geometry.py
+-rw-r--r--   0 sergey     (501) staff       (20)    10190 2024-03-27 17:17:26.000000 openparse-0.3.1/src/tests/tables/transformers/test_ml.py
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-28 23:19:06.000000 openparse-0.3.1/src/tests/test_main.py
+-rw-r--r--   0 sergey     (501) staff       (20)    20672 2024-03-31 21:03:58.000000 openparse-0.3.1/src/tests/test_schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.215465 openparse-0.3.1/src/tests/text/
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.231297 openparse-0.3.1/src/tests/text/pdf_miner/
+-rw-r--r--   0 sergey     (501) staff       (20)     4002 2024-03-27 17:19:41.000000 openparse-0.3.1/src/tests/text/pdf_miner/test_core.py
```

### Comparing `openparse-0.3.0/LICENSE` & `openparse-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/PKG-INFO` & `openparse-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: openparse
-Version: 0.3.0
+Version: 0.3.1
 Summary: Streamlines the process of preparing documents for LLM's.
 Home-page: https://github.com/Filimoa/open-parse/
 Author: Sergey Filimonov
 Author-email: hello@sergey.fyi
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyMuPDF>=1.23
+Requires-Dist: PyMuPDF>=1.23.2
 Requires-Dist: pillow>=8.3
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pypdf>=4.0.0
 Requires-Dist: pdfminer.six>=20200401
 Requires-Dist: tiktoken>=0.3
 Provides-Extra: ml
 Requires-Dist: torch; extra == "ml"
@@ -45,15 +45,15 @@
 import openparse
 
 basic_doc_path = "./sample-docs/mobile-home-manual.pdf"
 parser = openparse.DocumentParser()
 parsed_basic_doc = parser.parse(basic_doc_path)
 
 for node in parsed_basic_doc.nodes:
-    print(node)
+    display(node)
 ```
 
 **📓 Try the sample notebook** <a href="https://colab.research.google.com/drive/1Z5B5gsnmhFKEFL-5yYIcoox7-jQao8Ep?usp=sharing" class="external-link" target="_blank">here</a>
 
 ## Requirements
 
 Python 3.8+
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: openparse Version: 0.3.0 Summary: Streamlines the
+Metadata-Version: 2.1 Name: openparse Version: 0.3.1 Summary: Streamlines the
 process of preparing documents for LLM's. Home-page: https://github.com/
 Filimoa/open-parse/ Author: Sergey Filimonov Author-email: hello@sergey.fyi
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-PyMuPDF>=1.23 Requires-Dist: pillow>=8.3 Requires-Dist: pydantic>=2.0 Requires-
-Dist: pypdf>=4.0.0 Requires-Dist: pdfminer.six>=20200401 Requires-Dist:
-tiktoken>=0.3 Provides-Extra: ml Requires-Dist: torch; extra == "ml" Requires-
-Dist: torchvision; extra == "ml" Requires-Dist: transformers; extra == "ml"
+PyMuPDF>=1.23.2 Requires-Dist: pillow>=8.3 Requires-Dist: pydantic>=2.0
+Requires-Dist: pypdf>=4.0.0 Requires-Dist: pdfminer.six>=20200401 Requires-
+Dist: tiktoken>=0.3 Provides-Extra: ml Requires-Dist: torch; extra == "ml"
+Requires-Dist: torchvision; extra == "ml" Requires-Dist: transformers; extra ==
+"ml"
  [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/open-parse-
                             with-text-tp-logo.webp]
 
 Open-Parse streamlines the process of preparing complex documents for analysis
 by LLMs. Our goal is to expose state-of-the-art deep learning models with a few
 lines of code while also providing flexible heuristic options for faster, basic
 parsing. ### Highlights - **ð Visually-Driven:** Open-Parse visually
@@ -21,15 +22,15 @@
 **ð¡Intuitive:** Great editor support. Completion everywhere. Less time
 debugging. - **ð¯ Easy:** Designed to be easy to use and learn. Less time
 reading docs.
 [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/marked-up-doc-
                                     2.webp]
 ## Example ```python import openparse basic_doc_path = "./sample-docs/mobile-
 home-manual.pdf" parser = openparse.DocumentParser() parsed_basic_doc =
-parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: print(node)
+parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: display(node)
 ``` **ð Try the sample notebook** _h_e_r_e ## Requirements Python 3.8+ **Dealing
 with PDF's:** - _p_d_f_m_i_n_e_r_._s_i_x Fully open source. **Extracting Tables:** -
 _P_y_M_u_P_D_F has some table detection functionality. Please see their _l_i_c_e_n_s_e. -
 _T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning approach. - _u_n_i_t_a_b_l_e is a more recent deep
 learning approach that seems promising _(coming soon)_ ## Installation #### 1.
 Core Library ```console pip install openparse ``` **Enabling OCR Support**:
 PyMuPDF will already contain all the logic to support OCR functions. But it
```

### Comparing `openparse-0.3.0/README.md` & `openparse-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import openparse
 
 basic_doc_path = "./sample-docs/mobile-home-manual.pdf"
 parser = openparse.DocumentParser()
 parsed_basic_doc = parser.parse(basic_doc_path)
 
 for node in parsed_basic_doc.nodes:
-    print(node)
+    display(node)
 ```
 
 **📓 Try the sample notebook** <a href="https://colab.research.google.com/drive/1Z5B5gsnmhFKEFL-5yYIcoox7-jQao8Ep?usp=sharing" class="external-link" target="_blank">here</a>
 
 ## Requirements
 
 Python 3.8+
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 **ð¡Intuitive:** Great editor support. Completion everywhere. Less time
 debugging. - **ð¯ Easy:** Designed to be easy to use and learn. Less time
 reading docs.
 [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/marked-up-doc-
                                     2.webp]
 ## Example ```python import openparse basic_doc_path = "./sample-docs/mobile-
 home-manual.pdf" parser = openparse.DocumentParser() parsed_basic_doc =
-parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: print(node)
+parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: display(node)
 ``` **ð Try the sample notebook** _h_e_r_e ## Requirements Python 3.8+ **Dealing
 with PDF's:** - _p_d_f_m_i_n_e_r_._s_i_x Fully open source. **Extracting Tables:** -
 _P_y_M_u_P_D_F has some table detection functionality. Please see their _l_i_c_e_n_s_e. -
 _T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning approach. - _u_n_i_t_a_b_l_e is a more recent deep
 learning approach that seems promising _(coming soon)_ ## Installation #### 1.
 Core Library ```console pip install openparse ``` **Enabling OCR Support**:
 PyMuPDF will already contain all the logic to support OCR functions. But it
```

### Comparing `openparse-0.3.0/setup.py` & `openparse-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="openparse",
-    version="0.3.0",
+    version="0.3.1",
     install_requires=[
-        "PyMuPDF >= 1.23",
+        "PyMuPDF >= 1.23.2",
         "pillow >= 8.3",
         "pydantic >= 2.0",
         "pypdf >= 4.0.0",
         "pdfminer.six >= 20200401",
         "tiktoken >= 0.3",
     ],
     extras_require={
```

### Comparing `openparse-0.3.0/src/evals/run_evals.py` & `openparse-0.3.1/src/evals/run_evals.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/notebooks/trash.py` & `openparse-0.3.1/src/notebooks/trash.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/main.py` & `openparse-0.3.1/src/openparse/main.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/pdf.py` & `openparse-0.3.1/src/openparse/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
             for bbox_with_color in bboxes_with_color:
                 bbox = bbox_with_color.bbox
                 if bbox.page != page.number:
                     continue
                 if coordinates == "bottom-left":
                     bbox = self._flip_coordinates(bbox)
-                rect = fitz.Rect(x0=bbox.x0, y0=bbox.y0, x1=bbox.x1, y1=bbox.y1)
+                rect = fitz.Rect(bbox.x0, bbox.y0, bbox.x1, bbox.y1)
                 page.draw_rect(
                     rect, bbox_with_color.color
                 )  # Use the color associated with this bbox
         return pdf
 
     def display_with_bboxes(
         self,
```

### Comparing `openparse-0.3.0/src/openparse/postprocessing/steps.py` & `openparse-0.3.1/src/openparse/postprocessing/steps.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/processing/__init__.py` & `openparse-0.3.1/src/openparse/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/processing/ingest.py` & `openparse-0.3.1/src/openparse/processing/ingest.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/processing/steps.py` & `openparse-0.3.1/src/openparse/processing/steps.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/schemas.py` & `openparse-0.3.1/src/openparse/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/tables/parse.py` & `openparse-0.3.1/src/openparse/tables/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/tables/pymupdf/parse.py` & `openparse-0.3.1/src/openparse/tables/pymupdf/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/tables/schemas.py` & `openparse-0.3.1/src/openparse/tables/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/tables/table_transformers/geometry.py` & `openparse-0.3.1/src/openparse/tables/table_transformers/geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/tables/table_transformers/ml.py` & `openparse-0.3.1/src/openparse/tables/table_transformers/ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/tables/table_transformers/schemas.py` & `openparse-0.3.1/src/openparse/tables/table_transformers/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/tables/unitable/ml.py` & `openparse-0.3.1/src/openparse/tables/unitable/ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/tables/utils.py` & `openparse-0.3.1/src/openparse/tables/utils.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/text/parse.py` & `openparse-0.3.1/src/openparse/text/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/text/pdfminer/core.py` & `openparse-0.3.1/src/openparse/text/pdfminer/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse/text/pymupdf/core.py` & `openparse-0.3.1/src/openparse/text/pymupdf/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/openparse.egg-info/PKG-INFO` & `openparse-0.3.1/src/openparse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: openparse
-Version: 0.3.0
+Version: 0.3.1
 Summary: Streamlines the process of preparing documents for LLM's.
 Home-page: https://github.com/Filimoa/open-parse/
 Author: Sergey Filimonov
 Author-email: hello@sergey.fyi
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyMuPDF>=1.23
+Requires-Dist: PyMuPDF>=1.23.2
 Requires-Dist: pillow>=8.3
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pypdf>=4.0.0
 Requires-Dist: pdfminer.six>=20200401
 Requires-Dist: tiktoken>=0.3
 Provides-Extra: ml
 Requires-Dist: torch; extra == "ml"
@@ -45,15 +45,15 @@
 import openparse
 
 basic_doc_path = "./sample-docs/mobile-home-manual.pdf"
 parser = openparse.DocumentParser()
 parsed_basic_doc = parser.parse(basic_doc_path)
 
 for node in parsed_basic_doc.nodes:
-    print(node)
+    display(node)
 ```
 
 **📓 Try the sample notebook** <a href="https://colab.research.google.com/drive/1Z5B5gsnmhFKEFL-5yYIcoox7-jQao8Ep?usp=sharing" class="external-link" target="_blank">here</a>
 
 ## Requirements
 
 Python 3.8+
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: openparse Version: 0.3.0 Summary: Streamlines the
+Metadata-Version: 2.1 Name: openparse Version: 0.3.1 Summary: Streamlines the
 process of preparing documents for LLM's. Home-page: https://github.com/
 Filimoa/open-parse/ Author: Sergey Filimonov Author-email: hello@sergey.fyi
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-PyMuPDF>=1.23 Requires-Dist: pillow>=8.3 Requires-Dist: pydantic>=2.0 Requires-
-Dist: pypdf>=4.0.0 Requires-Dist: pdfminer.six>=20200401 Requires-Dist:
-tiktoken>=0.3 Provides-Extra: ml Requires-Dist: torch; extra == "ml" Requires-
-Dist: torchvision; extra == "ml" Requires-Dist: transformers; extra == "ml"
+PyMuPDF>=1.23.2 Requires-Dist: pillow>=8.3 Requires-Dist: pydantic>=2.0
+Requires-Dist: pypdf>=4.0.0 Requires-Dist: pdfminer.six>=20200401 Requires-
+Dist: tiktoken>=0.3 Provides-Extra: ml Requires-Dist: torch; extra == "ml"
+Requires-Dist: torchvision; extra == "ml" Requires-Dist: transformers; extra ==
+"ml"
  [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/open-parse-
                             with-text-tp-logo.webp]
 
 Open-Parse streamlines the process of preparing complex documents for analysis
 by LLMs. Our goal is to expose state-of-the-art deep learning models with a few
 lines of code while also providing flexible heuristic options for faster, basic
 parsing. ### Highlights - **ð Visually-Driven:** Open-Parse visually
@@ -21,15 +22,15 @@
 **ð¡Intuitive:** Great editor support. Completion everywhere. Less time
 debugging. - **ð¯ Easy:** Designed to be easy to use and learn. Less time
 reading docs.
 [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/marked-up-doc-
                                     2.webp]
 ## Example ```python import openparse basic_doc_path = "./sample-docs/mobile-
 home-manual.pdf" parser = openparse.DocumentParser() parsed_basic_doc =
-parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: print(node)
+parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: display(node)
 ``` **ð Try the sample notebook** _h_e_r_e ## Requirements Python 3.8+ **Dealing
 with PDF's:** - _p_d_f_m_i_n_e_r_._s_i_x Fully open source. **Extracting Tables:** -
 _P_y_M_u_P_D_F has some table detection functionality. Please see their _l_i_c_e_n_s_e. -
 _T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning approach. - _u_n_i_t_a_b_l_e is a more recent deep
 learning approach that seems promising _(coming soon)_ ## Installation #### 1.
 Core Library ```console pip install openparse ``` **Enabling OCR Support**:
 PyMuPDF will already contain all the logic to support OCR functions. But it
```

### Comparing `openparse-0.3.0/src/openparse.egg-info/SOURCES.txt` & `openparse-0.3.1/src/openparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/tests/processing/test_pipeline.py` & `openparse-0.3.1/src/tests/processing/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/tests/processing/test_steps.py` & `openparse-0.3.1/src/tests/processing/test_steps.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/tests/tables/pymupdf/test_parse.py` & `openparse-0.3.1/src/tests/tables/pymupdf/test_parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/tests/tables/transformers/test_geometry.py` & `openparse-0.3.1/src/tests/tables/transformers/test_geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/tests/tables/transformers/test_ml.py` & `openparse-0.3.1/src/tests/tables/transformers/test_ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/tests/test_schemas.py` & `openparse-0.3.1/src/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.0/src/tests/text/pdf_miner/test_core.py` & `openparse-0.3.1/src/tests/text/pdf_miner/test_core.py`

 * *Files identical despite different names*


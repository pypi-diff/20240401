# Comparing `tmp/meditability-0.2.1.tar.gz` & `tmp/meditability-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meditability-0.2.1.tar", last modified: Tue Feb  6 18:14:24 2024, max compression
+gzip compressed data, was "meditability-0.2.2.tar", last modified: Mon Apr  1 18:06:59 2024, max compression
```

## Comparing `meditability-0.2.1.tar` & `meditability-0.2.2.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxr-xr-x   0 bellieny   (503) staff       (20)        0 2024-02-06 18:14:24.321859 meditability-0.2.1/
--rw-r--r--   0 bellieny   (503) staff       (20)    32337 2024-01-25 20:51:34.000000 meditability-0.2.1/LICENSE
--rw-r--r--   0 bellieny   (503) staff       (20)      558 2024-02-06 18:14:24.321437 meditability-0.2.1/PKG-INFO
--rw-r--r--   0 bellieny   (503) staff       (20)     3621 2024-02-06 18:00:58.000000 meditability-0.2.1/README.md
--rw-r--r--   0 bellieny   (503) staff       (20)       38 2024-02-06 18:14:24.321938 meditability-0.2.1/setup.cfg
--rw-r--r--   0 bellieny   (503) staff       (20)     1018 2024-02-06 18:14:13.000000 meditability-0.2.1/setup.py
-drwxr-xr-x   0 bellieny   (503) staff       (20)        0 2024-02-06 18:14:24.012319 meditability-0.2.1/src/
-drwxr-xr-x   0 bellieny   (503) staff       (20)        0 2024-02-06 18:14:24.320903 meditability-0.2.1/src/meditability.egg-info/
--rw-r--r--   0 bellieny   (503) staff       (20)      558 2024-02-06 18:14:23.000000 meditability-0.2.1/src/meditability.egg-info/PKG-INFO
--rw-r--r--   0 bellieny   (503) staff       (20)     1934 2024-02-06 18:14:23.000000 meditability-0.2.1/src/meditability.egg-info/SOURCES.txt
--rw-r--r--   0 bellieny   (503) staff       (20)        1 2024-02-06 18:14:23.000000 meditability-0.2.1/src/meditability.egg-info/dependency_links.txt
--rw-r--r--   0 bellieny   (503) staff       (20)       36 2024-02-06 18:14:23.000000 meditability-0.2.1/src/meditability.egg-info/entry_points.txt
--rw-r--r--   0 bellieny   (503) staff       (20)      148 2024-02-06 18:14:23.000000 meditability-0.2.1/src/meditability.egg-info/requires.txt
--rw-r--r--   0 bellieny   (503) staff       (20)        9 2024-02-06 18:14:23.000000 meditability-0.2.1/src/meditability.egg-info/top_level.txt
-drwxr-xr-x   0 bellieny   (503) staff       (20)        0 2024-02-06 18:14:24.060662 meditability-0.2.1/src/prog/
--rw-r--r--   0 bellieny   (503) staff       (20)       24 2024-01-08 18:09:54.000000 meditability-0.2.1/src/prog/__init__.py
--rw-r--r--   0 bellieny   (503) staff       (20)     8424 2024-02-05 19:58:49.000000 meditability-0.2.1/src/prog/arguments.py
--rw-r--r--   0 bellieny   (503) staff       (20)     5602 2024-02-06 00:41:45.000000 meditability-0.2.1/src/prog/db_set.py
--rw-r--r--   0 bellieny   (503) staff       (20)     6856 2024-02-05 23:34:21.000000 meditability-0.2.1/src/prog/guide_prediction.py
--rw-r--r--   0 bellieny   (503) staff       (20)     1041 2024-01-25 20:39:18.000000 meditability-0.2.1/src/prog/list_editors.py
--rw-r--r--   0 bellieny   (503) staff       (20)      911 2024-01-25 20:32:22.000000 meditability-0.2.1/src/prog/mEdit.py
--rw-r--r--   0 bellieny   (503) staff       (20)     6743 2024-02-06 18:14:13.000000 meditability-0.2.1/src/prog/medit_lib.py
-drwxr-xr-x   0 bellieny   (503) staff       (20)        0 2024-02-06 18:14:24.061330 meditability-0.2.1/src/smk/
--rw-r--r--   0 bellieny   (503) staff       (20)        0 2024-01-10 18:47:01.000000 meditability-0.2.1/src/smk/__init__.py
-drwxr-xr-x   0 bellieny   (503) staff       (20)        0 2024-02-06 18:14:24.142844 meditability-0.2.1/src/smk/config/
--rw-r--r--   0 bellieny   (503) staff       (20)        0 2024-01-10 17:53:11.000000 meditability-0.2.1/src/smk/config/__init__.py
--rw-r--r--   0 bellieny   (503) staff       (20)     2209 2023-10-30 16:30:06.000000 meditability-0.2.1/src/smk/config/aws_download.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)      469 2023-09-27 16:24:56.000000 meditability-0.2.1/src/smk/config/caspedia_ingest.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)      201 2023-11-30 19:27:51.000000 meditability-0.2.1/src/smk/config/cluster.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)     2473 2023-12-08 17:42:34.000000 meditability-0.2.1/src/smk/config/guide_prediction_default_template.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)     2227 2023-12-11 19:17:26.000000 meditability-0.2.1/src/smk/config/guide_prediction_private_template.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)      461 2023-09-25 22:32:19.000000 meditability-0.2.1/src/smk/config/hgvs_input.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)      281 2023-11-15 18:34:44.000000 meditability-0.2.1/src/smk/config/id_convert.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)       99 2023-12-12 00:29:02.000000 meditability-0.2.1/src/smk/config/medit_cluster.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)     1226 2024-02-06 00:40:47.000000 meditability-0.2.1/src/smk/config/medit_database.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)     1756 2024-01-31 20:38:51.000000 meditability-0.2.1/src/smk/config/medit_guide_pred.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)     1639 2023-11-29 23:36:47.000000 meditability-0.2.1/src/smk/config/preprocessing_configuration.yaml
-drwxr-xr-x   0 bellieny   (503) staff       (20)        0 2024-02-06 18:14:24.257180 meditability-0.2.1/src/smk/envs/
--rw-r--r--   0 bellieny   (503) staff       (20)        0 2024-01-10 17:53:11.000000 meditability-0.2.1/src/smk/envs/__init__.py
--rw-r--r--   0 bellieny   (503) staff       (20)     2233 2024-01-22 22:57:06.000000 meditability-0.2.1/src/smk/envs/backup_medit.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)     6513 2023-11-27 19:17:03.000000 meditability-0.2.1/src/smk/envs/bio.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)     1582 2023-10-03 16:53:49.000000 meditability-0.2.1/src/smk/envs/casoff.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)      221 2023-09-05 15:56:46.000000 meditability-0.2.1/src/smk/envs/clinvar_pull.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)     1363 2023-09-25 16:41:10.000000 meditability-0.2.1/src/smk/envs/gdown.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)     2289 2024-01-25 18:39:00.000000 meditability-0.2.1/src/smk/envs/medit.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)      564 2024-01-17 18:04:18.000000 meditability-0.2.1/src/smk/envs/samtools.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)     2266 2024-01-22 21:59:06.000000 meditability-0.2.1/src/smk/envs/test_medit.yaml
--rw-r--r--   0 bellieny   (503) staff       (20)     2533 2024-02-01 19:54:30.000000 meditability-0.2.1/src/smk/envs/vcf.yaml
-drwxr-xr-x   0 bellieny   (503) staff       (20)        0 2024-02-06 18:14:24.277669 meditability-0.2.1/src/smk/pipelines/
--rw-r--r--   0 bellieny   (503) staff       (20)      123 2024-01-10 17:53:11.000000 meditability-0.2.1/src/smk/pipelines/__init__.py
--rw-r--r--   0 bellieny   (503) staff       (20)     3053 2024-01-10 17:53:11.000000 meditability-0.2.1/src/smk/pipelines/compression_routine.smk
--rw-r--r--   0 bellieny   (503) staff       (20)     1242 2024-01-10 17:53:11.000000 meditability-0.2.1/src/smk/pipelines/filename_standardization.smk
--rw-r--r--   0 bellieny   (503) staff       (20)     7213 2024-01-25 18:39:00.000000 meditability-0.2.1/src/smk/pipelines/guide_prediction.smk
--rw-r--r--   0 bellieny   (503) staff       (20)      543 2024-01-10 17:53:11.000000 meditability-0.2.1/src/smk/pipelines/offtarget_prediction.smk
-drwxr-xr-x   0 bellieny   (503) staff       (20)        0 2024-02-06 18:14:24.319924 meditability-0.2.1/src/smk/pipelines/py/
--rw-r--r--   0 bellieny   (503) staff       (20)        0 2024-01-17 18:04:18.000000 meditability-0.2.1/src/smk/pipelines/py/__init__.py
--rw-r--r--   0 bellieny   (503) staff       (20)    12717 2024-01-23 20:04:07.000000 meditability-0.2.1/src/smk/pipelines/py/annotate.py
--rw-r--r--   0 bellieny   (503) staff       (20)     2342 2024-01-17 18:04:18.000000 meditability-0.2.1/src/smk/pipelines/py/aws_pull.py
--rw-r--r--   0 bellieny   (503) staff       (20)     7717 2024-01-17 18:04:18.000000 meditability-0.2.1/src/smk/pipelines/py/clinVar_pull.py
--rw-r--r--   0 bellieny   (503) staff       (20)    15845 2024-01-23 21:59:34.000000 meditability-0.2.1/src/smk/pipelines/py/dataH.py
--rw-r--r--   0 bellieny   (503) staff       (20)    14046 2024-01-17 18:04:18.000000 meditability-0.2.1/src/smk/pipelines/py/featurization.py
--rw-r--r--   0 bellieny   (503) staff       (20)    18270 2024-01-24 00:23:49.000000 meditability-0.2.1/src/smk/pipelines/py/fetchGuides.py
--rw-r--r--   0 bellieny   (503) staff       (20)    19564 2024-01-23 23:18:53.000000 meditability-0.2.1/src/smk/pipelines/py/find_offtargets.py
--rw-r--r--   0 bellieny   (503) staff       (20)     4278 2024-01-17 18:04:18.000000 meditability-0.2.1/src/smk/pipelines/py/gdrive_import.py
--rw-r--r--   0 bellieny   (503) staff       (20)     3658 2024-01-17 18:04:18.000000 meditability-0.2.1/src/smk/pipelines/py/genome_seq_search.py
--rw-r--r--   0 bellieny   (503) staff       (20)    14903 2024-01-17 18:04:18.000000 meditability-0.2.1/src/smk/pipelines/py/make_tables.py
--rw-r--r--   0 bellieny   (503) staff       (20)     5481 2024-02-05 19:27:34.000000 meditability-0.2.1/src/smk/pipelines/py/ncbi_cross_database.py
--rw-r--r--   0 bellieny   (503) staff       (20)    11692 2024-01-25 18:39:00.000000 meditability-0.2.1/src/smk/pipelines/py/process_genome.py
--rw-r--r--   0 bellieny   (503) staff       (20)    11388 2024-01-23 21:59:34.000000 meditability-0.2.1/src/smk/pipelines/py/scoring.py
--rw-r--r--   0 bellieny   (503) staff       (20)    17166 2024-01-17 18:04:18.000000 meditability-0.2.1/src/smk/pipelines/py/validate.py
--rw-r--r--   0 bellieny   (503) staff       (20)     3701 2024-01-10 17:53:11.000000 meditability-0.2.1/src/smk/pipelines/vcf_processing.smk
+drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.772370 meditability-0.2.2/
+-rw-r--r--   0 bellieny   (501) staff       (20)    32337 2024-01-30 21:30:29.000000 meditability-0.2.2/LICENSE
+-rw-r--r--   0 bellieny   (501) staff       (20)      558 2024-04-01 18:06:59.768252 meditability-0.2.2/PKG-INFO
+-rw-r--r--   0 bellieny   (501) staff       (20)     3621 2024-02-16 18:08:11.000000 meditability-0.2.2/README.md
+-rw-r--r--   0 bellieny   (501) staff       (20)       38 2024-04-01 18:06:59.772450 meditability-0.2.2/setup.cfg
+-rw-r--r--   0 bellieny   (501) staff       (20)     1018 2024-03-13 00:31:40.000000 meditability-0.2.2/setup.py
+drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.369024 meditability-0.2.2/src/
+drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.766007 meditability-0.2.2/src/meditability.egg-info/
+-rw-r--r--   0 bellieny   (501) staff       (20)      558 2024-04-01 18:06:58.000000 meditability-0.2.2/src/meditability.egg-info/PKG-INFO
+-rw-r--r--   0 bellieny   (501) staff       (20)     2121 2024-04-01 18:06:59.000000 meditability-0.2.2/src/meditability.egg-info/SOURCES.txt
+-rw-r--r--   0 bellieny   (501) staff       (20)        1 2024-04-01 18:06:58.000000 meditability-0.2.2/src/meditability.egg-info/dependency_links.txt
+-rw-r--r--   0 bellieny   (501) staff       (20)       36 2024-04-01 18:06:58.000000 meditability-0.2.2/src/meditability.egg-info/entry_points.txt
+-rw-r--r--   0 bellieny   (501) staff       (20)      148 2024-04-01 18:06:58.000000 meditability-0.2.2/src/meditability.egg-info/requires.txt
+-rw-r--r--   0 bellieny   (501) staff       (20)        9 2024-04-01 18:06:58.000000 meditability-0.2.2/src/meditability.egg-info/top_level.txt
+drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.506374 meditability-0.2.2/src/prog/
+-rw-r--r--   0 bellieny   (501) staff       (20)       24 2024-01-12 17:32:35.000000 meditability-0.2.2/src/prog/__init__.py
+-rw-r--r--   0 bellieny   (501) staff       (20)    11022 2024-04-01 18:00:41.000000 meditability-0.2.2/src/prog/arguments.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     5602 2024-02-16 18:08:11.000000 meditability-0.2.2/src/prog/db_set.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     6932 2024-04-01 18:00:41.000000 meditability-0.2.2/src/prog/guide_prediction.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     1144 2024-04-01 18:00:41.000000 meditability-0.2.2/src/prog/list_editors.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     1037 2024-02-16 23:52:11.000000 meditability-0.2.2/src/prog/mEdit.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     7693 2024-04-01 18:00:41.000000 meditability-0.2.2/src/prog/medit_lib.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     4968 2024-04-01 18:00:41.000000 meditability-0.2.2/src/prog/offtarget_prediction.py
+drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.508356 meditability-0.2.2/src/smk/
+-rw-r--r--   0 bellieny   (501) staff       (20)        0 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/__init__.py
+drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.568907 meditability-0.2.2/src/smk/config/
+-rw-r--r--   0 bellieny   (501) staff       (20)        0 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/__init__.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     2209 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/aws_download.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)      469 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/caspedia_ingest.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)      201 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/cluster.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)     2473 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/guide_prediction_default_template.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)     2227 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/guide_prediction_private_template.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)      461 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/hgvs_input.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)      281 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/id_convert.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)       99 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/medit_cluster.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)     1226 2024-02-16 18:08:11.000000 meditability-0.2.2/src/smk/config/medit_database.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)     1841 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/config/medit_guide_pred.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)      613 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/config/medit_offtarget.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)     1639 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/preprocessing_configuration.yaml
+drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.628584 meditability-0.2.2/src/smk/envs/
+-rw-r--r--   0 bellieny   (501) staff       (20)        0 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/envs/__init__.py
+-rw-r--r--   0 bellieny   (501) staff       (20)      692 2024-01-12 18:02:39.000000 meditability-0.2.2/src/smk/envs/b_medit.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)     1582 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/envs/casoff.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)      221 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/envs/clinvar_pull.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)     1363 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/envs/gdown.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)     2289 2024-01-24 21:43:26.000000 meditability-0.2.2/src/smk/envs/medit.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)      564 2024-01-17 02:04:41.000000 meditability-0.2.2/src/smk/envs/samtools.yaml
+-rw-r--r--   0 bellieny   (501) staff       (20)     2533 2024-02-16 18:08:11.000000 meditability-0.2.2/src/smk/envs/vcf.yaml
+drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.660987 meditability-0.2.2/src/smk/pipelines/
+-rw-r--r--   0 bellieny   (501) staff       (20)      123 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/pipelines/__init__.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     3053 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/pipelines/compression_routine.smk
+-rw-r--r--   0 bellieny   (501) staff       (20)     1242 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/pipelines/filename_standardization.smk
+-rw-r--r--   0 bellieny   (501) staff       (20)     7280 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/pipelines/guide_prediction.smk
+-rw-r--r--   0 bellieny   (501) staff       (20)     5660 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/pipelines/offtarget_prediction.smk
+drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.759505 meditability-0.2.2/src/smk/pipelines/py/
+-rw-r--r--   0 bellieny   (501) staff       (20)        0 2024-01-12 00:46:24.000000 meditability-0.2.2/src/smk/pipelines/py/__init__.py
+-rw-r--r--   0 bellieny   (501) staff       (20)    12717 2024-01-23 20:04:30.000000 meditability-0.2.2/src/smk/pipelines/py/annotate.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     2342 2023-10-03 00:05:02.000000 meditability-0.2.2/src/smk/pipelines/py/aws_pull.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     5963 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/pipelines/py/build_casoff_input.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     4266 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/pipelines/py/build_casoff_output.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     7717 2023-11-02 16:12:49.000000 meditability-0.2.2/src/smk/pipelines/py/clinVar_pull.py
+-rw-r--r--   0 bellieny   (501) staff       (20)    17522 2024-04-01 18:00:42.000000 meditability-0.2.2/src/smk/pipelines/py/dataH.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     4373 2024-02-27 07:13:06.000000 meditability-0.2.2/src/smk/pipelines/py/deepcas_models.py
+-rw-r--r--   0 bellieny   (501) staff       (20)      581 2024-02-01 17:56:08.000000 meditability-0.2.2/src/smk/pipelines/py/fasta_chromosome_rename.py
+-rw-r--r--   0 bellieny   (501) staff       (20)    14046 2024-01-11 00:35:10.000000 meditability-0.2.2/src/smk/pipelines/py/featurization.py
+-rw-r--r--   0 bellieny   (501) staff       (20)    19981 2024-04-01 18:00:42.000000 meditability-0.2.2/src/smk/pipelines/py/fetchGuides.py
+-rw-r--r--   0 bellieny   (501) staff       (20)    19745 2024-02-16 23:52:11.000000 meditability-0.2.2/src/smk/pipelines/py/find_offtargets.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     4278 2023-09-27 16:24:56.000000 meditability-0.2.2/src/smk/pipelines/py/gdrive_import.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     3658 2023-10-16 17:01:06.000000 meditability-0.2.2/src/smk/pipelines/py/genome_seq_search.py
+-rw-r--r--   0 bellieny   (501) staff       (20)    16732 2024-03-12 23:53:04.000000 meditability-0.2.2/src/smk/pipelines/py/make_tables.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     5481 2024-02-16 18:08:11.000000 meditability-0.2.2/src/smk/pipelines/py/ncbi_cross_database.py
+-rw-r--r--   0 bellieny   (501) staff       (20)    12063 2024-02-27 07:13:06.000000 meditability-0.2.2/src/smk/pipelines/py/process_genome.py
+-rw-r--r--   0 bellieny   (501) staff       (20)    14218 2024-02-22 04:49:22.000000 meditability-0.2.2/src/smk/pipelines/py/scoring.py
+-rw-r--r--   0 bellieny   (501) staff       (20)    17166 2023-10-23 21:12:40.000000 meditability-0.2.2/src/smk/pipelines/py/validate.py
+-rw-r--r--   0 bellieny   (501) staff       (20)     3701 2024-01-31 16:49:32.000000 meditability-0.2.2/src/smk/pipelines/vcf_processing.smk
```

### Comparing `meditability-0.2.1/LICENSE` & `meditability-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/PKG-INFO` & `meditability-0.2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meditability
-Version: 0.2.1
+Version: 0.2.2
 Author: Interventional Genomics Unit
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 License-File: LICENSE
 Requires-Dist: snakemake>=7.32.4
```

### Comparing `meditability-0.2.1/README.md` & `meditability-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/setup.py` & `meditability-0.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # == Installed Modules
 from setuptools import setup, find_packages
 # == Project Modules
 
 
 setup(
     name='meditability',
-    version='0.2.1',
+    version='0.2.2',
     description='',
     author='Interventional Genomics Unit',
     author_email='',
     entry_points={
         "console_scripts": [
             "medit = prog:main"
         ]
```

### Comparing `meditability-0.2.1/src/meditability.egg-info/PKG-INFO` & `meditability-0.2.2/src/meditability.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meditability
-Version: 0.2.1
+Version: 0.2.2
 Author: Interventional Genomics Unit
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 License-File: LICENSE
 Requires-Dist: snakemake>=7.32.4
```

### Comparing `meditability-0.2.1/src/meditability.egg-info/SOURCES.txt` & `meditability-0.2.2/src/meditability.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,48 +10,52 @@
 src/prog/__init__.py
 src/prog/arguments.py
 src/prog/db_set.py
 src/prog/guide_prediction.py
 src/prog/list_editors.py
 src/prog/mEdit.py
 src/prog/medit_lib.py
+src/prog/offtarget_prediction.py
 src/smk/__init__.py
 src/smk/config/__init__.py
 src/smk/config/aws_download.yaml
 src/smk/config/caspedia_ingest.yaml
 src/smk/config/cluster.yaml
 src/smk/config/guide_prediction_default_template.yaml
 src/smk/config/guide_prediction_private_template.yaml
 src/smk/config/hgvs_input.yaml
 src/smk/config/id_convert.yaml
 src/smk/config/medit_cluster.yaml
 src/smk/config/medit_database.yaml
 src/smk/config/medit_guide_pred.yaml
+src/smk/config/medit_offtarget.yaml
 src/smk/config/preprocessing_configuration.yaml
 src/smk/envs/__init__.py
-src/smk/envs/backup_medit.yaml
-src/smk/envs/bio.yaml
+src/smk/envs/b_medit.yaml
 src/smk/envs/casoff.yaml
 src/smk/envs/clinvar_pull.yaml
 src/smk/envs/gdown.yaml
 src/smk/envs/medit.yaml
 src/smk/envs/samtools.yaml
-src/smk/envs/test_medit.yaml
 src/smk/envs/vcf.yaml
 src/smk/pipelines/__init__.py
 src/smk/pipelines/compression_routine.smk
 src/smk/pipelines/filename_standardization.smk
 src/smk/pipelines/guide_prediction.smk
 src/smk/pipelines/offtarget_prediction.smk
 src/smk/pipelines/vcf_processing.smk
 src/smk/pipelines/py/__init__.py
 src/smk/pipelines/py/annotate.py
 src/smk/pipelines/py/aws_pull.py
+src/smk/pipelines/py/build_casoff_input.py
+src/smk/pipelines/py/build_casoff_output.py
 src/smk/pipelines/py/clinVar_pull.py
 src/smk/pipelines/py/dataH.py
+src/smk/pipelines/py/deepcas_models.py
+src/smk/pipelines/py/fasta_chromosome_rename.py
 src/smk/pipelines/py/featurization.py
 src/smk/pipelines/py/fetchGuides.py
 src/smk/pipelines/py/find_offtargets.py
 src/smk/pipelines/py/gdrive_import.py
 src/smk/pipelines/py/genome_seq_search.py
 src/smk/pipelines/py/make_tables.py
 src/smk/pipelines/py/ncbi_cross_database.py
```

### Comparing `meditability-0.2.1/src/prog/arguments.py` & `meditability-0.2.2/src/prog/arguments.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def parse_arguments():
 	# -> === Launch argparse parser === <-
 	parser = argp(
 		prog='mEdit',
 		description=f'version {version("meditability")}',
 		# epilog="mEdit is pretty cool, huh? :)",
-		usage='%(prog)s [options]',
+		usage='%(prog)s ',
 		formatter_class=RawTextHelpFormatter
 	)
 
 	programs = parser.add_subparsers(
 		title="== mEdit Programs ==",
 		description=textwrap.dedent('''
 		mEdit can be operated through a list of different programs.'''),
@@ -32,15 +32,15 @@
 	ref_db_parse = dbset_parser.add_argument_group("== Reference Database Pre-Processing ==")
 	ref_db_parse.add_argument('-d',
 							  dest='db_path',
 							  default='.',
 							  help=textwrap.dedent('''
 	                          Provide the path where the "mEdit_database" 
 	                          directory will be created ahead of the analysis.
-	                          Requires ~6.5GB in-disk storage 
+	                          Requires ~3.2GB in-disk storage 
 	                          [default: ./mEdit_database]'''))
 	ref_db_parse.add_argument('-l',
 							  dest='latest_reference',
 							  action='store_true',
 							  help=textwrap.dedent('''
 							  Request the latest human genome reference as part
 							  of mEdit database unpacking. This is especially 
@@ -48,15 +48,15 @@
 							  genome assemblies. [default: False]'''))
 	ref_db_parse.add_argument('-c',
 							  dest='custom_reference',
 							  help=textwrap.dedent('''
 							  Provide the path to a custom human reference genome 
 							  in FASTA format. ***Chromosome annotation must follow a
 							    ">chrN" format (case sensitive)'''))
-	ref_db_parse.add_argument('-p',
+	ref_db_parse.add_argument('-t',
 							  dest='threads',
 							  default='1',
 							  help=textwrap.dedent('''
 	                          Provide the number of cores for parallel decompression
 	                          of mEdit databases.
 	                          '''))
 
@@ -73,26 +73,26 @@
 							  default='.',
 							  help=textwrap.dedent('''
 	                          Provide the path where the "mEdit_database"
 	                          directory was created ahead of the analysis
 	                          using the "db_set" program.
 	                          [default: ./mEdit_database]''')
 							  )
-	editors_list.add_argument('-e',
-							  dest='editors',
-							  action='store_true',
-							  help=textwrap.dedent('''
-	                          Provides the current list of available editors on mEdit
-	                           '''))
-	editors_list.add_argument('-b',
-							  dest='base_editors',
-							  action='store_true',
-							  help=textwrap.dedent('''
-	                          Provides the current list of available base editors on mEdit 
-	                          '''))
+	# editors_list.add_argument(('--editors'),
+	# 						  dest='editors',
+	# 						  action='store_true',
+	# 						  help=textwrap.dedent('''
+	#                           Provides the current list of available editors on mEdit
+	#                            '''))
+	# editors_list.add_argument('-b',
+	# 						  dest='base_editors',
+	# 						  action='store_true',
+	# 						  help=textwrap.dedent('''
+	#                           Provides the current list of available base editors on mEdit
+	#                           '''))
 
 	# === Guide Prediction Program ===
 	fguides_parser = programs.add_parser(
 		'guide_prediction',
 		help=textwrap.dedent('''
 			The core mEdit program finds potential guides for
 			variants specified on the input by searching a diverse set of
@@ -192,14 +192,23 @@
 		choices=['off', 'default', 'custom', 'user defined list'],
 		default='default',
 		help=textwrap.dedent('''
 			Add this flag to make mEdit process base-editors. 
 			[default = off]''')
 	)
 	run_params.add_argument(
+		'--cutdist',
+		dest='cutdist',
+		default='7',
+		help=textwrap.dedent('''
+				Max allowable window a variant start position can be from
+				the editor cut site. This option not available for base editors. 
+				[default = 7]''')
+	)
+	run_params.add_argument(
 		'--dry',
 		dest='dry_run',
 		action='store_true',
 		help=textwrap.dedent('''
 			Perform a dry run of mEdit.'''))
 	cluster_opt = fguides_parser.add_argument_group("== SLURM Options ==")
 	cluster_opt.add_argument(
@@ -227,19 +236,92 @@
 		help=textwrap.dedent('''
 			Specify the maximum amount of time allowed for each parallel job.
 			Format example: 2 hours -> "2:00:00" [default = 1 hour]''')
 	)
 
 	# === Off Target Effect Program ===
 	casoff_parser = programs.add_parser(
-		'offtargets',
+		'offtarget',
 		help=textwrap.dedent('''
 			Predict off-target effect for the guides found'''),
 		formatter_class=RawTextHelpFormatter
 	)
 	offtarget_params = casoff_parser.add_argument_group("== Off-Target Parameters ==")
 	offtarget_params.add_argument(
-		'-r', help='Reference Genome')
+		'--dry',
+		dest='dry_run',
+		action='store_true',
+		help=textwrap.dedent('''
+				Perform a dry run of mEdit.'''))
+
+	off_in_out = casoff_parser.add_argument_group("== Input/Output Options ==")
+	off_in_out.add_argument(
+		'-o',
+		dest='output',
+		default='medit_analysis',
+		help=textwrap.dedent('''
+		Path to root directory where mEdit guide_prediction
+		 outputs were stored. "medit offtarget" can't 
+		 operate if this path is incorrect. [default: mEdit_analysis_<jobtag>/]
+		 ''')
+	)
+	off_in_out.add_argument('-d',
+							dest='db_path',
+							default='.',
+							help=textwrap.dedent('''
+		                    Provide the path where the "mEdit_database" 
+		                    directory was created ahead of the analysis 
+		                    using the "db_set" program. 
+		                    [default: ./mEdit_database]''')
+							)
+	off_in_out.add_argument('-j',
+							dest='jobtag',
+							required=True,
+							help=textwrap.dedent('''
+							Provide the tag associated with the desired 
+							"medit guide_prediction" job ID.
+							"mEdit offtarget" will use the path from the
+							 OUTPUT option to access this JOBTAG.
+							''')
+							)
+	off_in_out.add_argument('--select_editors',
+							dest='select_editors',
+							default='',
+							help=textwrap.dedent('''
+								Provide a comma-separated list to select which 
+								editors should be analyzed for offtarget effect.
+								[default: all] 
+								''')
+							)
+
+	off_cluster_opt = casoff_parser.add_argument_group("== SLURM Options ==")
+	off_cluster_opt.add_argument(
+		'-p',
+		dest='parallel_processes',
+		help=textwrap.dedent('''
+					Most processes in mEdit can be submitted to SLURM.
+					When submitting mEdit jobs to SLURM, the user can specify
+					the number of parallel processes that will be sent to the 
+					server [default = 1]''')
+	)
+	off_cluster_opt.add_argument(
+		'--ncores',
+		dest='ncores',
+		default=2,
+		help=textwrap.dedent('''
+				Specify the number of cores through which each parallel process 
+				will be computed. [default = 2]''')
+	)
+
+	off_cluster_opt.add_argument(
+		'--maxtime',
+		dest='maxtime',
+		default='1:00:00',
+		help=textwrap.dedent('''
+				Specify the maximum amount of time allowed for each parallel job.
+				Format example: 2 hours -> "2:00:00" [default = 1 hour]''')
+	)
+	# TODO: Finish the other options at the user interface
 
 	# Parse arguments from the command line
 	arguments = parser.parse_args()
 	return arguments
```

### Comparing `meditability-0.2.1/src/prog/db_set.py` & `meditability-0.2.2/src/prog/db_set.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/prog/guide_prediction.py` & `meditability-0.2.2/src/prog/guide_prediction.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 	root_dir = abspath(args.output)
 	db_path_full = f"{abspath(args.db_path)}/medit_database"
 	mode = args.mode
 	private_genomes = args.private_genome
 	qtype = args.qtype_request
 	editor_request = parse_editor_request(args.editor_request)
 	be_request = parse_editor_request(args.be_request)
+	cutdist = args.cutdist
 
 	# == Load SLURM-related values ==
 	ncores = args.ncores
 	maxtime = args.maxtime
 	parallel_processes = args.parallel_processes
 	dry_run = args.dry_run
 
@@ -95,14 +96,15 @@
 	config_template['processing_mode'] = mode
 	config_template['output_directory'] = root_dir
 	config_template['variant_query_dir'] = query_input
 	# Assign run parameters to config
 	config_template['qtype'] = qtype
 	config_template['editor_request'] = editor_request
 	config_template['be_request'] = be_request
+	config_template['distance_from_cutsite'] = cutdist
 	# Assign cluster options
 	cluster_template['__default__']['cores'] = ncores
 	cluster_template['__default__']['time'] = maxtime
 
 	# ->=== PRIVATE GENOME RUN ===<-
 	# == Check run mode ==
 	if mode == 'private':
```

### Comparing `meditability-0.2.1/src/prog/list_editors.py` & `meditability-0.2.2/src/prog/list_editors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # == Native Modules
 import pickle
-from os.path import abspath
+from os.path import abspath, isdir
 # == Installed Modules
 import yaml
 # == Project Modules
 
 
 def ls_editors(args):
 	# == Load Run Parameters values ==
-	print_editors = args.editors
-	print_base_editors = args.base_editors
+	# print_editors = args.editors
+	# print_base_editors = args.base_editors
 
 	# === Load Database Path ===
 	db_path_full = f"{abspath(args.db_path)}/medit_database"
 	config_db_path = f"{db_path_full}/config_db/config_db.yaml"
 
+	if not isdir(db_path_full):
+		raise f"The database path {db_path_full} is not a directory."
+
 	# === Load configuration file ===
 	with open(config_db_path, 'r') as config_handle:
 		config_db_obj = yaml.safe_load(config_handle)
 
 	# === Load Editors Lists From Path Specified on config_db.yaml ===
-	if print_editors:
-		with open(str(config_db_obj["editors"]), 'rb') as editors_pkl_handle:
-			editors_dict = pickle.load(editors_pkl_handle)
-			print(f"Available editors:\n {list(editors_dict['clinical'].keys())}")
-	if print_base_editors:
-		with open(str(config_db_obj["base_editors"]), 'rb') as be_pkl_handle:
-			base_editors_dict = pickle.load(be_pkl_handle)
-			print(f"Available base editors:\n {list(base_editors_dict['all'].keys())}")
+	# if print_editors:
+	with open(str(config_db_obj["editors"]), 'rb') as editors_pkl_handle:
+		editors_dict = pickle.load(editors_pkl_handle)
+		print(f"Available editors:\n {list(editors_dict['clinical'].keys())}")
+	# if print_base_editors:
+	with open(str(config_db_obj["base_editors"]), 'rb') as be_pkl_handle:
+		base_editors_dict = pickle.load(be_pkl_handle)
+		print(f"Available base editors:\n {list(base_editors_dict['all'].keys())}")
```

### Comparing `meditability-0.2.1/src/prog/medit_lib.py` & `meditability-0.2.2/src/prog/medit_lib.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 import secrets
 import string
 import pytz
 import os
 import os.path
 import re
 import pathlib
+from pathlib import Path
 import pickle
 # == Installed Modules ==
 from alive_progress import alive_bar
 import yaml
 from importlib_resources import files
 from Bio import SeqIO
 import boto3
 from botocore.exceptions import NoCredentialsError
+import pandas as pd
 # == Project Modules ==
 
 
 def compress_file(file_path: str):
 	if not is_gzipped(file_path):
 		# If not gzipped, compress the file
 		with open(file_path, 'rb') as f_in, gzip.open(file_path + '.gz', 'wb') as f_out:
@@ -83,18 +85,42 @@
 				bar()
 				continue
 			pathlib.Path(destination_path).mkdir(parents=True, exist_ok=True)
 			s3.download_file(s3_bucket_name, key, destination_file)
 			bar()
 
 
+def export_guides_by_editor(guide_df_by_editor_dict: dict, output_dir: (str, Path)):
+	editors_list = []
+	for editor in guide_df_by_editor_dict:
+		editors_list.append(editor)
+		guide_df = pd.DataFrame(guide_df_by_editor_dict[editor][0])
+		filepath = f"{output_dir}/{editor}.pkl"
+		# Create output directory if non-existent
+		set_export(output_dir)
+		with open(filepath, 'wb') as guide_df_handle:
+			pickle.dump(guide_df, guide_df_handle)
+	return editors_list
+
+
 def file_exists(file_path):
 	return os.path.exists(file_path)
 
 
+def group_guide_table(guide_table_path: pathlib.Path, editor_filter: (list, str)):
+	guides_df = pd.read_csv(guide_table_path)
+	if editor_filter:
+		guides_df = guides_df[guides_df['Editor'].isin(editor_filter)]
+	grouped_guides_df = guides_df.groupby('Editor')
+	editor_expanded_dictionary = {}
+	for editor, stats in grouped_guides_df:
+		editor_expanded_dictionary.setdefault(editor, []).append(stats)
+	return editor_expanded_dictionary
+
+
 def handle_shell_exception(subprocess_result, shell_command, verbose: bool):
 	# === Handle SMK exceptions through subprocess
 	#   == Unlock directory if necessary for SMK run
 	if re.findall("Directory cannot be locked.", subprocess_result.stdout):
 		print("--> Target directory locked. Unlocking...")
 		unlock_smk_command = f"{shell_command} --unlock"
 		launch_shell_cmd(unlock_smk_command, verbose)
@@ -195,15 +221,16 @@
 	:return:
 	"""
 	return str(files(path_from_toplevel).joinpath(filename))
 
 
 def set_export(outdir: str):
 	if os.path.exists(outdir):
-		print(f'--> Skipping directory creation: {outdir}')
+		pass
+		# print(f'--> Skipping directory creation: {outdir}')
 	# Create outdir only if it doesn't exist
 	if not os.path.exists(outdir):
 		print(f'Directory created on: {outdir}')
 		pathlib.Path(outdir).mkdir(parents=True, exist_ok=True)
 	return outdir
```

### Comparing `meditability-0.2.1/src/smk/config/aws_download.yaml` & `meditability-0.2.2/src/smk/config/aws_download.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/config/guide_prediction_default_template.yaml` & `meditability-0.2.2/src/smk/config/guide_prediction_default_template.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/config/guide_prediction_private_template.yaml` & `meditability-0.2.2/src/smk/config/guide_prediction_private_template.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/config/medit_database.yaml` & `meditability-0.2.2/src/smk/config/medit_database.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/config/medit_guide_pred.yaml` & `meditability-0.2.2/src/smk/config/medit_guide_pred.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 # ::date+time:: -> YYMMDDHHMMSSf
 # ::random alphanumeric:: -> 9m7aQ0KRZx
 run_name: ""
 # Must be the same as specified for the run_name
 processing_mode: ""
 
 # == RUN PARAMETERS ==
+# Any applicable defaults are defined at prog/arguments.py
 qtype: ""
 be_request: ""
 editor_request: ""
+distance_from_cutsite: ""
 
 # === I/O PATHS ===
 # == DIRECTORIES ==
 # Directory that holds the query HGVSs
 variant_query_dir: ""
 
 # Parent database folder
```

### Comparing `meditability-0.2.1/src/smk/config/preprocessing_configuration.yaml` & `meditability-0.2.2/src/smk/config/preprocessing_configuration.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/envs/backup_medit.yaml` & `meditability-0.2.2/src/smk/envs/vcf.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-name: medit
+name: vcf
 channels:
   - conda-forge
+  - bioconda
 dependencies:
+  - _libgcc_mutex=0.1
+  - _openmp_mutex=4.5
   - absl-py=2.0.0
   - aiohttp=3.9.1
   - aiosignal=1.3.1
   - astunparse=1.6.3
   - attrs=23.2.0
+  - biopython=1.83
   - blinker=1.7.0
   - brotli-python=1.1.0
   - bzip2=1.0.8
   - c-ares=1.25.0
   - ca-certificates=2023.11.17
   - cached-property=1.5.2
   - cached_property=1.5.2
@@ -30,63 +34,74 @@
   - grpcio=1.59.3
   - h5py=3.10.0
   - hdf5=1.14.3
   - icu=73.2
   - idna=3.6
   - importlib-metadata=7.0.1
   - keras=2.15.0
+  - keyutils=1.6.1
   - krb5=1.21.2
+  - ld_impl_linux-64=2.40
   - libabseil=20230802.1
   - libaec=1.1.2
   - libblas=3.9.0
   - libcblas=3.9.0
   - libcurl=8.5.0
-  - libcxx=16.0.6
   - libedit=3.1.20191231
   - libev=4.33
   - libexpat=2.5.0
   - libffi=3.4.2
+  - libgcc-ng=13.2.0
+  - libgfortran-ng=13.2.0
+  - libgfortran5=13.2.0
+  - libgomp=13.2.0
   - libgrpc=1.59.3
   - libjpeg-turbo=3.0.0
   - liblapack=3.9.0
   - libnghttp2=1.58.0
+  - libnsl=2.0.1
   - libopenblas=0.3.25
   - libpng=1.6.39
   - libprotobuf=4.24.4
   - libre2-11=2023.06.02
   - libsqlite=3.44.2
   - libssh2=1.11.0
+  - libstdcxx-ng=13.2.0
+  - libuuid=2.38.1
+  - libxcrypt=4.4.36
   - libzlib=1.2.13
-  - llvm-openmp=17.0.6
   - markdown=3.5.2
   - markupsafe=2.1.3
   - ml_dtypes=0.2.0
   - multidict=6.0.4
   - ncurses=6.4
   - numpy=1.26.3
   - oauthlib=3.2.2
-  - openssl=3.2.0
+#  - openssl=3.2.0
+  - openssl=3.2.1
   - opt_einsum=3.3.0
   - packaging=23.2
-  - pandas=2.1.4
+  - pandas=2.2.0
   - pip=23.3.2
   - protobuf=4.24.4
   - pyasn1=0.5.1
   - pyasn1-modules=0.3.0
   - pycparser=2.21
   - pyjwt=2.8.0
   - pyopenssl=23.3.0
+  - pysam=0.22.0
   - pysocks=1.7.1
-  - python=3.11.7
+  - python=3.10.13
   - python-dateutil=2.8.2
   - python-flatbuffers=23.5.26
   - python-tzdata=2023.4
-  - python_abi=3.11
+#  - python_abi=3.11
   - pytz=2023.3.post1
   - pyu2f=0.1.5
+  - pyvcf=0.6.8
   - re2=2023.06.02
   - readline=8.2
   - requests=2.31.0
   - requests-oauthlib=1.3.1
   - rsa=4.9
   - setuptools=69.0.3
   - six=1.16.0
@@ -104,8 +119,8 @@
   - werkzeug=3.0.1
   - wheel=0.42.0
   - wrapt=1.14.1
   - xz=5.2.6
   - yarl=1.9.3
   - zipp=3.17.0
   - zstd=1.5.5
-prefix: /Users/bellieny/miniconda3/envs/medit
+prefix: /home/danielbr/miniconda3/envs/vcf
```

### Comparing `meditability-0.2.1/src/smk/envs/casoff.yaml` & `meditability-0.2.2/src/smk/envs/casoff.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 name: casoff
 channels:
-  - bioconda
   - conda-forge
+  - bioconda
   - defaults
 dependencies:
   - _libgcc_mutex=0.1
   - _openmp_mutex=4.5
   - biopython=1.81
   - bzip2=1.0.8
   - c-ares=1.19.1
```

### Comparing `meditability-0.2.1/src/smk/envs/gdown.yaml` & `meditability-0.2.2/src/smk/envs/gdown.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/envs/medit.yaml` & `meditability-0.2.2/src/smk/envs/medit.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/envs/samtools.yaml` & `meditability-0.2.2/src/smk/envs/samtools.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/pipelines/compression_routine.smk` & `meditability-0.2.2/src/smk/pipelines/compression_routine.smk`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/pipelines/filename_standardization.smk` & `meditability-0.2.2/src/smk/pipelines/filename_standardization.smk`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/pipelines/guide_prediction.smk` & `meditability-0.2.2/src/smk/pipelines/guide_prediction.smk`

 * *Files 8% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 rule all:
 	input:
 		# With the relevant VCF downloaded, proceed with creating consensus FASTA
 		expand("{meditdb_path}/{mode}/consensus_refs/{sequence_id}/{vcf_id}.fa",
 			meditdb_path=config["meditdb_path"],mode=config["processing_mode"],
 			vcf_id=config["vcf_id"],sequence_id=config["sequence_id"]),
 		# Predicted guides using the most recent human genome assembly
-		expand("{root_dir}/{mode}/jobs/{job_name}/guide_prediction-{sequence_id}/guides_report_ref/Guides_found.csv",
+		expand("{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/guides_report_ref/Guides_found.csv",
 			root_dir=config["output_directory"], mode=config["processing_mode"],
-			job_name=config["run_name"], sequence_id=config["sequence_id"]),
+			run_name=config["run_name"], sequence_id=config["sequence_id"]),
 		# Predicted guides on alternative genomes based on the reference listed above
-		expand("{root_dir}/{mode}/jobs/{job_name}/guide_prediction-{sequence_id}/guides_report_{vcf_id}/Guide_differences.csv",
+		expand("{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/guides_report_{vcf_id}/Guide_differences.csv",
 			root_dir=config["output_directory"],mode=config["processing_mode"],
-			job_name=config["run_name"],sequence_id=config["sequence_id"],
+			run_name=config["run_name"],sequence_id=config["sequence_id"],
 			vcf_id=config["vcf_id"])
 
 # noinspection SmkAvoidTabWhitespace
 rule consensus_fasta:
 	input:
 		assembly_path=lambda wildcards: glob.glob("{fasta_root_path}/{sequence_id}.fa.gz".format(
 			fasta_root_path=config["fasta_root_path"],sequence_id=wildcards.sequence_id)),
@@ -83,46 +83,47 @@
         """
 
 # noinspection SmkAvoidTabWhitespace
 rule predict_guides:
 	input:
 		query_manifest = lambda wildcards: glob.glob("{variant_query_dir}".format(
 			variant_query_dir=config["variant_query_dir"])),
-		assembly_path = lambda wildcards: glob.glob("{fasta_root_path}".format(
+		assembly_dir_path = lambda wildcards: glob.glob("{fasta_root_path}".format(
 			fasta_root_path=config["fasta_root_path"]))
 	output:
-		guides_report_out = "{root_dir}/{mode}/jobs/{job_name}/guide_prediction-{sequence_id}/guides_report_ref/Guides_found.csv",
-		guide_search_params = "{root_dir}/{mode}/jobs/{job_name}/guide_prediction-{sequence_id}/dynamic_params/guide_search_params.pkl",
-		snv_site_info = "{root_dir}/{mode}/jobs/{job_name}/guide_prediction-{sequence_id}/dynamic_params/snv_site_info.pkl"
+		guides_report_out = "{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/guides_report_ref/Guides_found.csv",
+		guide_search_params = "{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/dynamic_params/guide_search_params.pkl",
+		snv_site_info = "{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/dynamic_params/snv_site_info.pkl"
 	params:
 		# == Main output path
-		main_out = "{root_dir}/{mode}/jobs/{job_name}/guide_prediction-{sequence_id}/guides_report_ref",
+		main_out = "{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/guides_report_ref",
 		# == Main output filenames
 		gene_report = config["gene_report"],
 		variant_report = config["variant_report"],
 		be_report = config["be_report"],
 		# == Processed tables branch
 		support_tables = config["support_tables"],
 		annote_path = config["refseq_table"],
 		# == Editor Parameters
 		editors = config["editors"],
 		base_editors = config["base_editors"],
 		models_path= config["models_path"],
+		distance_from_cutsite = config["distance_from_cutsite"],
 		# == Run Parameters ==
 		qtype = config["qtype"],
 		be_request = config["be_request"],
 		editor_request = config["editor_request"]
 	conda:
 		"../envs/medit.yaml"
 	message:
 		"""
 # === PREDICT GUIDES ON REFERENCE GENOMES === #	
 Inputs used:
 --> Take variants from:\n {input.query_manifest}
---> Use reference assembly:\n {input.assembly_path}
+--> Use reference assembly:\n {input.assembly_dir_path}
 --> Support tables from:\n {params.support_tables}
 
 Run parameters:
 --> Query type: {params.qtype} 
 --> BEmode: {params.be_request}
 --> Editor scope: {params.editor_request}
 
@@ -137,24 +138,24 @@
 # noinspection SmkAvoidTabWhitespace
 rule process_altgenomes:
 	input:
 		filtered_vcf = lambda wildcards: glob.glob("{meditdb_path}/{mode}/consensus_refs/{sequence_id}/{vcf_id}.filtered.vcf.gz".format(
 			meditdb_path=config["meditdb_path"],mode=wildcards.mode,
 			vcf_id=wildcards.vcf_id,sequence_id=wildcards.sequence_id
 		)),
-		guides_report_out= "{root_dir}/{mode}/jobs/{job_name}/guide_prediction-{sequence_id}/guides_report_ref/Guides_found.csv",
-		guide_search_params= "{root_dir}/{mode}/jobs/{job_name}/guide_prediction-{sequence_id}/dynamic_params/guide_search_params.pkl",
-		snv_site_info= "{root_dir}/{mode}/jobs/{job_name}/guide_prediction-{sequence_id}/dynamic_params/snv_site_info.pkl"
+		guides_report_out= "{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/guides_report_ref/Guides_found.csv",
+		guide_search_params= "{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/dynamic_params/guide_search_params.pkl",
+		snv_site_info= "{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/dynamic_params/snv_site_info.pkl"
 	output:
-		diff_guides = "{root_dir}/{mode}/jobs/{job_name}/guide_prediction-{sequence_id}/guides_report_{vcf_id}/Guide_differences.csv",
+		diff_guides = "{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/guides_report_{vcf_id}/Guide_differences.csv",
 	params:
 		idx_filtered_vcf = "{root_dir}/{mode}/consensus_refs/{sequence_id}/{vcf_id}.filtered.vcf.gz.tbi",
 		models_path= config["models_path"]
 	# 	# == Main output path
-	# 	main_out = "{root_dir}/{mode}/jobs/{job_name}/guide_prediction-{sequence_id}/guides_report_{vcf_id}/"
+	# 	main_out = "{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/guides_report_{vcf_id}/"
 	conda:
 		"../envs/vcf.yaml"
 	message:
 		"""
 # === PREDICT GUIDES ON ALTERNATIVE GENOMES === #	
 Inputs used:
 --> Template guides obtained from reference assembly:\n {input.guides_report_out}
```

### Comparing `meditability-0.2.1/src/smk/pipelines/py/annotate.py` & `meditability-0.2.2/src/smk/pipelines/py/annotate.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/pipelines/py/aws_pull.py` & `meditability-0.2.2/src/smk/pipelines/py/aws_pull.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/pipelines/py/clinVar_pull.py` & `meditability-0.2.2/src/smk/pipelines/py/clinVar_pull.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/pipelines/py/dataH.py` & `meditability-0.2.2/src/smk/pipelines/py/dataH.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class DataHandler:
     """
     search for guides given a genomic sequence and SNV info
     """
 
-    def __init__(self, query, strand, ref, alt, feature_annotation, models_dir, extracted_seq, rf, coord,gname):
+    def __init__(self, query, strand, ref, alt, feature_annotation, models_dir, extracted_seq, rf, coord,gname,dist_from_cutsite = 7):
         """
         :param query: ex: 'NM_000532.5(PCCB):c.1316A>G (p.Tyr439Cys)' or 'chr19:136327650A>G'
         :param strand: ex. '-' or '+
         :param ref: ex. 'A'
         :param alt: ex. 'G'
         :param feature_annotation: ex: 'exon'
         :param extracted_seq: 'CCCACAGGGCCCTCACCTGCAGATTGTGATTGTGGCCGCACAGGTAGGCAGTGACCCCGT'
@@ -33,29 +33,32 @@
         self.rf = rf
         self.extracted_seq = str(extracted_seq)
         self.annotation = feature_annotation
         self.models_dir = models_dir
         self.coord = coord
         self.chrom = coord.split(':')[0].replace('chr', '')
         self.gname = gname
+        self.dist_from_cutsite = dist_from_cutsite
 
         # search params
         self.pam = str()  # Ex. 'NGG'
         self.pamISfirst = False  # Boolean
         self.win_size = list()  # Ex. list [4,8]
         self.gscoring = None  # Ex. True/False
         self.guidelen = 20
 
         # outputs
         self.guides_found = {'QueryTerm': [], 'GeneName':[],'Editor': [], 'Guide_ID': [], 'Coordinates': [],
-                             'Strand': [], 'gRNA': [], 'Pam': [], 'SNV Position': [],
-                             'On-Target Efficiency Score': [], 'OOF Score':[],'Ref>Alt': [], 'Annotation': []}
-
-        self.BEguides_found = {'QueryTerm': [], 'GeneName':[],'Base Editor': [], 'Guide_ID': [], 'Coordinates': [],
-                               'Strand': [],'gRNA': [], 'Pam': [], 'SNV Position': [],
+                             'Strand': [], 'gRNA': [], 'Pam': [], 'Variant Position': [], 'Extended Guide Site': [],
+                             'Azimuth Score': [], 'DeepCas9 Score':[],'DeepCpf1 Score':[],
+                             'OOF Score':[],'Ref>Alt': [], 'Annotation': []}
+
+        self.BEguides_found = {'QueryTerm': [], 'GeneName':[],'Editor': [], 'Guide_ID': [], 'Coordinates': [],
+                               'Strand': [],'gRNA': [], 'Pam': [], 'Variant Position': [],'Extended Guide Site': [],
+                               'ABE score':[], 'CBE Score':[],
                                'Hg38 Reference (Codon>AA)': [], 'Alternate (Codon>AA)': [], 'BE Converted (Codon>AA)': [],
                                'Conversion Type': [], 'Bystander': [], 'Annotation': []}
 
 
     def set_guide_search_params(self, pam, pamISfirst, win_size, gscoring, guidelen):
         self.pam = pam
         self.pamISfirst = pamISfirst
@@ -100,32 +103,36 @@
                 mtype = 'Non-conservative'
         return mtype
 
     def getBE(self, guides, conversion, win_size, name):
         """
         Finds codon level SNV and determines if the Base Editor Conversion can work
         """
-        coding_strand = self.strand
         snv_rel_pos = len(self.extracted_seq) / 2
 
         for i in range(len(guides)):
-            editor, guide, pam_found, guide_strand, snvpos, on_score, oof_score, start, end = guides[i]
+            scores = {'abe': '-',
+                      'cbe': '-'}
+            editor, guide, pam_found, guide_strand, snvpos, editor_scores,extended_guide, start, end = guides[i]
 
             target_bases = Seq(guide[win_size[0] - 1:win_size[1] + 1])  # Bases inside 4-8 window
 
             # Converted case
             convert = str(conversion[1])
             bystander = target_bases.count(conversion[0]) - 1
+
             if self.annotation not in ['exon','start_codon','stop_codon']:
                 ctype = 'NA'
                 self.add_BEguides(name,
                                   guide,
                                   pam_found,
                                   guide_strand,
                                   snvpos,
+                                  scores,
+                                  extended_guide,
                                   start,
                                   end,
                                   self.NM_ref_allele,
                                   self.NM_alt_allele,
                                   convert,
                                   ctype,
                                   bystander)
@@ -159,47 +166,55 @@
                 alt = f"{alt_codon}>{aa_alt}"
                 convert = f"{new_codon}>{aa_new}"
                 self.add_BEguides(name,
                                   guide,
                                   pam_found,
                                   guide_strand,
                                   snvpos,
+                                  scores,
+                                  extended_guide,
                                   start,
                                   end,
                                   ref,
                                   alt,
                                   convert,
                                   ctype,
                                   bystander)
 
-    def add_guides(self, name, guide, pam_found, strand, snvpos, on_score,oof_score,start,end):
+    def add_guides(self, name, guide, pam_found, strand, snvpos,scores,extended_guide,start,end):
         self.guides_found['QueryTerm'].append(self.query)
         self.guides_found['GeneName'].append(self.gname)
         self.guides_found['Editor'].append(name)
         self.guides_found['Guide_ID'].append(f'{name}_')
         self.guides_found['Coordinates'].append(f'{self.chrom}:{start}-{end}')
-        self.guides_found['On-Target Efficiency Score'].append(on_score)
-        self.guides_found['OOF Score'].append(oof_score)
+        self.guides_found['Azimuth Score'].append(scores['azimuth'])
+        self.guides_found['DeepCas9 Score'].append(scores['deepcas9'])
+        self.guides_found['DeepCpf1 Score'].append(scores['deepcpf1'])
+        self.guides_found['OOF Score'].append(scores['oof'])
+        self.guides_found['Extended Guide Site'].append(extended_guide)
         self.guides_found['Strand'].append(strand)
         self.guides_found['Pam'].append(str(pam_found))
         self.guides_found['gRNA'].append(str(guide))
         self.guides_found['Ref>Alt'].append(f"{self.NM_ref_allele}>{self.NM_alt_allele}")
-        self.guides_found['SNV Position'].append(snvpos)
+        self.guides_found['Variant Position'].append(snvpos)
         self.guides_found['Annotation'].append(self.annotation)
 
-    def add_BEguides(self, name, guide, pam_found, strand, snvpos, start, end, ref, alt, convert, ctype, bystander):
+    def add_BEguides(self, name, guide, pam_found, strand, snvpos, scores,extended_guide,start, end, ref, alt, convert, ctype, bystander):
         self.BEguides_found['QueryTerm'].append(self.query)
         self.BEguides_found['GeneName'].append(self.gname)
         self.BEguides_found['Guide_ID'].append(f'{name}_')
-        self.BEguides_found['Base Editor'].append(name)
+        self.BEguides_found['Editor'].append(name)
         self.BEguides_found['Coordinates'].append(f'{self.chrom}:{start}-{end}')
         self.BEguides_found['gRNA'].append(str(guide))
         self.BEguides_found['Pam'].append(str(pam_found))
-        self.BEguides_found['SNV Position'].append(snvpos)
+        self.BEguides_found['Variant Position'].append(snvpos)
+        self.BEguides_found['ABE score'].append(scores['abe']),
+        self.BEguides_found['CBE Score'].append(scores['cbe']),
         self.BEguides_found['Strand'].append(strand)
+        self.BEguides_found['Extended Guide Site'].append(extended_guide)
         self.BEguides_found['Hg38 Reference (Codon>AA)'].append(ref)
         self.BEguides_found['Alternate (Codon>AA)'].append(alt)
         self.BEguides_found['BE Converted (Codon>AA)'].append(convert)
         self.BEguides_found['Conversion Type'].append(ctype)
         self.BEguides_found['Bystander'].append(bystander)
         self.BEguides_found['Annotation'].append(self.annotation)
 
@@ -209,19 +224,24 @@
         :param pam: pam seq ex:'NGG'
         :param pamISfirst: 5'or3'PAM ex:True/False
         :param win_size: list containing upper and lower limits of the targetable window. Ex:[4,8]
         :param search window: intial search + or - SNV site
         :param guidelen: guide without pam length
         :return: Guide Dictionary
         """
+
         guides = []
         pamlen = len(pam)
         sitelen = guidelen + pamlen
         snv_rel_pos = int(len(self.extracted_seq)/2)
-        on_score, oof_score = '-','-'
+        extended_guide = '-'
+        scores = {'azimuth':'-',
+                  'deepcas9':'-',
+                  'deepcpf1':'-',
+                  'oof':'-'}
         if BEmode:
             win_size = [win_size[0] - guidelen -1,win_size[1] -guidelen-1]
 
         pam_min, pam_max = int((snv_rel_pos - win_size[1]))- 1, int((snv_rel_pos - win_size[0])) - 1
 
         if pamISfirst == True:
             pam_min, pam_max = pam_min + pamlen, pam_max + pamlen
@@ -229,55 +249,62 @@
         # Narrow based on guide params
         for search_strand in ["-", "+"]:
             search_seq = Seq(self.extracted_seq) if search_strand == "+" else Seq(self.extracted_seq).reverse_complement()
             pam_index = SeqUtils.nt_search(str(search_seq), pam)[1:]
 
             for i in pam_index:
                 if i in range(pam_min, pam_max + 1):
-
+                    extended_guide = '-'
+                    scores = {'azimuth': '-',
+                              'deepcas9': '-',
+                              'deepcpf1': '-',
+                              'oof': '-'}
                     if not pamISfirst:  # 3' PAM
                         target_start = i - guidelen
                         guide = search_seq[i - guidelen:i]
+                        extended_guide = str(search_seq[target_start - 3:target_start + sitelen + 4])
                         if not BEmode:
                             if pam == 'NGG' and guidelen == 20:
                                 #Azmith only accurate for NGG pams
-                                on_score = scoring.azimuth([str(search_seq[target_start - 3:target_start + sitelen + 4])],
+                                scores['azimuth'] = scoring.azimuth([extended_guide],
                                                            self.models_dir)[0]
+                                scores['deepcas9'] = round(scoring.deepspcas9([extended_guide],
+                                                           self.models_dir)[0][0],2)
                             #oof_score use only for DSB
-                            mh_score, oof_score = scoring.oofscore(str(search_seq[target_start - 20:target_start + sitelen + 20]))
+                            mh_score, scores['oof'] = scoring.oofscore(str(search_seq[target_start - 20:target_start + sitelen + 20]))
 
                         pam_found = str(search_seq[i:i + pamlen])
 
                     else:
                         target_start = i + pamlen
                         guide = search_seq[target_start: i + sitelen]
                         pam_found = search_seq[i:target_start]
+                        extended_guide = str(search_seq[i - 5:i + sitelen + 4])
                         if 'Cas12a' in name:
-                            on_score = round(scoring.deepcpf1([str(search_seq[i - 5:i + sitelen + 4])],
+                            scores['deepcpf1'] = round(scoring.deepcpf1([extended_guide],
                                                               self.models_dir)[0][0], 2)
 
                     snvpos = snv_rel_pos - target_start
                     start = self.SNV_chr_pos - snvpos
                     end = start + sitelen
 
-                    guides.append([name, guide, pam_found, search_strand, snvpos, on_score, oof_score, start, end])
+                    guides.append([name, guide, pam_found, search_strand, snvpos, scores,extended_guide, start, end])
 
                     if not BEmode:
-                        self.add_guides(name, guide, pam_found, search_strand, snvpos, on_score, oof_score, start, end)
+                        self.add_guides(name, guide, pam_found, search_strand, snvpos, scores ,extended_guide, start, end)
         return guides
 
     def get_Guides(self, search_params, BEsearch_params=None):
-
         for name, params, in search_params.items():
             pam, pamISfirst, guidelen, dsb_loc = params[0:4]
-            win_size = [int(dsb_loc)-7, int(dsb_loc)+7]
+            win_size = [int(dsb_loc)-self.dist_from_cutsite, int(dsb_loc)+self.dist_from_cutsite]
             guides = self.get_guide_set(name, pam, pamISfirst,win_size, guidelen, BEmode=False)
 
         # if BE mode is on
-        if BEsearch_params is not None:
+        if BEsearch_params is not None and len(self.NC_ref_allele + self.NC_alt_allele) ==2:
             for k, params, in BEsearch_params.items():
                 pam, pamISfirst, guidelen, win_size = params[0][0], params[0][1], params[0][2], params[0][3]
                 bguides = self.get_guide_set(k, pam, pamISfirst, win_size, guidelen, BEmode=True)
 
                 # if guides are found sep neg and pos strand guides
                 if len(bguides) > 0:
                     pos_guides, neg_guides = [], []
```

### Comparing `meditability-0.2.1/src/smk/pipelines/py/featurization.py` & `meditability-0.2.2/src/smk/pipelines/py/featurization.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/pipelines/py/fetchGuides.py` & `meditability-0.2.2/src/smk/pipelines/py/fetchGuides.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,35 +25,37 @@
 		os.makedirs(outdir)
 	return outdir
 
 
 class Fetch_Guides:
 
 	def __init__(self,
-	             queries: list,
-	             qtype: str,
-	             editor_request: str | list,
-	             be_request: str | list,
-	             editors: dict,
-	             base_editors: dict,
-	             datadir: str,
-	             fasta_path: str,
-	             annote_path: str,
-	             **kwargs):
+				 queries: list,
+				 qtype: str,
+				 editor_request: str | list,
+				 be_request: str | list,
+				 editors: dict,
+				 base_editors: dict,
+				 dist_from_cutsite: int,
+				 datadir: str,
+				 fasta_path: str,
+				 annote_path: str,
+				 **kwargs):
 		"""
 		:param queries: list of query terms, either in hgvs format - 'NM_000518.5:c.114G>A' or coords 'chr11:5226778C>T' (COORDS ALLELES MUST BE PLUS STRAND!!)
 		:param qtype: 'hgvs' or 'coord'
 		  --> if 'hgvs', providing the coordinates in the kwargs with 'hgvscoord' can reduce processing time
 		  --> hgvs assumes the query is already in clinvar and will generate a variant report with the gene report,
 		  --> if 'coord' then just gene report is created
 		:param editor_request: 'clinical', 'custom', name (list/str from editor choices)
 		--> custom must contain kwargs - pam, pamISFirst,guidelen (optional:name,win_size)
 		:param be_request: 'off','default','all', or select BE editor for base editor choices below
 		:param editors: Dictionary containing information on the current set of editors supported by mEdit
 		:param base_editors: Dictionary containing information on the current set of base editors supported by mEdit
+		:param dist_from_cutsite: this is how farway the cutsite may be from the start of the variant position
 		:param genome: genome used
 		:param datadir: folder where tables and pre-computed data live
 		:param fasta_path: *Unsure using chromsome seperate files right now but unsure if this will be permenant
 		:param kwargs: 'hgvscoord' , 'clin_report','gene_report'
 		"""
 		##-----------------User Inputs--------------------##
 		if qtype == 'hgvs':
@@ -62,24 +64,28 @@
 			self.queries = self.validate_coord(queries)
 		self.qtype = qtype
 		self.editor_request = editor_request
 		self.be_request = be_request
 		self.kwargs = kwargs
 		self.editor_lib = editors
 		self.be_lib = base_editors
+		self.dist_from_cutsite = dist_from_cutsite
 
 		# input paths/folders
 		self.processed_tables = f"{datadir}/processed_tables"  # folder with cleaned clinvar/hpa tabs
 		self.HGVSlookup_path = f"{self.processed_tables}/HGVSlookup.csv"
 		self.fasta_path = fasta_path
 		self.annote_path = annote_path
 		self.window = 50
+		if self.dist_from_cutsite > 7:
+			self.window = 100
+		# self.dist_from_cutsite = 7
 
 		# other variables
-		self.snv_info = {}  # {chrom: (id,snv_pos,ref,alt)}
+		self.snv_info = {}  # {chrom: (queryterm,tid,eid,gene,strand,ref,alt,feature,extracted_seq,rf,coord)}
 
 		##---------------libraries and keys--------------------##
 		self.editor_choices = list(editors.keys())
 		self.BE_choices = list(base_editors.keys())
 
 		## ------------Defaults and settings------------------##
 		##configure editor options
@@ -112,15 +118,15 @@
 		elif type(self.editor_request) is list:
 			search_params = {}
 			for editor in self.editor_request:
 				try:
 					search_params[editor] = self.editor_lib['user_request'][editor]
 				except KeyError:
 					print(f"Please list one or more editors available at the current version's list:"
-					      f" \n{self.editor_lib['user_request'].keys()}")
+						  f" \n{self.editor_lib['user_request'].keys()}")
 					raise Exception(f"The editor {editor} isn't available in the currently version of mEdit")
 
 		# else use single set parameters
 		else:
 			if self.editor_request in self.editor_choices:
 				search_params = {self.editor_request: self.editor_lib[self.editor_request]}
 
@@ -196,21 +202,34 @@
 		#query, tid, eid, strand, ref, alt, feature_annotation, extracted_seq, codons, coord
 		'''
 		with open(outfile, 'ab') as sfile:
 			pickle.dump(self.snv_info, sfile)
 
 	def write_not_found(self, outfile):
 		if len(self.not_found.keys()) > 0:
-			pd.DataFrame(self.not_found).to_csv(outfile, index=False)
+			pd.Series(data=self.not_found.values(), index=self.not_found.keys()).to_csv(outfile)
+
+	def write_extracted_sequences(self, extracted_seq_outfile):  # Taylor's been Walter Whiting here.
+		'''
+		writes tab-deliminated file of 100-mer sequence in which each
+		each variant was found.
+		'''
+		if len(self.snv_info.keys()) > 0:
+			with open(extracted_seq_outfile, "w") as out:
+				for chrom, snv_info in self.snv_info.items():
+					for value in snv_info:
+						query = value[0]
+						extracted_seq = str(value[8])
+						print(query + "\t" + extracted_seq, file=out)
 
 	def write_guide_csv(self, guides, outfile):
 		df = pd.DataFrame(guides)
 		if 'On-Target Efficiency Score' in df.columns:
 			temp = df[df['On-Target Efficiency Score'] != '-'].sort_values(by='On-Target Efficiency Score',
-			                                                               ascending=False)
+																		   ascending=False)
 			temp = temp.sort_values(by='Editor')
 			df = pd.concat([temp, df[df['On-Target Efficiency Score'] == '-']]).reset_index(drop=True)
 		df['Guide_ID'] = [y + str(x) for x, y in zip(list(df.index), list(df['Guide_ID']))]
 		df.to_csv(outfile, index=False)
 		return df
 
 	def add_clinvar(self, gadf):
@@ -236,19 +255,43 @@
 
 	def add_not_found(self, nfqueries, reason):
 		# adds queries that are not found ex: no guides or hgvs not found
 		for nf in nfqueries:
 			self.not_found[nf] = reason
 
 	@staticmethod
-	def extract_seqs(searchseq, pos, alt, window):
+	def extract_seqs(searchseq, pos, ref, alt, window):
 		# extracts the sequence +/windowbp surrounding a SNV then swaps ref for alt allele
-		extracted_seq = str(searchseq[pos - window:pos + window])
-		extracted_seq = Seq(extracted_seq[0:window] + alt + extracted_seq[window + 1:]).upper()
-		return extracted_seq
+
+		if len(ref) == len(alt):  ##substitution
+			extracted_seq = str(searchseq[pos - window:pos + window])
+			variant_seq = (extracted_seq[0:window] + alt + extracted_seq[window + len(alt):]).upper()
+
+
+		elif len(ref) > len(alt):  # deletion
+			diff= len(ref) - len(alt)
+			extracted_seq = str(searchseq[pos - window:(pos + window + diff)])
+			variant_seq = (extracted_seq[0:window] + alt+ extracted_seq[window+len(ref):]).upper()
+
+		elif len(ref) < len(alt):  # insertion
+			extracted_seq = str(searchseq[pos - window:pos + window - (len(alt))])
+			variant_seq = (extracted_seq[0:window] + alt + extracted_seq[window:]).upper()
+		# print(new_seq)
+
+		else:
+			print('VARIANT REF AND ALT DO NOT COMPLY')
+			print(ref,alt,pos)
+		#if len(variant_seq) != 2* self.window:
+		#	print('SEQUENCE LENGTH less than 100')
+		#	print('REF', ref)
+		#	print('ALT', alt)
+		#	print('t_pos', pos)
+
+
+		return variant_seq
 
 	def get_chroms(self, queries):
 		# finds unique chromosome for each hgvs
 		# needs to happen in order to select right fasta file
 		hgvs_tab = pd.read_csv(self.HGVSlookup_path)
 		q_prefixes = [x.split(':')[0] for x in queries]
 		chroms = set(hgvs_tab.loc[hgvs_tab['TranscriptID'].isin(q_prefixes), 'Chr'])
@@ -269,20 +312,21 @@
 				self.snv_info[ch] = \
 				gadf[['HGVS_Simple', 'PositionVCF', 'RefAlleleVCF', 'AltAlleleVCF']].to_dict('tight')['data']
 			found = []
 			for k in self.snv_info.keys():
 				for v in self.snv_info[k]:
 					found.append(v[0])
 			notfound = list(set(self.queries).difference(set(found)))
-			self.add_not_found(notfound, 'hgvs not found in clinvar')
+			self.add_not_found(notfound, 'hgvs not found in medit variant database')
 
 		# Else All information is given to find transcript info
 		else:
 
-			coord_fmt = r'chr[0-9MTXY]*:(\d*)([ATCG]{1})\>([ATCG]{1})'
+			# coord_fmt = r'chr[0-9MTXY]*:(\d*)([ATCG]{1})\>([ATCG]{1})'
+			coord_fmt = r'chr[0-9MTXY]*:(\d*)([ATCG]{1,10})\>([ATCG]{1,10})'
 			for query in self.queries:
 				ch = query.split(':')[0].replace('chr', '')
 				if ch not in self.snv_info.keys():
 					self.snv_info[ch] = []
 				snvpos, alt, ref = list(re.search(coord_fmt, query).groups())
 				self.snv_info[ch].append([query, int(snvpos), alt, ref])
 
@@ -317,38 +361,46 @@
 					snvcoord = f'chr{ch}:{d[1]}-{d[1]}'
 					tx = Transcript.transcript(snvcoord)
 
 					if tx == 'intergenic':
 						tid, eid, gname = '-', '-', '-'
 						feature_annotation = tx
 						rf, strand = 'None', '+'
-						extracted_seq = self.extract_seqs(searchseq=fasta.seq, pos=snvpos, alt=alt, window=self.window)
+						extracted_seq = self.extract_seqs(searchseq=fasta.seq, pos=snvpos, ref=ref, alt=alt,
+														  window=self.window)
 
 
 					else:
 						eid, tid, gname, strand, txstart = tx.tx_info()
 						tx_seq = tx.get_tx_seq(fasta)
 						t_snvpos = int(snvpos) - int(txstart)
-						extracted_seq = self.extract_seqs(searchseq=tx_seq, pos=t_snvpos - 1, alt=alt,
-						                                  window=self.window)
+						extracted_seq = self.extract_seqs(searchseq=tx_seq, pos=t_snvpos - 1, ref=ref, alt=alt,
+														  window=self.window)
 
 						if len(extracted_seq) != self.window * 2:
 							# if flanking or utr the extracted seq needs to come from the chromosome file
-							extracted_seq = self.extract_seqs(searchseq=fasta.seq[snvpos - 100:snvpos + 100],
-							                                  pos=t_snvpos - 1,
-							                                  alt=alt,
-							                                  window=self.window)
+							print('Extracted Sequence Length OUT OF BOUNDS in Transcript Sequence ')
+							print('Searching chromosome sequence instead')
+
+							extracted_seq = self.extract_seqs(
+								searchseq=fasta.seq[snvpos - self.window * 3:snvpos + self.window * 3],
+								pos=self.window * 3,
+								ref=ref,
+								alt=alt,
+								window=self.window)
 
 						feature_annotation, rf = tx.feature, tx.rf
 
 					new_data.append(
 						[query, tid, eid, gname, strand, ref, alt, feature_annotation, extracted_seq, rf,
 						 f"chr{str(ch)}:{str(snvpos)}"])
 
 					print('Query term & annoation:', query, feature_annotation)
+				else:
+					self.add_not_found(query, 'ref or alt allele contain non-ATCG characters')
 			self.snv_info[ch] = new_data
 
 	@staticmethod
 	def validate_hgvs(queries):
 		'''
 		standardizes input hgvs and checks formating
 		'''
@@ -366,15 +418,15 @@
 
 	@staticmethod
 	def validate_coord(queries):
 		'''
 		standardizes input coordinate and checks formatting
 		'''
 		# q = 'chr11:5226778C>T'
-		coord_fmt = r'(chr[0-9]*:\d*(A|T|C|G)>(A|T|C|G))'
+		coord_fmt = r'(chr[0-9XYM]*:\d*(A|T|C|G)>(A|T|C|G))'
 		validated_queries = []
 		for q in set(queries):
 			if re.search(coord_fmt, q):
 				validated_queries.append(re.search(coord_fmt, q).groups()[0])
 			else:
 				print(q)
 		n = len(validated_queries)
@@ -394,15 +446,15 @@
 				try:
 					query, tid, eid, gname, strand, ref, alt, feature_annotation, extracted_seq, codons, coord = d
 				except ValueError:
 					print(
 						f"WARNING: The query below has the wrong number of values to unpack. Needs further investigation:\n{d}")
 					continue
 				dh = DataHandler(query, strand, ref, alt, feature_annotation, models_dir, extracted_seq, codons, coord,
-				                 gname)
+								 gname, self.dist_from_cutsite)
 
 				if self.be_request != 'off':
 					guides, BEguides = dh.get_Guides(self.search_params, self.BE_search_params)
 				else:
 					guides, BEguides = dh.get_Guides(self.search_params)
 
 				if len(BEguides['gRNA']) > 0:
@@ -429,30 +481,31 @@
 		guidedf, BEdf = None, None
 
 		if len(self.all_guides.keys()) != 0:
 			guidedf = self.write_guide_csv(self.all_guides, outfile_guides)
 		else:
 			print('No Editor Guides found for any queries')
 
-		if len(self.all_BE.keys()) != 0:
-			BEdf = self.write_guide_csv(self.all_BE, outfile_be_guides)
-		else:
-			print('No Base Editor Guides found for any queries')
+		if self.be_request != 'off':
+			if len(self.all_BE.keys()) != 0:
+				BEdf = self.write_guide_csv(self.all_BE, outfile_be_guides)
+			else:
+				print('No Base Editor Guides found for any queries')
 
 		return {'all_variant': self.all_variant,
-		        'all_gene': self.all_gene,
-		        'guide_table': guidedf,
-		        'BE_table': BEdf}
+				'all_gene': self.all_gene,
+				'guide_table': guidedf,
+				'BE_table': BEdf}
 
 
 def main():
 	# SNAKEMAKE IMPORTS
 	# === Inputs ===
 	input_file = str(snakemake.input.query_manifest)
-	fasta_path = str(snakemake.input.assembly_path)
+	fasta_path = str(snakemake.input.assembly_dir_path)
 	# === Outputs ===
 	guides_report = str(snakemake.output.guides_report_out)
 	guide_search_params_path = str(snakemake.output.guide_search_params)
 	snv_site_info_path = str(snakemake.output.snv_site_info)
 	# === Params ===
 	resultsfolder = set_export(str(snakemake.params.main_out))
 	gene_report = f"{resultsfolder}/{str(snakemake.params.gene_report)}"
@@ -461,14 +514,15 @@
 	#   == Processed tables branch ==
 	datadir = str(snakemake.params.support_tables)
 	annote_path = str(snakemake.params.annote_path)
 	# == Editor Parameters
 	editors_path = str(snakemake.params.editors)
 	base_editors_path = str(snakemake.params.base_editors)
 	models_path = str(snakemake.params.models_path)
+	distance_from_cutsite = int(snakemake.params.distance_from_cutsite)
 	#   == Run Parameters ==
 	qtype = str(snakemake.params.qtype)
 	be_request = str(snakemake.params.be_request)
 	editor_request = str(snakemake.params.editor_request)
 	# == DEBUG BLOCK ==
 	# qtype = 'hgvs'
 	# BEmode = 'off'
@@ -499,23 +553,24 @@
 		-> {datadir}
 	OUTPUTS TO:
 		--> {resultsfolder}
 	""")
 
 	# == Get query items ==
 	fg = Fetch_Guides(queries,
-	                  qtype,
-	                  editor_request,
-	                  be_request,
-	                  editors,
-	                  base_editors,
-	                  datadir,
-	                  fasta_path,
-	                  annote_path
-	                  )
+					  qtype,
+					  editor_request,
+					  be_request,
+					  editors,
+					  base_editors,
+					  distance_from_cutsite,
+					  datadir,
+					  fasta_path,
+					  annote_path
+					  )
 	# == Set up object and run core methods ==
 	exports = fg.run_FetchGuides(guides_report, be_report, models_path)
 
 	# == Export Intermediate files ==
 	fg.write_snv_site_info(snv_site_info_path)
 	fg.write_gsearch_params(guide_search_params_path)
```

### Comparing `meditability-0.2.1/src/smk/pipelines/py/find_offtargets.py` & `meditability-0.2.2/src/smk/pipelines/py/find_offtargets.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 Copyright (c) 2021 Jeongbin Park and Sangsu Bae
 Website: http://github.com/snugel/cas-offinder
 
 Usage: cas-offinder {input_filename|-} {C|G|A}[device_id(s)] {output_filename|-}
 (C: using CPUs, G: using GPUs, A: using accelerators)
 '''
 
+# INPUT LEG
 def make_casoffinder_input(infile,fasta_fname,pam, pamISfirst, guidelen,guides,gnames,casoff_params):
     ## create input file for cas-offinder
     mm, RNAbb, DNAbb, PU = casoff_params
 
     with open(infile, 'w') as f:
         f.writelines(fasta_fname + "\n")
         line = 'N' * guidelen
@@ -41,22 +42,23 @@
                 line = f"{dpam}{grna} {mm} {gname}" + "\n"
             else:
                 line = f"{grna}{dpam} {mm} {gname}" + "\n"
             f.writelines(line)
 
 
 
+# INPUT/OUTPUT LEG
 def cas_offinder_bulge(input_filename, output_filename,cas_off_expath,bulge):
     '''
      The cas-offinder off-line package contains a bug that doesn't allow bulges
     This script is partially a wrapper for cas-offinder to fix this bug
      created by...
     https://github.com/hyugel/cas-offinder-bulge
     '''
-
+    # INPUT LEG
     fnhead = input_filename.replace("_input.txt", "")
     id_dict = {}
     if bulge == True:
         with open(input_filename) as f:
             chrom_path = f.readline()
             pattern, bulge_dna, bulge_rna = f.readline().strip().split()
             isreversed = False
@@ -116,35 +118,40 @@
                 f.write(pattern + bulge_dna*'N' + '\n')
             else:
                 f.write(bulge_dna*'N' + pattern + '\n')
             cnt = 0
             for tgt, mismatch in bg_tgts.items():
                 f.write(tgt + ' ' + str(max(mismatch)) + ' ' + '\n')
                 cnt+=1
+        # THIS FILE PATH IS SUPPLIED TO CASOFF-FINDER
         casin = fnhead + '_bulge.txt'
     else:
         nobulge_dict = {}
         with open(input_filename) as inf:
             for line in inf:
                 entry = line.strip().split(' ')
                 if len(entry) > 2 and len(entry[-1]) > 3:
                     seq, mm, gid = entry
                     nobulge_dict[seq] = [gid, mm]
         casin = input_filename
 
     print("Created temporary file (%s)." % (casin))
+    # THIS FILE PATH IS SUPPLIED TO CASOFF-FINDER
     outfn = fnhead + '_temp.txt'
     print("Running Cas-OFFinder (output file: %s)..." % outfn)
+
+
     p = Popen([cas_off_expath, casin, 'C', outfn])
     ret = p.wait()
     if ret != 0:
         print("Cas-OFFinder process was interrupted!")
         exit(ret)
     print("Processing output file...")
 
+    # OUTPUT LEG
     with open(outfn) as fi, open(output_filename, 'w') as fo:
         fo.write('Coordinates\tDirection\tGuide_ID\tBulge type\tcrRNA\tDNA\tMismatches\tBulge Size\n')\
         #fo.write('Guide_ID\tBulge type\tcrRNA\tDNA\tChromosome\tPosition\tDirection\tMismatches\tBulge Size\n')
         ot_coords = []
         for line in fi:
             entries = line.strip().split('\t')
             ncnt = 0
@@ -289,15 +296,15 @@
             ots_dict[gid] ={}
             for i in ['X','RNA','DNA']:
                 for j in range(mmco+1):
                     ots_dict[gid][(i,j)]= 0
         ots_dict[gid][(btype,int(mm))] += 1
     return ots_dict
 
-
+# OUTPUT LEG
 def write_out_res(ots,gdf,casoff_params,resultsfolder,guide_tab_fname):
     '''
     Adds two new columns to guides found table
     Creates and Aggregate summary text output
     '''
     df = pd.DataFrame(ots)#.rename(columns = {'0':'Off Target Score'})
     #this is just a precautionary if this script was run more than once
```

### Comparing `meditability-0.2.1/src/smk/pipelines/py/gdrive_import.py` & `meditability-0.2.2/src/smk/pipelines/py/gdrive_import.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/pipelines/py/genome_seq_search.py` & `meditability-0.2.2/src/smk/pipelines/py/genome_seq_search.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/pipelines/py/make_tables.py` & `meditability-0.2.2/src/smk/pipelines/py/make_tables.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # 		config = yaml.load(f, Loader=yaml.FullLoader)
 
 '''
 clinvar_ftp = "https://ftp.ncbi.nlm.nih.gov/pub/clinvar/tab_delimited/variant_summary.txt.gz"
 clinvar_vcf = ' https://ftp.ncbi.nlm.nih.gov/pub/clinvar/vcf_GRCh38/clinvar.vcf.gz'
 clinvar_index = ' https://ftp.ncbi.nlm.nih.gov/pub/clinvar/vcf_GRCh38/clinvar.vcf.gz.tbi'
 refseq = "https://hgdownload.soe.ucsc.edu/goldenPath/hg38/database/ncbiRefSeq.txt.gz"
+var_citations = "https://ftp.ncbi.nlm.nih.gov/pub/clinvar/tab_delimited/var_citations.txt"
 '''
 datadir = "/groups/clinical/projects/editability/tables/"
 
 # database paths
 raw_tables = f"{datadir}raw_tables/"
 clinvar_summary = f"{raw_tables}clinvar/variant_summary.txt.gz"  # raw clinvar table
 mane_path = f'{raw_tables}clinvar/MANE.GRch38.v1.1.summary.txt.gz'
@@ -28,16 +29,14 @@
 
 processed_tables = f"{datadir}processed_tables/"
 simple_tables = f"{processed_tables}guide_acquisition_tables/"
 HGVSlookup_path = f"{processed_tables}HGVSlookup.csv" #Chrom to refID key table
 lastUpdate_file = f"{processed_tables}clinvar_lastUpdate.txt"
 mane_cleaned = f'{processed_tables}MANE.GRch38.summary_cleaned.txt.gz'
 
-
-
 #variables
 chroms = ['1', '2','3', '4', '5', '6', '7', '8', '9', '10', '11','12',
                  '13', '14', '15', '16', '17', '18', '19', '20', '21', '22','MT', 'Y', 'X']
 
 
 def process_refseq(raw_tables,processed_tables):
     '''
@@ -82,14 +81,37 @@
                 line_out = [chrom,tstart,tend,'|'.join([strand,tid,eid,gname,cds_start,cds_end, exons_start,exon_end,frames])]
                 ref_out.write('\t'.join(line_out) + '\n')
                 if cnt < 20:
                     print('\t'.join(line_out))
 
     ref_out.close()
 
+def process_citations(raw_tables):
+    citations = pd.read_csv(f"{raw_tables}var_citations.txt", sep = "\t")
+    citations = citations[['#AlleleID', 'citation_source', 'citation_id']].rename(
+        columns={'#AlleleID': 'AlleleID'})
+    alids = []
+    for ch in chroms:
+        alids +=list(pd.read_csv(f"{processed_tables}variant_tables/{ch}_variant.txt")['AlleleID'].astype('int'))
+    grp = citations.groupby('AlleleID')
+    new_citations = {'AlleleID':[],
+                     'citation_source':[],
+                     'citation_id':[]
+                     }
+    for g in grp:
+        new_citations['AlleleID'].append(g[0])
+        new_citations['citation_source'].append('|'.join(list(set(g[1].citation_source))))
+        new_citations['citation_id'].append('|'.join(list(set(g[1].citation_id))))
+
+
+    citations = pd.DataFrame(new_citations)
+    citations = citations[citations['AlleleID'].isin(alids)]
+    citations.to_csv(f"{processed_tables}var_citations.csv",index = False)
+
+
 
 def process_MANE(raw_tables,processed_tables):
     '''
     Mane has joins ENS and REFSEQ IDs
     '''
     mane = pd.read_csv(f'{raw_tables}clinvar/MANE.GRch38.v1.1.summary.txt.gz', sep="\t")
 
@@ -104,36 +126,36 @@
     mane.to_csv(f'{processed_tables}MANE.GRch38.summary_cleaned.txt.gz',index = False, compression='gzip')
 
 
 def process_clinvarVCF(processed_tables):
     '''
     clinvarvcf has molecular consequences
     '''
-    mc = pd.read_csv('/groups/clinical/projects/editability/tables/raw_tables/clinvar/clinvar.vcf'
+    mc = pd.read_csv('/groups/clinical/projects/editability/tables/raw_tables/clinvar/clinvar.vcf.gz'
                      , comment='#', sep='\t', names=['Chr', 'PositionVCF', '?', 'REF', 'ALT', 'x', 'x1','attributes'])
+    mc = mc.drop(columns = ['?','x','x1'])
     mc['chrHGVS_ID'] = mc['attributes'].str.extract(r'CLNHGVS=([^;]*)', expand=False)
     mc['MC'] = mc['attributes'].str.extract(r'MC=([^;]*)', expand=False)
     mc['AlleleID'] = mc['attributes'].str.extract(r'ALLELEID=([^;]*)', expand=False)
     con = []
     mc.loc[mc['MC'].isna(),'MC'] = '-'
     for x in mc['MC']:
         if '|' in x:
             x = ','.join([y for y in x.split('|') if 'SO' not in y])
         con.append(x)
     mc['MC'] = con
-
     mc = mc.drop(columns=['x1', 'x', 'attributes'])
     mc.to_csv(f'{processed_tables}clinvarvcf2txt.txt', index=False)
 
 
 def add_molecular_consequences(chroms,processed_tables):
     '''
     add molecular consequences
     '''
-    for ch in chroms[10:]:
+    for ch in chroms:
         df = pd.read_csv(f"{processed_tables}variant_tables/{ch}_variant.txt")
         mc = pd.read_csv(f'{processed_tables}clinvarvcf2txt.txt')
         mc['Chr'] = mc['Chr'].astype('str')
         mc = mc[mc['Chr'] == ch]
         mc = mc[['MC', 'AlleleID']]
         mc['AlleleID'] = mc['AlleleID'].astype('int64')
         joined = df.join(mc.set_index('AlleleID'), on='AlleleID')
@@ -154,15 +176,15 @@
             simple_ids.append(suf)
         elif h.startswith('m'):
             tid = 'm'
             suf = h
             tids.append(tid)
             simple_ids.append(suf)
         else:
-            print(h)
+            print(' Removed-None conforming HGVSID format; ', h)
             tids.append('-')
             simple_ids.append('-')
 
     vdf.insert(3, 'HGVS_Simple', simple_ids)
     vdf.insert(4,'TranscriptID',tids)
     vdf = vdf.loc[vdf['HGVS_Simple'] !='-']
     vdf = vdf.reset_index(drop=True)
@@ -236,19 +258,28 @@
         out_fname = f"{processed_tables}/variant_tables/{ch}_variant.txt"
         lines = []
         for line in contents:
             line = line.split("\t")
             if line[18] == str(ch):
                 if line[16] != "GRCh37": # Remove hg19 data
                     line[-1] = line[-1].replace("\n", "")
-                    if 'single nucleotide variant' in line:
+                    if 'single nucleotide variant' in line or 'Deletion' in line:
+                        line = [line[i] for i in cols]
+                        lines.append(line)
+                    elif 'Indel' in line or 'Insertion' in line or 'Duplication ':
                         line = [line[i] for i in cols]
                         lines.append(line)
 
         vdf = pd.DataFrame(lines, columns = [allcols[i] for i in cols])
+        vdf = vdf[vdf.RefAlleleVCF != 'na']
+        vdf = vdf[vdf.AltAlleleVCF != 'na']
+
+        vdf = vdf[vdf.RefAlleleVCF.str.len()<100] #Deletion under 100
+        vdf = vdf[vdf.AltAlleleVCF.str.len()<10]
+
         vdf['HGNC_ID'] = vdf['HGNC_ID'].apply(lambda x: x.replace("HGNC:",""))
         vdf['PositionVCF'] = vdf['PositionVCF'].astype('int')
         vdf = vdf[vdf['PositionVCF']>1]
         vdf = vdf.sort_values('GeneSymbol')
 
         #Extract GeneID and GeneSymbol from HGVSID, In places that are missing
         blankgenes = vdf.loc[vdf['GeneID'] == '-1']
@@ -266,14 +297,15 @@
         vdf = extract_tid_from_hgvs(vdf)
         vdf = extractOMIM(vdf)
         vdf.to_csv(out_fname,index=False)
 
 
 def make_var_table(clinvar_summary,chroms):
     clean_clinvar(clinvar_summary, chroms)
+    process_MANE(raw_tables, processed_tables)
     add_MANE(processed_tables, chroms)
     add_molecular_consequences(chroms,processed_tables)
 
 
 def make_gene_tables(processed_tables,HPApath):
     '''
     attached HPA gene expression info to clinvar info by ensembl id
@@ -302,15 +334,15 @@
     for ch in chroms:
         clin = pd.read_csv(f"{processed_tables}variant_tables/{ch}_variant.txt")
         names += list(set(clin['TranscriptID']))
         chrs += [ch for i in range(len(set(clin['TranscriptID'])))]
 
     df = pd.DataFrame({"TranscriptID": names, "Chr": chrs}).drop_duplicates()
     out_file = f"{processed_tables}HGVSlookup.csv"
-    df.to_csv(out_file, index=None)
+    df.to_csv(out_file, index=False)
 
 
 def updateTables(clinvar_ftp,clinvar_summary,refseq):
     # TODO: add user inquiry to whether they want to init update
     print("updating to latest version of clinvar")
 
     cmd = f"wget {clinvar_ftp} -O {clinvar_summary}"
@@ -325,29 +357,35 @@
 
     cmd = f"wget https://ftp.ncbi.nlm.nih.gov/refseq/MANE/MANE_human/current/MANE.GRCh38.v1.1.summary.txt.gz -O " \
           f"{raw_tables}clinvar/MANE.GRch38.v1.1.summary.txt.gz"
     p = subprocess.run(cmd, shell=True,
                        capture_output=True)
     print(p)
 
-    # cmd = f"wget {clinvar_vcf} -O {raw_tables}clinvar/clinvar.vcf.gz"
-    # p = subprocess.run(cmd, shell=True,
-    #                    capture_output=True)
-    # print(p)
+    cmd = f"wget {clinvar_vcf} -O {raw_tables}clinvar/clinvar.vcf.gz"
+    p = subprocess.run(cmd, shell=True,
+                        capture_output=True)
+    print(p)
+
+    cmd = f"wget {var_citations} -O {raw_tables}var_citations.txt"
+    p = subprocess.run(cmd, shell=True,
+                       capture_output=True)
+    print(p)
     # cmd = f"wget {clinvar_index} -O {raw_tables}clinvar/clinvar.vcf.gz.tbi"
     # p = subprocess.run(cmd, shell=True,
     #                    capture_output=True)
     #
     # cmd = f"bcftools view -f type!=snp {clinvar_vcf} -o {raw_tables}clinvar/clinvar.vcf -O v"
     # p = subprocess.run(cmd, shell=True,
     #                    capture_output=True)
 
     print("Cleaning and Splitting Clinvar.....")
     clean_clinvar(clinvar_summary, chroms)
     print("Adding Ensembl Identifiers....")
+    process_MANE(raw_tables, processed_tables)
     add_MANE(processed_tables, chroms)
     print("Adding Molecular Consequences....")
     add_molecular_consequences(chroms, processed_tables)
     print("Appending HPA data.....")
     make_gene_tables(processed_tables, HPApath)
     print("Writing new HGVS Lookup table.....")
     make_HGVStable(processed_tables, chroms)
@@ -367,7 +405,9 @@
     f = open(lastUpdate_file, "r").readlines()
     lastdate = datetime.strptime(f[0], '%Y-%m-%d').date()
     if (date.today() - lastdate).days > 31:
         updateTables()
     else:
         print('You are using the latest clinvar data')
         print(f"Last updated {lastdate}")
+
+
```

### Comparing `meditability-0.2.1/src/smk/pipelines/py/ncbi_cross_database.py` & `meditability-0.2.2/src/smk/pipelines/py/ncbi_cross_database.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/pipelines/py/process_genome.py` & `meditability-0.2.2/src/smk/pipelines/py/process_genome.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     '''
     seraches for an alternate genome variant in the +/-60bp of snv query position
     '''
     #snv_coord = 'chr11:5226788'
     #extracted_seq = 'ATCCCCAAAGGACTCAAAGAACCTCTGGGTTCAAGGGTAGACCACCAGCAGCCTAAGGGT'
     ch, pos = snv_coord.split(':')
     records_found = []
+    print(ch,pos)
 
     vcf_reader = vcf.Reader(filename = vcf_fname, compressed = True)
     for record in vcf_reader.fetch(ch, int(pos) - window, int(pos) + window):
         records_found.append(record)
         print(record)
     return records_found
 
@@ -232,17 +233,21 @@
     #       Once the DataHandler class is properly instantiated this can be removed
     models_path = str(snakemake.params.models_path)
     # === Wildcards ===
     altgenome_name = str(snakemake.wildcards.vcf_id)
     refgenome_name = str(snakemake.wildcards.sequence_id)
 
     # resultsfolder = "/groups/clinical/projects/editability/medit_queries/medit_test/test_out/"
-    # vcf_fname = "/groups/clinical/projects/editability/tables/raw_tables/VCFs/HG02257.filtered.vcf.gz"
-    # altgenome_name = 'HG02257'
-    # refgenome_name = 'HG38'
+    # datadir = "/groups/clinical/projects/editability/tables/"
+    # filtered_vcf = f"{datadir}raw_tables/VCFs/HG02257.filtered.vcf.gz"
+    # models_path = "/home/thudson/projects/editability/scr/pkl/models/"
+    # snv_site_info, guide_search_params  = f'{resultsfolder}snv_site_info.pkl',f'{resultsfolder}guide_search_params.pkl'
+    # guides_report = f'{resultsfolder}hg38_Guides_found.csv'
+    # altgenome_name,refgenome_name  = 'HG02257','HG38'
+    # diffguides_out = f'{resultsfolder}HG02257_guide_differences.csv'
 
     # Generate vcf index with tabix
     print(f"Generate tabix file on:\n {idx_filtered_vcf}")
     subprocess.run(f"tabix {filtered_vcf}", shell=True)
 
     fetch_ALT_guides(filtered_vcf,
                      guides_report,
```

### Comparing `meditability-0.2.1/src/smk/pipelines/py/scoring.py` & `meditability-0.2.2/src/smk/pipelines/py/scoring.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Native Modules
 from math import exp
 import pickle
 import re
 # Installed Modules
 import pandas as pd
 import numpy as np
+import tensorflow.compat.v1 as tf1
 from tensorflow.keras.models import load_model
 # Project Modules
 from featurization import featurize_data
+from deepcas_models import DeepCas9
 
 
 def load_model_params(score_name: str, models_dir: str):
     try:
         # dirname = os.path.dirname(os.path.realpath(__file__)).replace('py/','')
         dirname = '/home/thudson/projects/editability'
         if score_name == 'cfd':
@@ -24,24 +26,92 @@
         if score_name == 'doench14':
             doench14params = pickle.load(open(models_dir + '/doench14params.pkl', 'rb'))
             return doench14params
         if score_name == 'deepcpf1':
             model1 = load_model(models_dir + "/DeepCpf1.h5")
             model2 = load_model(models_dir + "/Seq_deepCpf1.h5")
             return model1, model2
+        if score_name == 'deepspcas9':
+            model = DeepCas9
+            #model = pickle.load(open(models_dir + '/DeepCas9.pkl', 'rb'))
+            sess_path = f"{models_dir}/DeepCas9_Final/PreTrain-Final-False-3-5-7-100-70-40-0.001-550-True-80-60"
+            return model, sess_path
     except FileNotFoundError:
         raise Exception(f"File containing {score_name} could not be opened")
 
 
 def revcom(s):
     basecomp = {'A': 'T', 'C': 'G', 'G': 'C', 'T': 'A','U':'A'}
     letters = list(s[::-1])
     letters = [basecomp[base] for base in letters]
     return ''.join(letters)
 
+def preprocess_seq(data):
+    length = 30
+    DATA_X = np.zeros((len(data), 1, length, 4), dtype=int)
+    for l in range(len(data)):
+        for i in range(length):
+            try:
+                data[l][i]
+            except:
+                print(data[l], i, length, len(data))
+
+            if data[l][i] in "Aa":
+                DATA_X[l, 0, i, 0] = 1
+            elif data[l][i] in "Cc":
+                DATA_X[l, 0, i, 1] = 1
+            elif data[l][i] in "Gg":
+                DATA_X[l, 0, i, 2] = 1
+            elif data[l][i] in "Tt":
+                DATA_X[l, 0, i, 3] = 1
+            else:
+                pass
+    return DATA_X
+
+
+##########
+##
+##                   DANIEL MAKE TENSORFLOR STOP YELLING AT ME!!!!
+##   it's giving me some warning about keras conv. layers but still runs
+##
+##########
+
+def deepspcas9(cas9_sites, models_dir):
+    '''
+    Hui Kwon Kim et al. ,SpCas9 activity prediction by DeepSpCas9,
+    a deep learning–based model with high generalization performance.Sci. Adv.5,eaax9249(2019).
+    predicts the likelihood of getting a spCas9 indel at the desired target
+    This script is copied and modified from https://github.com/MyungjaeSong/Paired-Library
+    '''
+    model, sess_path = load_model_params('deepspcas9', models_dir)
+    processed_seqs = preprocess_seq(cas9_sites)
+
+    # TensorFlow config
+    conf = tf1.ConfigProto()
+    conf.gpu_options.allow_growth = True
+    filter_size = [3, 5, 7]
+    filter_num = [100, 70, 40]
+    l_rate, load_episode = 0.001, 550
+    node_1, node_2 = 80, 60
+    tf1.reset_default_graph()
+    scores = np.zeros((processed_seqs.shape[0], 1), dtype=float)
+    test_batch = 500
+    tf1.logging.set_verbosity(tf1.logging.ERROR)
+    with tf1.Session(config=conf) as sess:
+        sess.run(tf1.global_variables_initializer())
+        model = model(filter_size, filter_num, node_1, node_2, l_rate)
+        saver = tf1.train.Saver()
+        saver.restore(sess, sess_path)
+        optimizer = model.optimizer
+        for i in range(int(np.ceil(float(processed_seqs.shape[0]) / float(test_batch)))):
+            Dict = {model.inputs: processed_seqs[i * test_batch:(i + 1) * test_batch], model.is_training: False}
+            scores[i * test_batch:(i + 1) * test_batch] = sess.run([model.outputs], feed_dict=Dict)[0]
+    return scores
+
+
 
 # === On-target Efficiency Scoring ===
 def doench2014(cas9_sites, models_dir):
         """
         Doench 2014 'on-target score'
         Input is a 30mer: 4bp 5', 20bp guide, 3bp PAM, 3bp 5'
         Doench et al, Nat Biotech 2014, PMID 25184501, http://www.broadinstitute.org/rnai/public/analysis-tools/sgrna-design
@@ -314,8 +384,13 @@
 
 seq1, seq2 = 'GTGCGGCTGGCCCAGGACC-T', 'GTGCtGCTacCCCAGGACCCTCGG'
 print('CFD score ',cfd_score(seq1, seq2))
 
 DeepCpf1
 cas12_sites = ['TGACTTTGAATGGAGTCGTGAGCGCAAGAACGCT','GTTATTTGAGCAATGCCACTTAATAAACATGTAA']
 #= [55.437206] [78.50043]
+
+DeepCas9
+cas9_sites = ['TAAGAGAGTGGTAATAGAAGTGCCAGGTAT', 'CCCTCATGGTGCAGCTAAAGGCCCAGGAGC']
+print(deepspcas9(cas9_sites, models_dir))
+#[[67.55651855][56.93091202]]
 '''
```

### Comparing `meditability-0.2.1/src/smk/pipelines/py/validate.py` & `meditability-0.2.2/src/smk/pipelines/py/validate.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.1/src/smk/pipelines/vcf_processing.smk` & `meditability-0.2.2/src/smk/pipelines/vcf_processing.smk`

 * *Files identical despite different names*


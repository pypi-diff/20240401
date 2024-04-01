# Comparing `tmp/autotrain-advanced-0.7.8.tar.gz` & `tmp/autotrain-advanced-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.7.8.tar", last modified: Sat Mar  9 09:41:41 2024, max compression
+gzip compressed data, was "autotrain-advanced-0.7.9.tar", last modified: Sat Mar  9 10:16:49 2024, max compression
```

## Comparing `autotrain-advanced-0.7.8.tar` & `autotrain-advanced-0.7.9.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.211072 autotrain-advanced-0.7.8/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.8/LICENSE
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    11924 2024-03-09 09:41:41.211072 autotrain-advanced-0.7.8/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2433 2024-03-08 09:21:33.000000 autotrain-advanced-0.7.8/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-03-09 09:41:41.215072 autotrain-advanced-0.7.8/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2585 2024-02-29 11:54:14.000000 autotrain-advanced-0.7.8/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.191073 autotrain-advanced-0.7.8/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.195073 autotrain-advanced-0.7.8/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      954 2024-03-09 09:41:32.000000 autotrain-advanced-0.7.8/src/autotrain/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1774 2024-03-08 08:21:06.000000 autotrain-advanced-0.7.8/src/autotrain/api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17396 2024-03-09 07:47:44.000000 autotrain-advanced-0.7.8/src/autotrain/app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5159 2024-02-22 14:54:32.000000 autotrain-advanced-0.7.8/src/autotrain/app_params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5918 2024-02-29 11:39:11.000000 autotrain-advanced-0.7.8/src/autotrain/app_utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    22047 2024-03-09 07:57:49.000000 autotrain-advanced-0.7.8/src/autotrain/backend.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.195073 autotrain-advanced-0.7.8/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.8/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2110 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.8/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1312 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.8/src/autotrain/cli/run_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2136 2023-12-15 13:15:05.000000 autotrain-advanced-0.7.8/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13233 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.8/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6303 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.8/src/autotrain/cli/run_image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14393 2024-02-22 15:15:30.000000 autotrain-advanced-0.7.8/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7510 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.8/src/autotrain/cli/run_seq2seq.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-09 07:52:04.000000 autotrain-advanced-0.7.8/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5224 2023-12-05 20:59:47.000000 autotrain-advanced-0.7.8/src/autotrain/cli/run_spacerunner.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5671 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.8/src/autotrain/cli/run_tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7497 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.8/src/autotrain/cli/run_text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6121 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.8/src/autotrain/cli/run_token_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10880 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.8/src/autotrain/cli/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9719 2024-02-13 17:29:11.000000 autotrain-advanced-0.7.8/src/autotrain/commands.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      309 2023-08-16 09:13:38.000000 autotrain-advanced-0.7.8/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16028 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.8/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-02-14 13:51:37.000000 autotrain-advanced-0.7.8/src/autotrain/db.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-02-21 15:24:07.000000 autotrain-advanced-0.7.8/src/autotrain/help.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1067 2024-02-14 15:04:27.000000 autotrain-advanced-0.7.8/src/autotrain/logging.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4323 2024-02-29 14:19:36.000000 autotrain-advanced-0.7.8/src/autotrain/oauth.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.195073 autotrain-advanced-0.7.8/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.8/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3241 2023-12-20 19:37:58.000000 autotrain-advanced-0.7.8/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.8/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14997 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.8/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7225 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.8/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2449 2024-03-08 08:21:06.000000 autotrain-advanced-0.7.8/src/autotrain/project.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.195073 autotrain-advanced-0.7.8/src/autotrain/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-12-15 11:33:40.000000 autotrain-advanced-0.7.8/src/autotrain/static/logo.png
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2865 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.8/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.195073 autotrain-advanced-0.7.8/src/autotrain/templates/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-02-24 10:09:47.000000 autotrain-advanced-0.7.8/src/autotrain/templates/duplicate.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2023-12-15 11:33:14.000000 autotrain-advanced-0.7.8/src/autotrain/templates/error.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    36074 2024-03-09 07:52:04.000000 autotrain-advanced-0.7.8/src/autotrain/templates/index.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1033 2024-02-29 12:52:07.000000 autotrain-advanced-0.7.8/src/autotrain/templates/login.html
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.195073 autotrain-advanced-0.7.8/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.195073 autotrain-advanced-0.7.8/src/autotrain/trainers/clm/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/clm/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21138 2024-02-23 07:46:34.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/clm/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/clm/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3312 2024-02-22 15:16:12.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/clm/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10791 2024-02-29 12:02:21.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/clm/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5163 2024-02-19 10:34:58.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/common.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.195073 autotrain-advanced-0.7.8/src/autotrain/trainers/dreambooth/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/dreambooth/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13123 2024-03-08 09:54:18.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/dreambooth/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-08 09:54:18.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/dreambooth/datasets.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4071 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/dreambooth/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21920 2023-11-04 11:49:08.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/dreambooth/trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13687 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/dreambooth/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.195073 autotrain-advanced-0.7.8/src/autotrain/trainers/generic/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/generic/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/generic/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      654 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/generic/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3640 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/generic/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.199073 autotrain-advanced-0.7.8/src/autotrain/trainers/image_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/image_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6699 2024-02-26 12:26:15.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/image_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/image_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1945 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/image_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4457 2024-03-08 09:54:18.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/image_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.199073 autotrain-advanced-0.7.8/src/autotrain/trainers/seq2seq/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/seq2seq/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8217 2023-12-21 15:04:54.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/seq2seq/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/seq2seq/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2485 2024-02-22 09:28:57.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/seq2seq/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1642 2023-10-24 15:04:44.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/seq2seq/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.199073 autotrain-advanced-0.7.8/src/autotrain/trainers/tabular/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/tabular/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12525 2023-12-21 18:57:22.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/tabular/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1468 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/tabular/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/tabular/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.199073 autotrain-advanced-0.7.8/src/autotrain/trainers/text_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/text_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7253 2024-01-26 09:52:49.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/text_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/text_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1997 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/text_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3309 2023-08-23 10:09:58.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/text_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.199073 autotrain-advanced-0.7.8/src/autotrain/trainers/token_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/token_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6999 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/token_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/token_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1998 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/token_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1696 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.8/src/autotrain/trainers/token_classification/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6788 2024-02-14 13:51:37.000000 autotrain-advanced-0.7.8/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.199073 autotrain-advanced-0.7.8/src/autotrain_advanced.egg-info/
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    11924 2024-03-09 09:41:41.000000 autotrain-advanced-0.7.8/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3449 2024-03-09 09:41:41.000000 autotrain-advanced-0.7.8/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-03-09 09:41:41.000000 autotrain-advanced-0.7.8/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-03-09 09:41:41.000000 autotrain-advanced-0.7.8/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3129 2024-03-09 09:41:41.000000 autotrain-advanced-0.7.8/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-03-09 09:41:41.000000 autotrain-advanced-0.7.8/src/autotrain_advanced.egg-info/top_level.txt
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 09:41:41.199073 autotrain-advanced-0.7.8/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.8/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.904001 autotrain-advanced-0.7.9/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.9/LICENSE
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    11924 2024-03-09 10:16:49.904001 autotrain-advanced-0.7.9/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2433 2024-03-08 09:21:33.000000 autotrain-advanced-0.7.9/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-03-09 10:16:49.908001 autotrain-advanced-0.7.9/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2585 2024-02-29 11:54:14.000000 autotrain-advanced-0.7.9/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.888002 autotrain-advanced-0.7.9/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.888002 autotrain-advanced-0.7.9/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      954 2024-03-09 10:16:44.000000 autotrain-advanced-0.7.9/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1774 2024-03-08 08:21:06.000000 autotrain-advanced-0.7.9/src/autotrain/api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17396 2024-03-09 07:47:44.000000 autotrain-advanced-0.7.9/src/autotrain/app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5159 2024-02-22 14:54:32.000000 autotrain-advanced-0.7.9/src/autotrain/app_params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5918 2024-02-29 11:39:11.000000 autotrain-advanced-0.7.9/src/autotrain/app_utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    22327 2024-03-09 10:14:16.000000 autotrain-advanced-0.7.9/src/autotrain/backend.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.888002 autotrain-advanced-0.7.9/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.9/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2110 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1312 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2136 2023-12-15 13:15:05.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13233 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6303 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14393 2024-02-22 15:15:30.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7510 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_seq2seq.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-09 07:52:04.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5224 2023-12-05 20:59:47.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_spacerunner.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5671 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7497 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6121 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_token_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10880 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/cli/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9719 2024-02-13 17:29:11.000000 autotrain-advanced-0.7.9/src/autotrain/commands.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      309 2023-08-16 09:13:38.000000 autotrain-advanced-0.7.9/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16028 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-02-14 13:51:37.000000 autotrain-advanced-0.7.9/src/autotrain/db.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-02-21 15:24:07.000000 autotrain-advanced-0.7.9/src/autotrain/help.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1067 2024-02-14 15:04:27.000000 autotrain-advanced-0.7.9/src/autotrain/logging.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4323 2024-02-29 14:19:36.000000 autotrain-advanced-0.7.9/src/autotrain/oauth.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.888002 autotrain-advanced-0.7.9/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.9/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3241 2023-12-20 19:37:58.000000 autotrain-advanced-0.7.9/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.9/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14997 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7225 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.9/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2449 2024-03-08 08:21:06.000000 autotrain-advanced-0.7.9/src/autotrain/project.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.888002 autotrain-advanced-0.7.9/src/autotrain/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-12-15 11:33:40.000000 autotrain-advanced-0.7.9/src/autotrain/static/logo.png
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2865 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/templates/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-02-24 10:09:47.000000 autotrain-advanced-0.7.9/src/autotrain/templates/duplicate.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2023-12-15 11:33:14.000000 autotrain-advanced-0.7.9/src/autotrain/templates/error.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    36074 2024-03-09 07:52:04.000000 autotrain-advanced-0.7.9/src/autotrain/templates/index.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1033 2024-02-29 12:52:07.000000 autotrain-advanced-0.7.9/src/autotrain/templates/login.html
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/clm/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/clm/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21138 2024-02-23 07:46:34.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/clm/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/clm/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3312 2024-02-22 15:16:12.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/clm/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10791 2024-02-29 12:02:21.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/clm/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5163 2024-02-19 10:34:58.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/common.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13123 2024-03-08 09:54:18.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-08 09:54:18.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4071 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21920 2023-11-04 11:49:08.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13687 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/generic/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/generic/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/generic/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      654 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/generic/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3640 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/generic/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6699 2024-02-26 12:26:15.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1945 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4457 2024-03-08 09:54:18.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8217 2023-12-21 15:04:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2485 2024-02-22 09:28:57.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1642 2023-10-24 15:04:44.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12525 2023-12-21 18:57:22.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1468 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7253 2024-01-26 09:52:49.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1997 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3309 2023-08-23 10:09:58.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6999 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1998 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1696 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6788 2024-02-14 13:51:37.000000 autotrain-advanced-0.7.9/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    11924 2024-03-09 10:16:49.000000 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3449 2024-03-09 10:16:49.000000 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-03-09 10:16:49.000000 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-03-09 10:16:49.000000 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3129 2024-03-09 10:16:49.000000 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-03-09 10:16:49.000000 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.9/static/logo.png
```

### Comparing `autotrain-advanced-0.7.8/LICENSE` & `autotrain-advanced-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/PKG-INFO` & `autotrain-advanced-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.8
+Version: 0.7.9
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.7.8/README.md` & `autotrain-advanced-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/setup.py` & `autotrain-advanced-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/__init__.py` & `autotrain-advanced-0.7.9/src/autotrain/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 
 from autotrain.logging import custom_logger as logger  # noqa: F401
 
 
 warnings.filterwarnings("ignore", category=UserWarning, module="tensorflow")
 
 
-__version__ = "0.7.8"
+__version__ = "0.7.9"
```

### Comparing `autotrain-advanced-0.7.8/src/autotrain/api.py` & `autotrain-advanced-0.7.9/src/autotrain/api.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/app.py` & `autotrain-advanced-0.7.9/src/autotrain/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/app_params.py` & `autotrain-advanced-0.7.9/src/autotrain/app_params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/app_utils.py` & `autotrain-advanced-0.7.9/src/autotrain/app_utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/backend.py` & `autotrain-advanced-0.7.9/src/autotrain/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,35 +420,36 @@
             return [self._convert_dict_to_object(item) for item in dictionary]
         else:
             return dictionary
 
     def _conf_nvcf(self, token, nvcf_type, url, method="POST", payload=None):
         logger.info(f"{self.job_name}: {method} - Configuring NVCF {nvcf_type}.")
         headers = {"Content-Type": "application/json", "Authorization": f"Bearer {token}"}
-
+        logger.info(f"Headers: {headers}")
+        logger.info(f"Payload: {payload}")
         try:
             if method.upper() == "POST":
                 response = requests.post(url, headers=headers, json=payload, timeout=30)
             else:
+
                 raise ValueError(f"Unsupported HTTP method: {method}")
 
             response.raise_for_status()
 
             if response.status_code == 202:
                 logger.info(
                     f"{self.job_name}: {method} - Successfully submitted NVCF job. Polling reqId for completion"
                 )
                 response_data = response.json()
                 nvcf_reqid = response_data.get("nvcfRequestId")
                 if nvcf_reqid:
                     logger.info(f"{self.job_name}: nvcfRequestId: {nvcf_reqid}")
                     return nvcf_reqid
-                else:
-                    logger.warning(f"{self.job_name}: nvcfRequestId key is missing in the response body")
-                    return None
+                logger.warning(f"{self.job_name}: nvcfRequestId key is missing in the response body")
+                return None
 
             result = response.json()
             result_obj = self._convert_dict_to_object(result)
             logger.info(f"{self.job_name}: {method} - Successfully processed NVCF {nvcf_type}.")
             return result_obj
 
         except requests.HTTPError as http_err:
@@ -500,14 +501,18 @@
             time.sleep(interval)
 
         if not success:
             raise TimeoutError(f"Operation '{op}' did not complete successfully within the timeout period.")
 
     def create(self):
         nvcf_url_submit = f"{self.nvcf_api}/invoke/{self.instance_map[self.backend]['id']}"
+        org_name = os.environ.get("SPACE_ID")
+        if org_name is None:
+            raise ValueError("SPACE_ID environment variable is not set")
+        org_name = org_name.split("/")[0]
         nvcf_fr_payload = {
             "cmd": [
                 "conda",
                 "run",
                 "-p",
                 "/app/env",
                 "python",
@@ -516,14 +521,15 @@
                 "autotrain.api:api",
                 "--host",
                 "0.0.0.0",
                 "--port",
                 "7860",
             ],
             "env": {key: value for key, value in self.env_vars.items()},
+            "ORG_NAME": org_name,
         }
 
         nvcf_fn_req = self._conf_nvcf(
             token=self.hf_token, nvcf_type="job_submit", url=nvcf_url_submit, method="POST", payload=nvcf_fr_payload
         )
 
         nvcf_url_reqpoll = f"{self.nvcf_api}/status/{nvcf_fn_req}"
```

### Comparing `autotrain-advanced-0.7.8/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/cli/run_api.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_api.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/cli/run_dreambooth.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/cli/run_image_classification.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/cli/run_seq2seq.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_seq2seq.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/cli/run_spacerunner.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_spacerunner.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/cli/run_tabular.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/cli/run_text_classification.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/cli/run_token_classification.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_token_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/cli/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/commands.py` & `autotrain-advanced-0.7.9/src/autotrain/commands.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/dataset.py` & `autotrain-advanced-0.7.9/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/db.py` & `autotrain-advanced-0.7.9/src/autotrain/db.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/help.py` & `autotrain-advanced-0.7.9/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/logging.py` & `autotrain-advanced-0.7.9/src/autotrain/logging.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/oauth.py` & `autotrain-advanced-0.7.9/src/autotrain/oauth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.7.9/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.7.9/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.7.9/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.7.9/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/project.py` & `autotrain-advanced-0.7.9/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/static/logo.png` & `autotrain-advanced-0.7.9/src/autotrain/static/logo.png`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/tasks.py` & `autotrain-advanced-0.7.9/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/templates/duplicate.html` & `autotrain-advanced-0.7.9/src/autotrain/templates/duplicate.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/templates/error.html` & `autotrain-advanced-0.7.9/src/autotrain/templates/error.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/templates/index.html` & `autotrain-advanced-0.7.9/src/autotrain/templates/index.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/templates/login.html` & `autotrain-advanced-0.7.9/src/autotrain/templates/login.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/clm/__main__.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/clm/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/clm/callbacks.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/clm/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/clm/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/clm/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/clm/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/clm/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/common.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/common.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/dreambooth/__main__.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/dreambooth/datasets.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/datasets.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/dreambooth/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/dreambooth/trainer.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/dreambooth/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/generic/__main__.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/generic/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/generic/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/generic/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/generic/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/generic/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/image_classification/__main__.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/image_classification/dataset.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/image_classification/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/image_classification/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/seq2seq/__main__.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/seq2seq/dataset.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/seq2seq/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/seq2seq/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/tabular/__main__.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/tabular/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/tabular/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/text_classification/__main__.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/text_classification/dataset.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/text_classification/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/text_classification/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/token_classification/__main__.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/token_classification/dataset.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/token_classification/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/trainers/token_classification/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.8
+Version: 0.7.9
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.7.8/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.8/static/logo.png` & `autotrain-advanced-0.7.9/static/logo.png`

 * *Files identical despite different names*


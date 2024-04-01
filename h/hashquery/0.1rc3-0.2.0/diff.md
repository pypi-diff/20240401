# Comparing `tmp/hashquery-0.1rc3.tar.gz` & `tmp/hashquery-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashquery-0.1rc3.tar", last modified: Tue Mar 19 02:12:26 2024, max compression
+gzip compressed data, was "hashquery-0.2.0.tar", last modified: Mon Apr  1 19:47:15 2024, max compression
```

## Comparing `hashquery-0.1rc3.tar` & `hashquery-0.2.0.tar`

### file list

```diff
@@ -1,120 +1,131 @@
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.828979 hashquery-0.1rc3/
--rw-r--r--   0 dse        (501) staff       (20)        7 2024-03-07 00:24:07.000000 hashquery-0.1rc3/.gitignore
--rw-r--r--   0 dse        (501) staff       (20)    11357 2024-03-06 22:37:45.000000 hashquery-0.1rc3/LICENSE
--rw-r--r--   0 dse        (501) staff       (20)      387 2024-03-07 00:24:07.000000 hashquery-0.1rc3/Makefile
--rw-r--r--   0 dse        (501) staff       (20)      267 2024-03-19 02:12:26.827736 hashquery-0.1rc3/PKG-INFO
--rw-r--r--   0 dse        (501) staff       (20)     1970 2024-03-06 22:37:45.000000 hashquery-0.1rc3/README.md
--rw-r--r--   0 dse        (501) staff       (20)       13 2024-03-06 22:37:45.000000 hashquery-0.1rc3/README_external.md
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.783648 hashquery-0.1rc3/docs/
--rw-r--r--   0 dse        (501) staff       (20)        8 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/.gitignore
--rw-r--r--   0 dse        (501) staff       (20)      138 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/Makefile
--rw-r--r--   0 dse        (501) staff       (20)      488 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/README.md
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.784114 hashquery-0.1rc3/docs/_fragments/
--rw-r--r--   0 dse        (501) staff       (20)      325 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/_fragments/alpha_notice.md
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.784548 hashquery-0.1rc3/docs/_static/
--rw-r--r--   0 dse        (501) staff       (20)        0 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/_static/.gitkeep
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.784768 hashquery-0.1rc3/docs/_static/css/
--rw-r--r--   0 dse        (501) staff       (20)     1391 2024-03-13 18:00:28.000000 hashquery-0.1rc3/docs/_static/css/overrides.css
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.786336 hashquery-0.1rc3/docs/_static/js/
--rw-r--r--   0 dse        (501) staff       (20)   161921 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/_static/js/jquery.js
--rw-r--r--   0 dse        (501) staff       (20)      396 2024-03-13 18:00:28.000000 hashquery-0.1rc3/docs/_static/js/markup.js
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.788513 hashquery-0.1rc3/docs/api_reference/
--rw-r--r--   0 dse        (501) staff       (20)      340 2024-03-13 20:00:19.000000 hashquery-0.1rc3/docs/api_reference/0_model.md
--rw-r--r--   0 dse        (501) staff       (20)      223 2024-03-13 20:00:19.000000 hashquery-0.1rc3/docs/api_reference/1_column_expression.md
--rw-r--r--   0 dse        (501) staff       (20)      373 2024-03-13 20:00:19.000000 hashquery-0.1rc3/docs/api_reference/2_func.md
--rw-r--r--   0 dse        (501) staff       (20)      204 2024-03-13 20:00:19.000000 hashquery-0.1rc3/docs/api_reference/3_project.md
--rw-r--r--   0 dse        (501) staff       (20)      817 2024-03-13 20:00:19.000000 hashquery-0.1rc3/docs/api_reference/4_keypath.md
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.789201 hashquery-0.1rc3/docs/concept_explanations/
--rw-r--r--   0 dse        (501) staff       (20)       49 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/concept_explanations/keypaths.md
--rw-r--r--   0 dse        (501) staff       (20)       24 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/concept_explanations/stub.md
--rw-r--r--   0 dse        (501) staff       (20)     2125 2024-03-19 02:11:08.000000 hashquery-0.1rc3/docs/conf.py
--rw-r--r--   0 dse        (501) staff       (20)      549 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/index.md
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.789660 hashquery-0.1rc3/docs/pattern_guides/
--rw-r--r--   0 dse        (501) staff       (20)       24 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/pattern_guides/stub.md
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.791766 hashquery-0.1rc3/docs/project_info/
--rw-r--r--   0 dse        (501) staff       (20)       14 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/project_info/development.md
--rw-r--r--   0 dse        (501) staff       (20)       21 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/project_info/feedback.md
--rw-r--r--   0 dse        (501) staff       (20)     1546 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/project_info/roadmap.md
--rw-r--r--   0 dse        (501) staff       (20)       67 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/requirements.txt
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.796509 hashquery-0.1rc3/docs/setup_tutorial/
--rw-r--r--   0 dse        (501) staff       (20)      375 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/setup_tutorial/0_requirements.md
--rw-r--r--   0 dse        (501) staff       (20)      809 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/setup_tutorial/1_install.md
--rw-r--r--   0 dse        (501) staff       (20)     2352 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/setup_tutorial/2_authentication.md
--rw-r--r--   0 dse        (501) staff       (20)     4999 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/setup_tutorial/3_first_analysis.md
--rw-r--r--   0 dse        (501) staff       (20)      356 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/setup_tutorial/first_analysis_0.py
--rw-r--r--   0 dse        (501) staff       (20)      458 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/setup_tutorial/first_analysis_1.py
--rw-r--r--   0 dse        (501) staff       (20)      578 2024-03-06 22:37:45.000000 hashquery-0.1rc3/docs/setup_tutorial/first_analysis_2.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.826490 hashquery-0.1rc3/hashquery.egg-info/
--rw-r--r--   0 dse        (501) staff       (20)      267 2024-03-19 02:12:25.000000 hashquery-0.1rc3/hashquery.egg-info/PKG-INFO
--rw-r--r--   0 dse        (501) staff       (20)     2697 2024-03-19 02:12:26.000000 hashquery-0.1rc3/hashquery.egg-info/SOURCES.txt
--rw-r--r--   0 dse        (501) staff       (20)        1 2024-03-19 02:12:25.000000 hashquery-0.1rc3/hashquery.egg-info/dependency_links.txt
--rw-r--r--   0 dse        (501) staff       (20)       42 2024-03-19 02:12:25.000000 hashquery-0.1rc3/hashquery.egg-info/requires.txt
--rw-r--r--   0 dse        (501) staff       (20)       10 2024-03-19 02:12:25.000000 hashquery-0.1rc3/hashquery.egg-info/top_level.txt
--rw-r--r--   0 dse        (501) staff       (20)      401 2024-03-19 02:11:53.000000 hashquery-0.1rc3/pyproject.toml
--rw-r--r--   0 dse        (501) staff       (20)       38 2024-03-19 02:12:26.829268 hashquery-0.1rc3/setup.cfg
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.798804 hashquery-0.1rc3/src/
--rw-r--r--   0 dse        (501) staff       (20)      300 2024-03-18 20:57:02.000000 hashquery-0.1rc3/src/__init__.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.799982 hashquery-0.1rc3/src/demo/
--rw-r--r--   0 dse        (501) staff       (20)       62 2024-03-18 15:50:28.000000 hashquery-0.1rc3/src/demo/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)      605 2024-03-19 02:11:05.000000 hashquery-0.1rc3/src/demo/project.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.801822 hashquery-0.1rc3/src/func/
--rw-r--r--   0 dse        (501) staff       (20)      489 2024-03-18 20:57:02.000000 hashquery-0.1rc3/src/func/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)     1232 2024-03-13 20:00:19.000000 hashquery-0.1rc3/src/func/_cases.py
--rw-r--r--   0 dse        (501) staff       (20)      702 2024-03-18 20:57:02.000000 hashquery-0.1rc3/src/func/_logical.py
--rw-r--r--   0 dse        (501) staff       (20)     2121 2024-03-13 20:00:19.000000 hashquery-0.1rc3/src/func/_sql_functions.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.804346 hashquery-0.1rc3/src/hashboard_api/
--rw-r--r--   0 dse        (501) staff       (20)        0 2024-03-06 22:37:45.000000 hashquery-0.1rc3/src/hashboard_api/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)     1905 2024-03-18 16:25:20.000000 hashquery-0.1rc3/src/hashboard_api/api.py
--rw-r--r--   0 dse        (501) staff       (20)     4659 2024-03-18 16:25:04.000000 hashquery-0.1rc3/src/hashboard_api/credentials.py
--rw-r--r--   0 dse        (501) staff       (20)     1179 2024-03-18 20:57:02.000000 hashquery-0.1rc3/src/hashboard_api/default_project.py
--rw-r--r--   0 dse        (501) staff       (20)     1399 2024-03-18 15:50:28.000000 hashquery-0.1rc3/src/hashboard_api/project_importer.py
--rw-r--r--   0 dse        (501) staff       (20)     5468 2024-03-18 15:50:28.000000 hashquery-0.1rc3/src/hashboard_api/project_manifest.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.807451 hashquery-0.1rc3/src/model/
--rw-r--r--   0 dse        (501) staff       (20)        0 2024-03-06 22:37:45.000000 hashquery-0.1rc3/src/model/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)      945 2024-03-18 20:57:02.000000 hashquery-0.1rc3/src/model/accessors.py
--rw-r--r--   0 dse        (501) staff       (20)     1283 2024-03-18 20:57:02.000000 hashquery-0.1rc3/src/model/activity_schema.py
--rw-r--r--   0 dse        (501) staff       (20)     2053 2024-03-13 20:00:19.000000 hashquery-0.1rc3/src/model/column.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.811905 hashquery-0.1rc3/src/model/column_expression/
--rw-r--r--   0 dse        (501) staff       (20)      388 2024-03-06 22:37:45.000000 hashquery-0.1rc3/src/model/column_expression/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)     1408 2024-03-06 22:37:45.000000 hashquery-0.1rc3/src/model/column_expression/binary_op.py
--rw-r--r--   0 dse        (501) staff       (20)     1698 2024-03-16 03:11:06.000000 hashquery-0.1rc3/src/model/column_expression/cases.py
--rw-r--r--   0 dse        (501) staff       (20)    11928 2024-03-18 20:57:02.000000 hashquery-0.1rc3/src/model/column_expression/column_expression.py
--rw-r--r--   0 dse        (501) staff       (20)     1467 2024-03-14 14:40:59.000000 hashquery-0.1rc3/src/model/column_expression/column_name.py
--rw-r--r--   0 dse        (501) staff       (20)     1240 2024-03-06 22:37:45.000000 hashquery-0.1rc3/src/model/column_expression/granularity.py
--rw-r--r--   0 dse        (501) staff       (20)     1287 2024-03-13 20:00:19.000000 hashquery-0.1rc3/src/model/column_expression/py_value.py
--rw-r--r--   0 dse        (501) staff       (20)     2698 2024-03-18 20:57:02.000000 hashquery-0.1rc3/src/model/column_expression/sql_function.py
--rw-r--r--   0 dse        (501) staff       (20)     1141 2024-03-13 20:00:19.000000 hashquery-0.1rc3/src/model/column_expression/sql_text.py
--rw-r--r--   0 dse        (501) staff       (20)      181 2024-03-18 15:50:28.000000 hashquery-0.1rc3/src/model/data_connection.py
--rw-r--r--   0 dse        (501) staff       (20)    29434 2024-03-19 02:11:08.000000 hashquery-0.1rc3/src/model/model.py
--rw-r--r--   0 dse        (501) staff       (20)     2184 2024-03-14 14:40:59.000000 hashquery-0.1rc3/src/model/namespace.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.816738 hashquery-0.1rc3/src/model/source/
--rw-r--r--   0 dse        (501) staff       (20)      374 2024-03-18 15:50:28.000000 hashquery-0.1rc3/src/model/source/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)     1406 2024-03-08 13:39:09.000000 hashquery-0.1rc3/src/model/source/aggregate.py
--rw-r--r--   0 dse        (501) staff       (20)      957 2024-03-08 13:39:09.000000 hashquery-0.1rc3/src/model/source/filter.py
--rw-r--r--   0 dse        (501) staff       (20)     1523 2024-03-11 18:45:43.000000 hashquery-0.1rc3/src/model/source/join_one.py
--rw-r--r--   0 dse        (501) staff       (20)      953 2024-03-18 20:57:02.000000 hashquery-0.1rc3/src/model/source/limit.py
--rw-r--r--   0 dse        (501) staff       (20)     1111 2024-03-11 18:45:43.000000 hashquery-0.1rc3/src/model/source/match_steps.py
--rw-r--r--   0 dse        (501) staff       (20)      988 2024-03-08 13:39:09.000000 hashquery-0.1rc3/src/model/source/pick.py
--rw-r--r--   0 dse        (501) staff       (20)     1181 2024-03-19 02:11:08.000000 hashquery-0.1rc3/src/model/source/sort.py
--rw-r--r--   0 dse        (501) staff       (20)     1371 2024-03-16 03:11:06.000000 hashquery-0.1rc3/src/model/source/source.py
--rw-r--r--   0 dse        (501) staff       (20)      709 2024-03-06 22:37:45.000000 hashquery-0.1rc3/src/model/source/sql_text.py
--rw-r--r--   0 dse        (501) staff       (20)     1032 2024-03-13 20:00:19.000000 hashquery-0.1rc3/src/model/source/table_name.py
--rw-r--r--   0 dse        (501) staff       (20)      903 2024-03-18 15:50:28.000000 hashquery-0.1rc3/src/model/source/union.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.818022 hashquery-0.1rc3/src/run/
--rw-r--r--   0 dse        (501) staff       (20)        0 2024-03-06 22:37:45.000000 hashquery-0.1rc3/src/run/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)     1894 2024-03-19 02:11:08.000000 hashquery-0.1rc3/src/run/post_run_endpoint.py
--rw-r--r--   0 dse        (501) staff       (20)     4184 2024-03-19 02:11:08.000000 hashquery-0.1rc3/src/run/run_results.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.821879 hashquery-0.1rc3/src/utils/
--rw-r--r--   0 dse        (501) staff       (20)        0 2024-03-06 22:37:45.000000 hashquery-0.1rc3/src/utils/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)      720 2024-03-14 14:40:59.000000 hashquery-0.1rc3/src/utils/builder.py
--rw-r--r--   0 dse        (501) staff       (20)     1028 2024-03-13 18:00:28.000000 hashquery-0.1rc3/src/utils/date_shift.py
--rw-r--r--   0 dse        (501) staff       (20)      872 2024-03-16 03:11:06.000000 hashquery-0.1rc3/src/utils/env.py
--rw-r--r--   0 dse        (501) staff       (20)     2062 2024-03-14 14:40:59.000000 hashquery-0.1rc3/src/utils/identifiable.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-03-19 02:12:26.825641 hashquery-0.1rc3/src/utils/keypath/
--rw-r--r--   0 dse        (501) staff       (20)      644 2024-03-06 22:37:45.000000 hashquery-0.1rc3/src/utils/keypath/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)     8520 2024-03-14 14:40:59.000000 hashquery-0.1rc3/src/utils/keypath/keypath.py
--rw-r--r--   0 dse        (501) staff       (20)      443 2024-03-14 14:40:59.000000 hashquery-0.1rc3/src/utils/keypath/keypath_ctx.py
--rw-r--r--   0 dse        (501) staff       (20)     6672 2024-03-14 14:40:59.000000 hashquery-0.1rc3/src/utils/keypath/resolve.py
--rw-r--r--   0 dse        (501) staff       (20)      746 2024-03-06 22:37:45.000000 hashquery-0.1rc3/src/utils/keypath/unwrap.py
--rw-r--r--   0 dse        (501) staff       (20)      744 2024-03-18 15:50:28.000000 hashquery-0.1rc3/src/utils/resource.py
--rw-r--r--   0 dse        (501) staff       (20)     4819 2024-03-19 02:11:08.000000 hashquery-0.1rc3/src/utils/serializable.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.637184 hashquery-0.2.0/
+-rw-r--r--   0 charlie    (501) staff       (20)        7 2024-03-08 01:32:07.000000 hashquery-0.2.0/.gitignore
+-rw-r--r--   0 charlie    (501) staff       (20)    11357 2024-03-08 01:32:07.000000 hashquery-0.2.0/LICENSE
+-rw-r--r--   0 charlie    (501) staff       (20)      387 2024-03-08 01:32:07.000000 hashquery-0.2.0/Makefile
+-rw-r--r--   0 charlie    (501) staff       (20)      266 2024-04-01 19:47:15.636942 hashquery-0.2.0/PKG-INFO
+-rw-r--r--   0 charlie    (501) staff       (20)     1970 2024-03-08 01:32:07.000000 hashquery-0.2.0/README.md
+-rw-r--r--   0 charlie    (501) staff       (20)     4209 2024-03-20 15:23:35.000000 hashquery-0.2.0/README_external.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.625507 hashquery-0.2.0/docs/
+-rw-r--r--   0 charlie    (501) staff       (20)        8 2024-03-08 01:32:07.000000 hashquery-0.2.0/docs/.gitignore
+-rw-r--r--   0 charlie    (501) staff       (20)      138 2024-03-08 01:32:07.000000 hashquery-0.2.0/docs/Makefile
+-rw-r--r--   0 charlie    (501) staff       (20)      488 2024-03-08 01:32:07.000000 hashquery-0.2.0/docs/README.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.625738 hashquery-0.2.0/docs/_fragments/
+-rw-r--r--   0 charlie    (501) staff       (20)      646 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/_fragments/alpha_notice.md
+-rw-r--r--   0 charlie    (501) staff       (20)      381 2024-03-20 15:23:35.000000 hashquery-0.2.0/docs/_fragments/quickstart_smoke_test.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.625851 hashquery-0.2.0/docs/_static/
+-rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.0/docs/_static/.gitkeep
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.625951 hashquery-0.2.0/docs/_static/css/
+-rw-r--r--   0 charlie    (501) staff       (20)     3849 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/_static/css/overrides.css
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.626420 hashquery-0.2.0/docs/_static/js/
+-rw-r--r--   0 charlie    (501) staff       (20)     2678 2024-03-20 15:23:35.000000 hashquery-0.2.0/docs/_static/js/analytics.js
+-rw-r--r--   0 charlie    (501) staff       (20)   161921 2024-03-08 01:32:07.000000 hashquery-0.2.0/docs/_static/js/jquery.js
+-rw-r--r--   0 charlie    (501) staff       (20)      396 2024-03-18 18:49:18.000000 hashquery-0.2.0/docs/_static/js/markup.js
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.627019 hashquery-0.2.0/docs/api_reference/
+-rw-r--r--   0 charlie    (501) staff       (20)      340 2024-03-14 15:01:43.000000 hashquery-0.2.0/docs/api_reference/0_model.md
+-rw-r--r--   0 charlie    (501) staff       (20)      223 2024-03-14 15:01:43.000000 hashquery-0.2.0/docs/api_reference/1_column_expression.md
+-rw-r--r--   0 charlie    (501) staff       (20)      373 2024-03-14 15:01:43.000000 hashquery-0.2.0/docs/api_reference/2_func.md
+-rw-r--r--   0 charlie    (501) staff       (20)      219 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/api_reference/3_project.md
+-rw-r--r--   0 charlie    (501) staff       (20)      721 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/api_reference/4_keypath.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.627389 hashquery-0.2.0/docs/concept_explanations/
+-rw-r--r--   0 charlie    (501) staff       (20)     1044 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/concept_explanations/0_models.md
+-rw-r--r--   0 charlie    (501) staff       (20)      143 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/concept_explanations/1_column_expressions.md
+-rw-r--r--   0 charlie    (501) staff       (20)     6971 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/concept_explanations/z_advanced_keypaths.md
+-rw-r--r--   0 charlie    (501) staff       (20)     2328 2024-03-20 15:23:35.000000 hashquery-0.2.0/docs/conf.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.627626 hashquery-0.2.0/docs/hashboard_intg/
+-rw-r--r--   0 charlie    (501) staff       (20)     2057 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/hashboard_intg/0_import.md
+-rw-r--r--   0 charlie    (501) staff       (20)      234 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/hashboard_intg/dataops.md
+-rw-r--r--   0 charlie    (501) staff       (20)     1302 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/index.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.628276 hashquery-0.2.0/docs/pattern_guides/
+-rw-r--r--   0 charlie    (501) staff       (20)     1135 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/pattern_guides/binning.md
+-rw-r--r--   0 charlie    (501) staff       (20)     7039 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/pattern_guides/events.md
+-rw-r--r--   0 charlie    (501) staff       (20)     1202 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/pattern_guides/joins.md
+-rw-r--r--   0 charlie    (501) staff       (20)     1257 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/pattern_guides/segments.md
+-rw-r--r--   0 charlie    (501) staff       (20)     1356 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/pattern_guides/timeframes.md
+-rw-r--r--   0 charlie    (501) staff       (20)      748 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/pattern_guides/visualizations.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.628492 hashquery-0.2.0/docs/project_info/
+-rw-r--r--   0 charlie    (501) staff       (20)       21 2024-03-18 17:09:06.000000 hashquery-0.2.0/docs/project_info/feedback.md
+-rw-r--r--   0 charlie    (501) staff       (20)      609 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/project_info/roadmap.md
+-rw-r--r--   0 charlie    (501) staff       (20)       67 2024-03-08 01:32:07.000000 hashquery-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.629151 hashquery-0.2.0/docs/setup_tutorial/
+-rw-r--r--   0 charlie    (501) staff       (20)     2905 2024-03-20 15:23:35.000000 hashquery-0.2.0/docs/setup_tutorial/1_quickstart.md
+-rw-r--r--   0 charlie    (501) staff       (20)     4519 2024-03-20 15:23:35.000000 hashquery-0.2.0/docs/setup_tutorial/2_first_analysis.md
+-rw-r--r--   0 charlie    (501) staff       (20)     1813 2024-03-21 17:47:59.000000 hashquery-0.2.0/docs/setup_tutorial/3_authentication.md
+-rw-r--r--   0 charlie    (501) staff       (20)      284 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/setup_tutorial/first_analysis_0.py
+-rw-r--r--   0 charlie    (501) staff       (20)      377 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/setup_tutorial/first_analysis_1.py
+-rw-r--r--   0 charlie    (501) staff       (20)      508 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/setup_tutorial/first_analysis_2.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.636642 hashquery-0.2.0/hashquery.egg-info/
+-rw-r--r--   0 charlie    (501) staff       (20)      266 2024-04-01 19:47:15.000000 hashquery-0.2.0/hashquery.egg-info/PKG-INFO
+-rw-r--r--   0 charlie    (501) staff       (20)     3065 2024-04-01 19:47:15.000000 hashquery-0.2.0/hashquery.egg-info/SOURCES.txt
+-rw-r--r--   0 charlie    (501) staff       (20)        1 2024-04-01 19:47:15.000000 hashquery-0.2.0/hashquery.egg-info/dependency_links.txt
+-rw-r--r--   0 charlie    (501) staff       (20)       42 2024-04-01 19:47:15.000000 hashquery-0.2.0/hashquery.egg-info/requires.txt
+-rw-r--r--   0 charlie    (501) staff       (20)       10 2024-04-01 19:47:15.000000 hashquery-0.2.0/hashquery.egg-info/top_level.txt
+-rw-r--r--   0 charlie    (501) staff       (20)      400 2024-04-01 19:46:34.000000 hashquery-0.2.0/pyproject.toml
+-rw-r--r--   0 charlie    (501) staff       (20)       38 2024-04-01 19:47:15.637226 hashquery-0.2.0/setup.cfg
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.629760 hashquery-0.2.0/src/
+-rw-r--r--   0 charlie    (501) staff       (20)      300 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/__init__.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.629975 hashquery-0.2.0/src/demo/
+-rw-r--r--   0 charlie    (501) staff       (20)       62 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/demo/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)      861 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/demo/project.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.630442 hashquery-0.2.0/src/func/
+-rw-r--r--   0 charlie    (501) staff       (20)      489 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/func/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1232 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/func/_cases.py
+-rw-r--r--   0 charlie    (501) staff       (20)      702 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/func/_logical.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2121 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/func/_sql_functions.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.631121 hashquery-0.2.0/src/hashboard_api/
+-rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/hashboard_api/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1905 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/hashboard_api/api.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4659 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/hashboard_api/credentials.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1214 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/hashboard_api/default_project.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2074 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/hashboard_api/project_importer.py
+-rw-r--r--   0 charlie    (501) staff       (20)     6334 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/hashboard_api/project_manifest.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.631979 hashquery-0.2.0/src/model/
+-rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/model/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)      945 2024-03-27 19:20:01.000000 hashquery-0.2.0/src/model/accessors.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1283 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/activity_schema.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2355 2024-04-01 19:00:43.000000 hashquery-0.2.0/src/model/column.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.633210 hashquery-0.2.0/src/model/column_expression/
+-rw-r--r--   0 charlie    (501) staff       (20)      446 2024-03-27 21:43:29.000000 hashquery-0.2.0/src/model/column_expression/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1562 2024-04-01 19:00:43.000000 hashquery-0.2.0/src/model/column_expression/binary_op.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1698 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/column_expression/cases.py
+-rw-r--r--   0 charlie    (501) staff       (20)    19869 2024-04-01 19:00:43.000000 hashquery-0.2.0/src/model/column_expression/column_expression.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1467 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/model/column_expression/column_name.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1240 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/model/column_expression/granularity.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1287 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/model/column_expression/py_value.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2698 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/column_expression/sql_function.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4294 2024-04-01 19:00:43.000000 hashquery-0.2.0/src/model/column_expression/sql_text.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1139 2024-03-27 21:43:29.000000 hashquery-0.2.0/src/model/column_expression/subquery_expression.py
+-rw-r--r--   0 charlie    (501) staff       (20)      181 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/data_connection.py
+-rw-r--r--   0 charlie    (501) staff       (20)    30027 2024-04-01 19:00:43.000000 hashquery-0.2.0/src/model/model.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2184 2024-03-27 19:19:55.000000 hashquery-0.2.0/src/model/namespace.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.634611 hashquery-0.2.0/src/model/source/
+-rw-r--r--   0 charlie    (501) staff       (20)      374 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/source/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1406 2024-03-08 02:35:55.000000 hashquery-0.2.0/src/model/source/aggregate.py
+-rw-r--r--   0 charlie    (501) staff       (20)      957 2024-03-08 02:35:55.000000 hashquery-0.2.0/src/model/source/filter.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1523 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/model/source/join_one.py
+-rw-r--r--   0 charlie    (501) staff       (20)      953 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/source/limit.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1111 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/model/source/match_steps.py
+-rw-r--r--   0 charlie    (501) staff       (20)      988 2024-03-08 02:35:55.000000 hashquery-0.2.0/src/model/source/pick.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1181 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/model/source/sort.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1371 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/source/source.py
+-rw-r--r--   0 charlie    (501) staff       (20)      709 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/model/source/sql_text.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1032 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/model/source/table_name.py
+-rw-r--r--   0 charlie    (501) staff       (20)      903 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/source/union.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.634937 hashquery-0.2.0/src/run/
+-rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/run/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1894 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/run/post_run_endpoint.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4034 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/run/run_results.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.635866 hashquery-0.2.0/src/utils/
+-rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/utils/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)      720 2024-03-27 20:58:55.000000 hashquery-0.2.0/src/utils/builder.py
+-rw-r--r--   0 charlie    (501) staff       (20)      872 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/utils/env.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2062 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/utils/identifiable.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.636484 hashquery-0.2.0/src/utils/keypath/
+-rw-r--r--   0 charlie    (501) staff       (20)      644 2024-03-21 15:14:14.000000 hashquery-0.2.0/src/utils/keypath/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     8520 2024-03-21 15:14:14.000000 hashquery-0.2.0/src/utils/keypath/keypath.py
+-rw-r--r--   0 charlie    (501) staff       (20)      443 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/utils/keypath/keypath_ctx.py
+-rw-r--r--   0 charlie    (501) staff       (20)     6705 2024-04-01 19:28:53.000000 hashquery-0.2.0/src/utils/keypath/resolve.py
+-rw-r--r--   0 charlie    (501) staff       (20)      746 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/utils/keypath/unwrap.py
+-rw-r--r--   0 charlie    (501) staff       (20)      744 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/utils/resource.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4809 2024-04-01 19:00:43.000000 hashquery-0.2.0/src/utils/serializable.py
+-rw-r--r--   0 charlie    (501) staff       (20)      662 2024-03-27 16:32:34.000000 hashquery-0.2.0/src/utils/timeinterval.py
+-rw-r--r--   0 charlie    (501) staff       (20)      106 2024-03-27 21:43:29.000000 hashquery-0.2.0/src/utils/types.py
```

### Comparing `hashquery-0.1rc3/LICENSE` & `hashquery-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/README.md` & `hashquery-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/docs/_static/js/jquery.js` & `hashquery-0.2.0/docs/_static/js/jquery.js`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/docs/conf.py` & `hashquery-0.2.0/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,8 +62,13 @@
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "sphinx_rtd_theme"
 html_static_path = ["_static"]
 html_css_files = ["css/overrides.css"]
-html_js_files = ["js/jquery.js", "js/markup.js"]
+html_js_files = ["js/jquery.js", "js/markup.js", "js/analytics.js"]
+html_theme_options = {
+    # options here:
+    # https://sphinx-rtd-theme.readthedocs.io/en/latest/configuring.html
+    # the defaults are fine; they don't give us much to work with
+}
```

### Comparing `hashquery-0.1rc3/docs/index.md` & `hashquery-0.2.0/docs/index.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 # Hashquery
 
-Hashquery is a tool for modeling complex analysis inside of [Hashboard](https://www.hashboard.com).
+## A Python framework for modeling and querying business data inside of your data warehouse
+
+Logic shouldn’t be trapped in any tool, especially not your BI tool.
+But data teams are often forced to choose between doing their modeling with proprietary
+DSLs like LookML or adding complex business logic into raw SQL, where it can't be
+easily re-used or extended. That’s why we’re building **hashquery**.
+
+Hashquery expressions are defined in Python, compiled into SQL, and run directly
+against your data warehouse. It is capable of expressing complex, multi-layered
+data queries, way beyond the capabilities of standard SQL.
+It natively integrates with upstream semantic layers.
+And unlike a DSL, hashquery is fully composable and extensible — it’s just Python.
 
 ```{include} /_fragments/alpha_notice.md
 
 ```
 
 ```{toctree}
 :caption: Getting Started
@@ -27,14 +38,22 @@
 :glob:
 :hidden:
 
 pattern_guides/*
 ```
 
 ```{toctree}
+:caption: Hashboard Integration
+:glob:
+:hidden:
+
+hashboard_intg/*
+```
+
+```{toctree}
 :caption: API Reference
 :glob:
 :maxdepth: 1
 :hidden:
 
 api_reference/*
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hashquery-0.1rc3/docs/setup_tutorial/3_first_analysis.md` & `hashquery-0.2.0/docs/setup_tutorial/2_first_analysis.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # Your first analysis
 
 ```{eval-rst}
 .. currentmodule:: hashquery
 ```
 
-Your first query will depend on the data you have access to,
-but this should serve as a simple guide to get you started.
+This first query will use the demo project to get started.
 
-:::{note}
-Values in this code that will need to be changed based on your data
-will appear in UPPERCASE in the Python snippets below.
-:::
+You can choose to adapt this to your data if you choose. If you get stuck importing
+some content from your project, try `print(project)` to show all your project's
+content.
 
 ## Getting the count of items
 
 Let's start simple. We'll import a connection, and count the amount of records
 in a table.
 
 First, let's import our connection. This does not actually connect to your data
@@ -22,137 +20,125 @@
 used later on.
 
 ```{literalinclude} first_analysis_0.py
 :end-at: connection =
 :lineno-match:
 ```
 
-:::{dropdown} Failing to load the connection?
-
-Use the following to print all the names of valid connections:
-
-```python
-from hashquery import *
-from hashquery.project_importer import ProjectImporter
-
-connections = ProjectImporter().all_data_connections()
-print("Data connections:")
-print([dc.alias for dc in connections])
-```
-
-:::
-
 Next, we'll define a simple {py:class}`Model` for a table. This model represents
-all the records in the table named `TABLE_NAME`.
+all the records in the table named `sales.parquet`.
 
 ```{literalinclude} first_analysis_0.py
-:start-at: table_model =
-:end-at: table_model =
+:start-at: sales =
+:end-at: sales =
 :lineno-match:
 ```
 
 Let's now sub-model this to form a new model. While the previous model
 represented _all records_ in the table, this new model will represent
 the total count of the records in the table.
 
 We can do so by calling {py:func}`Model.aggregate` with no groups, and a single
-measure: {py:func}`count`.
+measure: {py:func}`func.count`.
 
 ```{literalinclude} first_analysis_0.py
-:start-at: count_model =
-:end-at: count_model =
+:start-at: total_sales =
+:end-at: total_sales =
 :lineno-match:
 ```
 
-Finally, we'll execute the model:
+Finally, we'll run the model ({py:func}`Model.run`) and collect the result
+as a Pandas DataFrame ({py:attr}`~Model.df`):
 
 ```{literalinclude} first_analysis_0.py
-:start-at: results =
+:start-at: print
 :lineno-match:
 ```
 
 When you run this script, you should should see a printed item containing a
 value for the count of records in the table.
 
+If you want to see the SQL that ran, you can reference `.sql_query` on the
+value returned by {py:func}`Model.run`:
+
+```python
+result = total_sales.run()
+print(result.sql_query) # the query
+print(result.df) # the data
+```
+
 :::{dropdown} Code so far
 
 ```{literalinclude} first_analysis_0.py
 :linenos:
 ```
 
 :::
 
 ## Breaking out by groups
 
 Let's revisit our analysis. Instead of gathering a count of all records,
-let's group the records into buckets, and count the totals within each bucket.
-We'll then take the top 3 largest buckets.
-
-Pick a column that the data may be split on well. If you choose a date column,
-instead of specifying `column("COLUMN_NAME")`, use
-`column("COLUMN_NAME").by_month` to truncate the timestamps into months.
+let's group the records into buckets by year, and count the totals within
+each bucket.
 
 ```{literalinclude} first_analysis_1.py
-:start-at: top_counts_model =
-:lines: -8
+:start-at: sales_by_year =
 :lineno-match:
 ```
 
-This should now show you the top 3 buckets.
+This should now show you the top 3 years on record.
 
 :::{dropdown} Code so far
 
 ```{literalinclude} first_analysis_1.py
 :linenos:
 ```
 
 :::
 
 ## Modeling & referencing properties
 
 Our queries work well, but they aren't very reusable. Anytime somebody needs
-to reference your columns, they need to find the physical name of the column
-in the database table, which could change and result in a cascade of changes.
+to reference the columns, they need to find the physical name of the column
+in the database table, which could change.
 Similarly, our measure may become more complex, accounting for business logic
 about double counting, and if the logic was spread across many queries, you
 would have to update it in many places.
 
 What we want to do is have a layer between the raw expressions and the
 semantics of the model. We'll use the model as a centralized, shared definition
 of what's interesting about the table.
 
 For this tutorial, we'll just attach attributes and measures.
 
 - **Attributes** are expressions which are a property of _an individual record_.
 - **Measures** are expressions which are a property of _a group of records_.
 
 You can attach attributes and measures onto a model using
-{py:func}`Model.with_attribute` and {py:func}`Model.with_measure` respectively.
+{py:func}`Model.with_attributes` and {py:func}`Model.with_measures` respectively.
 We'll attach these to our base model, so any analysis using this table can
 reuse them.
 
 ```{literalinclude} first_analysis_2.py
-:start-at: table_model =
+:start-at: sales =
 :lines: -6
 :lineno-match:
 ```
 
 We can then update our references in our sub-model to use the new definitions.
-In HashQuery, we reference properties on models using the `_` operator.
-The `_` operator [is covered in more detail here](/concept_explanations/keypaths.md).
-For now, imagine `_` as a magic reference to "the model I am querying".
+In HashQuery, we reference attributes on models using `attr.`, measures using
+`msr.` and relations using `rel.`.
 
 ```{literalinclude} first_analysis_2.py
-:start-at: top_counts_model =
-:lines: -8
+:start-at: sales_by_year =
 :lineno-match:
 ```
 
 Now our sub-model query will automatically adjust if we change the definition
-for `my_attribute` or `my_measure`. In addition, `table_model` now has more
+for `my_attribute` or `my_measure`. In addition, `sales` now has more
 metadata about what's interesting about the table, which allows tools in
 Hashboard to offer better UIs for non-technical consumers of your data.
 
 :::{dropdown} Final code
 
 ```{literalinclude} first_analysis_2.py
 :linenos:
@@ -162,9 +148,8 @@
 
 ## Next Steps
 
 You can learn about the core concepts and principles of Hashquery under the
 **Concepts** sidebar. For further examples, check out **Common Patterns**. API
 documentation can be found under **API Reference**.
 
-Have fun querying! [Please let us know if you have any feedback, or
-encounter any issues](/project_info/feedback.md).
+Have fun querying! [Please let us know if you have any feedback, or encounter any issues](/project_info/feedback.md).
```

### Comparing `hashquery-0.1rc3/hashquery.egg-info/SOURCES.txt` & `hashquery-0.2.0/hashquery.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,33 +7,41 @@
 docs/.gitignore
 docs/Makefile
 docs/README.md
 docs/conf.py
 docs/index.md
 docs/requirements.txt
 docs/_fragments/alpha_notice.md
+docs/_fragments/quickstart_smoke_test.md
 docs/_static/.gitkeep
 docs/_static/css/overrides.css
+docs/_static/js/analytics.js
 docs/_static/js/jquery.js
 docs/_static/js/markup.js
 docs/api_reference/0_model.md
 docs/api_reference/1_column_expression.md
 docs/api_reference/2_func.md
 docs/api_reference/3_project.md
 docs/api_reference/4_keypath.md
-docs/concept_explanations/keypaths.md
-docs/concept_explanations/stub.md
-docs/pattern_guides/stub.md
-docs/project_info/development.md
+docs/concept_explanations/0_models.md
+docs/concept_explanations/1_column_expressions.md
+docs/concept_explanations/z_advanced_keypaths.md
+docs/hashboard_intg/0_import.md
+docs/hashboard_intg/dataops.md
+docs/pattern_guides/binning.md
+docs/pattern_guides/events.md
+docs/pattern_guides/joins.md
+docs/pattern_guides/segments.md
+docs/pattern_guides/timeframes.md
+docs/pattern_guides/visualizations.md
 docs/project_info/feedback.md
 docs/project_info/roadmap.md
-docs/setup_tutorial/0_requirements.md
-docs/setup_tutorial/1_install.md
-docs/setup_tutorial/2_authentication.md
-docs/setup_tutorial/3_first_analysis.md
+docs/setup_tutorial/1_quickstart.md
+docs/setup_tutorial/2_first_analysis.md
+docs/setup_tutorial/3_authentication.md
 docs/setup_tutorial/first_analysis_0.py
 docs/setup_tutorial/first_analysis_1.py
 docs/setup_tutorial/first_analysis_2.py
 hashquery.egg-info/PKG-INFO
 hashquery.egg-info/SOURCES.txt
 hashquery.egg-info/dependency_links.txt
 hashquery.egg-info/requires.txt
@@ -63,14 +71,15 @@
 src/model/column_expression/cases.py
 src/model/column_expression/column_expression.py
 src/model/column_expression/column_name.py
 src/model/column_expression/granularity.py
 src/model/column_expression/py_value.py
 src/model/column_expression/sql_function.py
 src/model/column_expression/sql_text.py
+src/model/column_expression/subquery_expression.py
 src/model/source/__init__.py
 src/model/source/aggregate.py
 src/model/source/filter.py
 src/model/source/join_one.py
 src/model/source/limit.py
 src/model/source/match_steps.py
 src/model/source/pick.py
@@ -80,17 +89,18 @@
 src/model/source/table_name.py
 src/model/source/union.py
 src/run/__init__.py
 src/run/post_run_endpoint.py
 src/run/run_results.py
 src/utils/__init__.py
 src/utils/builder.py
-src/utils/date_shift.py
 src/utils/env.py
 src/utils/identifiable.py
 src/utils/resource.py
 src/utils/serializable.py
+src/utils/timeinterval.py
+src/utils/types.py
 src/utils/keypath/__init__.py
 src/utils/keypath/keypath.py
 src/utils/keypath/keypath_ctx.py
 src/utils/keypath/resolve.py
 src/utils/keypath/unwrap.py
```

### Comparing `hashquery-0.1rc3/src/func/_cases.py` & `hashquery-0.2.0/src/func/_cases.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/func/_logical.py` & `hashquery-0.2.0/src/func/_logical.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/func/_sql_functions.py` & `hashquery-0.2.0/src/func/_sql_functions.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/hashboard_api/api.py` & `hashquery-0.2.0/src/hashboard_api/api.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/hashboard_api/credentials.py` & `hashquery-0.2.0/src/hashboard_api/credentials.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/hashboard_api/default_project.py` & `hashquery-0.2.0/src/hashboard_api/default_project.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 base_uri = (
     env_with_fallback("HASHQUERY_API_BASE_URI", "HASHBOARD_CLI_BASE_URI")
     or "https://hashboard.com"
 )
 
 
 class ObjectThatRaisesAnErrorIfYouTouchIt:
-    """
-    This is a fake object that explodes if you touch it.
-    This is used as the `default_project` object if resources failed to load.
-
-    We don't want to raise an error unless the line of code in which you
-    actually try to use the default project. This defers that error.
-    """
+    # This is a fake object that explodes if you touch it.
+    # This is used as the `default_project` object if resources failed to load.
+    #
+    # We don't want to raise an error unless the line of code in which you
+    # actually try to use the default project. This defers that error.
+    __doc__ = ProjectManifest.__doc__
 
     def __getattr__(self, __name: str) -> Any:
         raise AttributeError(
             "Could not authenticate to Hashboard services. "
             + "No credentials were found."
         )
```

### Comparing `hashquery-0.1rc3/src/hashboard_api/project_manifest.py` & `hashquery-0.2.0/src/hashboard_api/project_manifest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from typing import *
 
 from .api import HashboardAPI
-from .project_importer import fetch_all_connections, fetch_all_models
+from .project_importer import (
+    fetch_all_connections,
+    fetch_all_models,
+    fetch_all_project_metrics,
+)
 from ..utils.env import guess_execution_environment
 
 if TYPE_CHECKING:
     from ..model.model import Model
     from ..utils.resource import LinkedResource
 
 
@@ -25,34 +29,43 @@
         models: Collection of project `Model` instances.
         connections: Collection of project connections, as `LinkedResource` instances.
     """
 
     def __init__(self, project_id: str) -> None:
         self.project_id = project_id
         self.models = ProjectModels(project_id)
+        self.metrics = ProjectMetrics(project_id)
         self.connections = ProjectConnections(project_id)
 
         # pre-cache the names of imported resources so they can be
         # auto-completed in notebooks
         try:
             if guess_execution_environment() == "ipython":
                 self.models.get_all()
                 self.connections.get_all()
+                self.metrics.get_all()
         except:
             # this is just a pre-cache attempt which is triggered on `import`
             # so swallow the error and it will resurface naturally if the user
             # attempts something later on where this is needed
             pass
 
+    def _refresh(self) -> "ProjectManifest":
+        self.models._refresh()
+        self.metrics._refresh()
+        self.connections._refresh()
+        return self
+
     def __repr__(self) -> str:
         api = HashboardAPI.get_for_project(self.project_id)
         return "\n".join(
             [
                 f"Project: {self.project_id} on {api.base_uri}",
                 str(self.models),
+                str(self.metrics),
                 str(self.connections),
             ]
         )
 
 
 T = TypeVar("T")
 
@@ -78,14 +91,18 @@
 
     def get_all(self) -> List[T]:
         if self._cache is not None:
             return self._cache
         self._cache = self._get_all_impl()
         return self._cache
 
+    def _refresh(self):
+        self._cache = None
+        return self
+
     def _accessor(self, key: Union[str, int], *, dot_access: bool) -> T:
         if type(key) == int:
             return self.get_all()[key]
         else:
             if found := next(
                 (i for i in self.get_all() if self._item_alias(i) == key),
                 None,
@@ -133,20 +150,36 @@
     def _item_type_name(self) -> str:
         return "Model"
 
     def _item_alias(self, item: "Model") -> str:
         return item._linked_resource.alias or "__unnamed_model__"
 
 
+class ProjectMetrics(ProjectManifestTypedCollection["Model"]):
+    """
+    Collection of all the available Hashboard project metrics.
+    """
+
+    def _get_all_impl(self) -> List["Model"]:
+        return fetch_all_project_metrics(self._project_id)
+
+    @property
+    def _item_type_name(self) -> str:
+        return "Metric"
+
+    def _item_alias(self, item: "Model") -> str:
+        return item._linked_resource.alias or "__unnamed_project_metric__"
+
+
 class ProjectConnections(ProjectManifestTypedCollection["LinkedResource"]):
     """
     Collection of all the Hashboard connections available for the project.
     """
 
-    def _get_all_impl(self) -> List["Model"]:
+    def _get_all_impl(self) -> List["LinkedResource"]:
         return fetch_all_connections(self._project_id)
 
     @property
     def _item_type_name(self) -> str:
         return "Connection"
 
     def _item_alias(self, item: "LinkedResource") -> str:
```

### Comparing `hashquery-0.1rc3/src/model/accessors.py` & `hashquery-0.2.0/src/model/accessors.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/activity_schema.py` & `hashquery-0.2.0/src/model/activity_schema.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/column.py` & `hashquery-0.2.0/src/model/column.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import *
 
+from ..utils.keypath.keypath import _
 from .column_expression import (
     ColumnExpression,
     ColumnNameColumnExpression,
     SqlTextColumnExpression,
     PyValueColumnExpression,
 )
 
@@ -58,18 +59,21 @@
     """
     Constructs a `ColumnExpression`. This function has three variants:
 
     1. `column(str)` will construct a column expression using the column name.
        This name is escaped according to the dialect.
 
     2. `column(sql=str)` will construct an expression which uses the literal
-       SQL, unescaped, as its contents.
+       SQL, unescaped, as its contents. The syntax `{{ some_expr }}` can
+       be used within this SQL string to reference attributes and measure
+       definitions on the given Model. Note that when this is done, the
+       referenced expressions can also become unescaped.
 
     3. `column(value=Any)` will construct an expression which represents
        the provided Python value. For example, `None` is translated to `NULL`.
     """
     if name:
         return ColumnNameColumnExpression(name)
     elif sql:
-        return SqlTextColumnExpression(sql)
+        return SqlTextColumnExpression(sql).bind_references_to_model(_)
     else:
         return PyValueColumnExpression(value)
```

### Comparing `hashquery-0.1rc3/src/model/column_expression/binary_op.py` & `hashquery-0.2.0/src/model/column_expression/binary_op.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 
 class BinaryOpColumnExpression(ColumnExpression):
     def __init__(
         self,
         left: ColumnExpression,
         right: ColumnExpression,
         op: str,
+        options: Optional[Dict[str, Union[str, bool]]] = None,
     ) -> None:
         super().__init__()
         self.left = left
         self.right = right
         self.op = op
+        self.options = options or {}
 
     def default_identifier(self) -> Optional[str]:
         return None
 
     @builder_method
     def disambiguated(self, namespace) -> "BinaryOpColumnExpression":
         self.left.disambiguated(namespace)
@@ -33,17 +35,18 @@
 
     def to_wire_format(self) -> Any:
         return {
             **super().to_wire_format(),
             "left": self.left.to_wire_format(),
             "right": self.right.to_wire_format(),
             "op": self.op,
+            "options": self.options,
         }
 
     @classmethod
     def from_wire_format(cls, wire: dict) -> "BinaryOpColumnExpression":
         assert wire["subType"] == cls.__TYPE_KEY__
         left = ColumnExpression.from_wire_format(wire["left"])
         right = ColumnExpression.from_wire_format(wire["right"])
         return BinaryOpColumnExpression(
-            left, right, wire["op"]
+            left, right, wire["op"], wire["options"]
         )._from_wire_format_shared(wire)
```

### Comparing `hashquery-0.1rc3/src/model/column_expression/cases.py` & `hashquery-0.2.0/src/model/column_expression/cases.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/column_expression/column_name.py` & `hashquery-0.2.0/src/model/column_expression/column_name.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/column_expression/granularity.py` & `hashquery-0.2.0/src/model/column_expression/granularity.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/column_expression/py_value.py` & `hashquery-0.2.0/src/model/column_expression/py_value.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/column_expression/sql_function.py` & `hashquery-0.2.0/src/model/column_expression/sql_function.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/column_expression/sql_text.py` & `hashquery-0.2.0/src/model/column_expression/subquery_expression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from typing import *
 
 from .column_expression import ColumnExpression
 from ...utils.builder import builder_method
 
+if TYPE_CHECKING:
+    from ..model import Model
 
-class SqlTextColumnExpression(ColumnExpression):
-    def __init__(self, sql: str) -> None:
+
+class SubqueryColumnExpression(ColumnExpression):
+    def __init__(self, model: "Model") -> None:
         super().__init__()
-        self.sql = sql
+        self.model = model
 
     def default_identifier(self) -> str:
-        if self.sql.isidentifier():
-            return self.sql
-        return None
+        return list(self.model._attributes.keys())[0]
 
     @builder_method
-    def disambiguated(self, namespace) -> "SqlTextColumnExpression":
-        # TODO: users need some ability to qualify their own textual
-        # references in raw SQL; which right now they cannot
+    def disambiguated(self, namespace) -> "ColumnExpression":
+        # a subquery cannot be scoped/qualified
         pass
 
     def __repr__(self) -> str:
-        return f'sql("{self.sql}")'
+        return f"<subquery>"
 
     # --- Serialization ---
 
-    __TYPE_KEY__ = "sqlText"
+    __TYPE_KEY__ = "subquery"
 
     def to_wire_format(self) -> dict:
-        return {
-            **super().to_wire_format(),
-            "sql": self.sql,
-        }
+        return {**super().to_wire_format(), "model": self.model.to_wire_format()}
 
     @classmethod
-    def from_wire_format(cls, wire: dict) -> "SqlTextColumnExpression":
+    def from_wire_format(cls, wire: dict) -> "ColumnExpression":
+        from ..model import Model
+
         assert wire["subType"] == cls.__TYPE_KEY__
-        result = SqlTextColumnExpression(wire["sql"])
+        model = Model.from_wire_format(wire["model"])
+        result = SubqueryColumnExpression(model)
         result._from_wire_format_shared(wire)
         return result
```

### Comparing `hashquery-0.1rc3/src/model/model.py` & `hashquery-0.2.0/src/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,66 +58,88 @@
         # and its relation to an original Hashboard resource
         self._linked_resource: Optional[LinkedResource] = None
 
     # --- Public accessors ---
 
     def _access_identifiable_map(
         self,
-        map_name: str,
+        map_names: Union[str, List[str]],
         identifier: str,
         *,
-        keypath_ctx: KeyPathCtx = None,
+        keypath_ctx: Union[KeyPathCtx, str] = None,
+        syntax: Union[Literal["accessor"], Literal["sql_ref"]] = "accessor",
     ):
         # internal accessor for getting attributes, measures, and relations
-        map: IdentifiableMap = getattr(self, map_name)
-        if result := map.get(identifier):
-            return result
+        map_names = [map_names] if isinstance(map_names, str) else map_names
+        maps: List[IdentifiableMap] = [
+            getattr(self, map_name) for map_name in map_names
+        ]
+        for map in maps:
+            if result := map.get(identifier):
+                return result
+
         # accessing an attr/measure/namespace which doesn't exist is a pretty
         # common pitfall, so put in the extra work to make a good error message
-        map_debug_name = map_name[1:-1]
-        if map_debug_name == "namespace":
-            map_debug_name = "relation"
-        error = [f"No {map_debug_name} named `{identifier}` was found in the model."]
+        map_debug_names = [
+            map_name[1:-1].replace("namespace", "relation") for map_name in map_names
+        ]
+        error = [
+            f"No {' or '.join(map_debug_names)} named `{identifier}` was found in the model."
+        ]
+        did_you_mean = (
+            lambda accessor, id: f"Did you mean `{accessor}.{id}`?"
+            if syntax == "accessor"
+            else "Did you mean `{{" + id + "}}`?"
+        )
         if attr_result := self._attributes.get(identifier):
             error.append(f"An attribute ({attr_result}) was found instead. ")
             error.append(
                 "This was potentially caused because measures are converted "
                 + "to attributes after an aggregation. "
             )
-            error.append(f"Did you mean to use `attr.{identifier}`?")
+            error.append(did_you_mean("attr", identifier))
         if measure_result := self._measures.get(identifier):
             error.append(f"A measure ({measure_result}) was found instead. ")
-            error.append(f"Did you mean to use `msr.{identifier}`?")
+            error.append(did_you_mean("msr", identifier))
         if self._namespaces.get(identifier):
             error.append(f"A model relation was found instead. ")
-            error.append(f"Did you mean to use `rel.{identifier}`?")
-        if map_name == "_namespaces":
+            error.append(did_you_mean("rel", identifier))
+        if "_namespaces" in map_names:
             # look for if the next access is against an attribute we have,
             # in which case this mistake was that they didn't realize the
             # relation had been flattened.
-            next_access = keypath_ctx.remaining_keypath._key_path_components[0]
+            next_access = (
+                keypath_ctx.remaining_keypath._key_path_components[0]
+                if isinstance(keypath_ctx, KeyPathCtx)
+                else keypath_ctx
+            )
             next_access_name: str = None
-            if type(next_access) is KeyPathComponentProperty:
+            if type(next_access) is str:
+                next_access_name = next_access
+            elif type(next_access) is KeyPathComponentProperty:
                 next_access_name = next_access.name
             next_access_attr = (
                 self._attributes.get(next_access_name) if next_access_name else None
             )
             if next_access_attr:
                 error.append(f"The target attribute `{next_access_name}` was found. ")
                 error.append(
                     "A transformation may have moved the attribute "
                     + f"from the {identifier} relation to being directly available. "
                 )
-                error.append(f"Did you mean `attr.{next_access_name}`?")
+                error.append(did_you_mean("attr", next_access_name))
         if len(error) == 1:
-            error.append(
-                f"Available {map_debug_name}s: {', '.join(map.keys())}"
-                if map
-                else f"No {map_debug_name}s are defined for this model."
-            )
+            for idx, map_name in enumerate(map_names):
+                map: IdentifiableMap = getattr(self, map_name)
+                debug_name = map_debug_names[idx]
+                error.append(
+                    f"Available {debug_name}s: {', '.join(map.keys())}"
+                    if map
+                    else f"No {debug_name}s are defined for this model."
+                )
         raise AttributeError("\n".join(error))
 
     def __repr__(self):
         result = ["Model:"]
         show_ids = lambda map: ", ".join(map.keys()) if map else "<none>"
         result.append(f"  Attributes: {show_ids(self._attributes)}")
         result.append(f"  Measures: {show_ids(self._measures)}")
@@ -246,38 +268,33 @@
         *,
         foreign_key: Optional[Union[ColumnExpression, KeyPath]] = None,
         condition: Optional[ColumnExpression] = None,
         named: Optional[Union[str, KeyPath]] = None,
         drop_unmatched: bool = False,
     ) -> "Model":
         """
-        Forms a new Model with a new property which can be used to reference
+        Returns a new Model with a new property which can be used to reference
         the properties of the `joined` Model. Records are aligned using `foreign_key`
         and/or `condition`. Attributes on joined relations can be referenced with
         `rel.<name>.<attr_name>`.
 
         Similar to `with_measures` and `with_attributes`, `with_join_one` has no
         performance cost on its own. No JOIN statement is added to queries
         unless the relation is actually referenced.
 
-        This never changes the record count of the data by exploding rows.
-        If multiple records match, only the first matching record is joined.
-        If you want to explode records, use `Model.cross_join` instead.
-
         If no records match, `NULL` values are filled in for the missing columns,
         unless `drop_unmatched=True` is passed.
         """
         # -- gather all the parameters up, resolve and validate --
         if foreign_key is None and condition is None:
             raise ValueError(
                 "`.with_join_one` must specify a join condition using "
                 + "`foreign_key=<foreign_key>` and/or `condition=<column_expression>`"
             )
-        if type(joined) == KeyPath:
-            joined = resolve_keypath(self, joined)
+        joined = resolve_keypath(self, joined)
         relation_name = unwrap_keypath_to_name(named)
         if not relation_name:
             if default_identifier := joined._source._default_identifier():
                 relation_name = default_identifier
         if not relation_name:
             raise ValueError(
                 "Join was not provided an identifier and a default could not be inferred. "
@@ -286,19 +303,15 @@
 
         # -- form the namespace we're joining to --
         relation = ModelNamespace(identifier=relation_name, nested_model=joined)
 
         # -- determine the column expression to join with --
         join_predicate = None
         if foreign_key is not None:
-            foreign_key: ColumnExpression = (
-                resolve_keypath(self, foreign_key)
-                if isinstance(foreign_key, KeyPath)
-                else foreign_key
-            )
+            foreign_key: ColumnExpression = resolve_keypath(self, foreign_key)
             join_predicate = foreign_key == joined._primary_key.disambiguated(
                 relation_name
             )
         # you can reference the relation in the `condition=` but not in
         # `foreign_key=` so add it to `_namespaces` here
         self._namespaces.add(relation)
         if condition is not None:
@@ -491,19 +504,21 @@
             6           other_event             2024-01-01
             '''
 
             events.funnel("ad_impression", "visit", "purchase")
             '''
             step                 count
             ------------------------------
+            count                7
             ad_impression        5
             visit                5
             purchase             2
             '''
-            # `ad_impression` is 5 because 5 unique users saw an ad:
+            # `count` is 7 because there are 7 unique users.
+            # `ad_impression` is 5 because of those 7 unique users, 5 of them saw an ad:
             #        This is users 0, 1, 2, 3, and 4.
             #        Users 5 and 6 did not see ads, so they are not included.
             # `visit` is 4 because of the 5 users who saw an ad, 4 of them went on to visit:
             #        This is users 0, 1, 2, and 3.
             #        User 5 visited, but not after seeing an ad, so they are not included in the funnel.
             # `purchase` is 2 because of the 4 users who saw an ad, then visited, 2 of them went on to purchase:
             #        This is users 0 and 1. User 1 made two purchases but is only counted once.
@@ -527,49 +542,48 @@
 
     # --- Record Management ---
 
     @builder_method
     @resolve_keypath_args_from(_.self)
     def pick(self, *columns: ColumnExpression) -> "Model":
         """
-        Forms a new Model with only the included attributes included.
+        Returns a new Model with only the included attributes.
         """
         self._source = PickSource(self._source, columns)
         self._attributes = IdentifiableMap(column(c.identifier) for c in columns)
         self._namespaces = IdentifiableMap()
         # we might want to preserve measures if we can inspect them
         # and confirm they only rely on selected columns (?)
         self._measures = IdentifiableMap()
 
     @builder_method
     @resolve_keypath_args_from(_.self)
     def filter(self, condition: ColumnExpression) -> "Model":
         """
-        Forms a new Model with records filtered to only those which
+        Returns a new Model with records filtered to only those which
         match the given condition.
         """
         self._source = FilterSource(self._source, condition)
 
     @builder_method
     @resolve_keypath_args_from(_.self)
     def sort(
         self, sort: ColumnExpression, dir: Literal["asc", "desc"] = "asc"
     ) -> "Model":
         """
-        Forms a new Model with records ordered by the provided column.
-
+        Returns a new Model with records ordered by the provided column.
         Sort direction `dir` can be either "asc" or "desc" (defaults to "asc").
         """
         self._source = SortSource(self._source, sort, dir)
 
     @builder_method
     @resolve_keypath_args_from(_.self)
     def limit(self, count: int, *, offset: Optional[int] = 0) -> "Model":
         """
-        Forms a new Model with only the first N records.
+        Returns a new Model with only the first N records.
         """
         self._source = LimitSource(self._source, count, offset=offset)
 
     @builder_method
     @resolve_keypath_args_from(_.self)
     def union_all(self, other: "Model") -> "Model":
         """
@@ -708,15 +722,15 @@
 
     # --- Custom Meta ---
 
     @builder_method
     @resolve_keypath_args_from(_.self)
     def with_custom_meta(self, name: str, value: Any) -> "Model":
         """
-        Forms a new Model with the custom metadata attached. Hashquery will
+        Returns a new Model with the custom metadata attached. Hashquery will
         never read or write to this key, making it a good spot to put any
         custom configuration or encode semantic information about the Model
         which you want to use.
         """
         self._custom_meta[name] = value
 
     def get_custom_meta(self, name: str):
```

### Comparing `hashquery-0.1rc3/src/model/namespace.py` & `hashquery-0.2.0/src/model/namespace.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/source/aggregate.py` & `hashquery-0.2.0/src/model/source/aggregate.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/source/filter.py` & `hashquery-0.2.0/src/model/source/filter.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/source/join_one.py` & `hashquery-0.2.0/src/model/source/join_one.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/source/limit.py` & `hashquery-0.2.0/src/model/source/limit.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/source/match_steps.py` & `hashquery-0.2.0/src/model/source/match_steps.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/source/pick.py` & `hashquery-0.2.0/src/model/source/pick.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/source/sort.py` & `hashquery-0.2.0/src/model/source/sort.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/source/source.py` & `hashquery-0.2.0/src/model/source/source.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/source/sql_text.py` & `hashquery-0.2.0/src/model/source/sql_text.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/source/table_name.py` & `hashquery-0.2.0/src/model/source/table_name.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/model/source/union.py` & `hashquery-0.2.0/src/model/source/union.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/run/post_run_endpoint.py` & `hashquery-0.2.0/src/run/post_run_endpoint.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/run/run_results.py` & `hashquery-0.2.0/src/run/run_results.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,17 +31,15 @@
         return compile_result["sqlQuery"]
 
     @property
     def df(self) -> pd.DataFrame:
         """
         The result records as a pandas DataFrame.
         """
-        self._print_compile_warnings_if_needed()
-        self._print_execution_stats_if_needed()
-        data_result = self._get_ok_result("data")
+        data_result = self._validated_result("data")
         if "arrow" in data_result:
             arrow_ipc = base64.b64decode(data_result["arrow"])
             with pa.ipc.open_file(arrow_ipc) as reader:
                 table = reader.read_all()
                 return table.to_pandas()
 
         elif "csv" in data_result:
@@ -68,16 +66,15 @@
         if key == "compile":
             return compile_result
         if key == "data":
             self._print_execution_stats_if_needed()
             return self._get_ok_result("data")
 
     def _get_ok_result(self, key: Union[Literal["compile"], Literal["data"]]):
-        # raise an error at this point if the key is not `ok`
-        key_obj = self._result_json.get(key, {})
+        key_obj: dict = self._result_json.get(key, {})
         if not key_obj.get("ok", False):
             raise RunResultsError(
                 phase=key,
                 msg="\n".join(
                     key_obj.get(
                         "errors",
                         [
```

### Comparing `hashquery-0.1rc3/src/utils/builder.py` & `hashquery-0.2.0/src/utils/builder.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/utils/env.py` & `hashquery-0.2.0/src/utils/env.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/utils/identifiable.py` & `hashquery-0.2.0/src/utils/identifiable.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/utils/keypath/__init__.py` & `hashquery-0.2.0/src/utils/keypath/__init__.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/utils/keypath/keypath.py` & `hashquery-0.2.0/src/utils/keypath/keypath.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/utils/keypath/resolve.py` & `hashquery-0.2.0/src/utils/keypath/resolve.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,60 @@
 import inspect
 from functools import wraps
-from typing import Any, Callable
+from typing import Any
 
 from .keypath import (
     BoundKeyPath,
     KeyPath,
     KeyPathComponentCall,
     KeyPathComponentProperty,
     KeyPathComponentSubscript,
 )
 from .keypath_ctx import KeyPathCtx
 
 
-def get_keypath_resolver(keypath: KeyPath) -> Callable[[Any], Any]:
-    """
-    Given a keypath, returns it as a callable accessor function.
-    """
-
-    def resolver(root: Any) -> Any:
-        current = root
-        if type(keypath) == BoundKeyPath:
-            current = keypath._bound_root
-
-        for component_idx, component in enumerate(keypath._key_path_components):
-            if type(component) is KeyPathComponentProperty:
-                current = getattr(current, component.name)
-            elif type(component) is KeyPathComponentSubscript:
-                current = current[component.key]
-            elif type(component) is KeyPathComponentCall:
-                args = resolve_all_nested_keypaths(root, component.args)
-                kwargs = resolve_all_nested_keypaths(root, component.kwargs)
-                if component.include_keypath_ctx:
-                    kwargs["keypath_ctx"] = KeyPathCtx(
-                        root=root,
-                        current=current,
-                        full_keypath=keypath,
-                        current_keypath_component=component,
-                        remaining_keypath=KeyPath(
-                            keypath._key_path_components[component_idx + 1 :]
-                        ),
-                    )
-                current = current(*args, **kwargs)
-            else:
-                raise AssertionError(f"Invalid keypath component: {type(component)}")
-        return current
-
-    return resolver
-
-
 def resolve_keypath(root: Any, keypath: KeyPath) -> Any:
     """
     Given a root and a KeyPath, resolves the keypath for that root
-    and returns the final result (or fails with `AttributeError` if the
-    keypath is invalid for that root).
+    and returns the final result.
+
+    If the given `keypath` argument is not a KeyPath, this will just return
+    it as is, since it already represents a resolved value.
     """
-    return get_keypath_resolver(keypath)(root)
+    if not isinstance(keypath, KeyPath):
+        return keypath
+
+    current = root
+    if type(keypath) == BoundKeyPath:
+        current = keypath._bound_root
+
+    for component_idx, component in enumerate(keypath._key_path_components):
+        if type(component) is KeyPathComponentProperty:
+            current = getattr(current, component.name)
+        elif type(component) is KeyPathComponentSubscript:
+            current = current[component.key]
+        elif type(component) is KeyPathComponentCall:
+            args = resolve_all_nested_keypaths(root, component.args)
+            kwargs = resolve_all_nested_keypaths(root, component.kwargs)
+            if component.include_keypath_ctx:
+                kwargs["keypath_ctx"] = KeyPathCtx(
+                    root=root,
+                    current=current,
+                    full_keypath=keypath,
+                    current_keypath_component=component,
+                    remaining_keypath=KeyPath(
+                        keypath._key_path_components[component_idx + 1 :]
+                    ),
+                )
+            current = current(*args, **kwargs)
+        else:
+            raise AssertionError(f"Invalid keypath component: {type(component)}")
+
+    # a KeyPath may result in another KeyPath, which we need to further resolve
+    return resolve_keypath(root, current)
 
 
 def resolve_all_nested_keypaths(root: Any, values) -> Any:
     """
     Given a data structure that may have KeyPaths in it, resolves all of them
     recursively with the provided root. This is helpful for handling collections
     of values that may or may not be KeyPaths, and turning them all into real
@@ -70,15 +66,18 @@
             for key, nested in values.items()
         }
     elif type(values) is list:
         return [resolve_all_nested_keypaths(root, nested) for nested in values]
     elif type(values) is tuple:
         return (resolve_all_nested_keypaths(root, nested) for nested in values)
     elif isinstance(values, KeyPath):
-        return resolve_keypath(root, values)
+        # a KeyPath may result in a structure containing more KeyPaths,
+        # which we need to further resolve
+        next = resolve_keypath(root, values)
+        return resolve_all_nested_keypaths(root, next)
     else:
         return values
 
 
 def resolve_keypath_args_from(root_keypath: KeyPath):
     """
     Decorates a function to convert its arguments to KeyPaths, using
```

### Comparing `hashquery-0.1rc3/src/utils/keypath/unwrap.py` & `hashquery-0.2.0/src/utils/keypath/unwrap.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/utils/resource.py` & `hashquery-0.2.0/src/utils/resource.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.1rc3/src/utils/serializable.py` & `hashquery-0.2.0/src/utils/serializable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from abc import ABC
 from datetime import date, datetime, timedelta
 from functools import wraps
 from typing import Type
 
 from typing_extensions import Self
 
-from .date_shift import _DateShift
+from .timeinterval import timeinterval
 
 HASHQUERY_WIRE_VERSION_KEY = "_version"
 # This is a version number for the wire format of Hashquery.
 # Increase it if you ever make a backwards incompatible change
 # to a `to_wire_format`/`from_wire_format` pair, or if you change
 # the JSON payload for `RunResults`.
-HASHQUERY_WIRE_VERSION = 4
+HASHQUERY_WIRE_VERSION = 6
 
 
 class Serializable(ABC):
     def to_wire_format(cls) -> dict:
         ...
 
     @classmethod
@@ -27,19 +27,19 @@
     def _primitive_to_wire_format(cls, value):
         if isinstance(value, datetime):
             return {"$typeKey": "py.datetime", "iso": value.isoformat()}
         elif isinstance(value, date):
             return {"$typeKey": "py.date", "iso": value.isoformat()}
         elif isinstance(value, timedelta):
             return {"$typeKey": "py.timedelta", "seconds": int(value.total_seconds())}
-        elif isinstance(value, _DateShift):
+        elif isinstance(value, timeinterval):
             return {
-                "$typeKey": "py.shift",
-                "years": value.years,
-                "months": value.months,
+                "$typeKey": "py.timeinterval",
+                "unit": value.unit,
+                "num": value.num,
             }
         # directly serializable to JSON without type information
         return value
 
     @classmethod
     def _primitive_from_wire_format(cls, wire):
         type_key = wire.get("$typeKey") if type(wire) == dict else None
@@ -47,23 +47,22 @@
             return wire
         elif type_key == "py.datetime":
             return datetime.fromisoformat(wire["iso"])
         elif type_key == "py.date":
             return date.fromisoformat(wire["iso"])
         elif type_key == "py.timedelta":
             return timedelta(seconds=wire["seconds"])
-        elif type_key == "py.shift":
-            return _DateShift(
-                years=wire["years"],
-                months=wire["months"],
+        elif type_key == "py.timeinterval":
+            return timeinterval(
+                unit=wire["unit"],
+                num=wire["num"],
             )
         else:
             raise ValueError(
-                "Cannot deserialize value. `$typeKey` is present but an unrecognized type. "
-                + wire
+                f"Cannot deserialize value. `$typeKey` is present but an unrecognized type. {wire}"
             )
 
     def __init_subclass__(cls) -> None:
         """
         When we subclass, update their `to_wire_format`/`from_wire_format`
         methods to populate and validate the wire version keys.
         """
```


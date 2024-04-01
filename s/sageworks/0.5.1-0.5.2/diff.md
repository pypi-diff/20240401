# Comparing `tmp/sageworks-0.5.1.tar.gz` & `tmp/sageworks-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.5.1.tar", last modified: Mon Apr  1 15:28:23 2024, max compression
+gzip compressed data, was "sageworks-0.5.2.tar", last modified: Mon Apr  1 16:27:58 2024, max compression
```

## Comparing `sageworks-0.5.1.tar` & `sageworks-0.5.2.tar`

### file list

```diff
@@ -1,505 +1,505 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.171829 sageworks-0.5.1/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.118468 sageworks-0.5.1/.github/
--rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.5.1/.github/dependabot.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.118694 sageworks-0.5.1/.github/workflows/
--rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.5.1/.github/workflows/deploy-docs.yml
--rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.5.1/.github/workflows/python-lint.yml
--rw-r--r--   0 briford    (501) staff       (20)     2008 2023-12-24 17:18:24.000000 sageworks-0.5.1/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      444 2024-03-28 17:23:43.000000 sageworks-0.5.1/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.5.1/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.5.1/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.5.1/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     4118 2024-04-01 15:28:23.171730 sageworks-0.5.1/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     2695 2024-03-28 17:23:43.000000 sageworks-0.5.1/README.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.5.1/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.109583 sageworks-0.5.1/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.119743 sageworks-0.5.1/applications/aws_dashboard/
--rw-r--r--   0 briford    (501) staff       (20)     1071 2024-04-01 13:10:05.000000 sageworks-0.5.1/applications/aws_dashboard/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/Dockerfile_plugins
--rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.5.1/applications/aws_dashboard/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1296 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.120176 sageworks-0.5.1/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)    14995 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.5.1/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.5.1/applications/aws_dashboard/assets/trash.png
--rwxr-xr-x   0 briford    (501) staff       (20)      644 2024-03-31 16:51:01.000000 sageworks-0.5.1/applications/aws_dashboard/dashboard
--rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.5.1/applications/aws_dashboard/nginx.conf
--rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/open_source_config.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.109511 sageworks-0.5.1/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.120642 sageworks-0.5.1/applications/aws_dashboard/pages/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)    11696 2024-03-30 22:43:51.000000 sageworks-0.5.1/applications/aws_dashboard/pages/data_sources/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/pages/data_sources/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/pages/data_sources/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.121033 sageworks-0.5.1/applications/aws_dashboard/pages/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)     3975 2024-03-30 22:43:51.000000 sageworks-0.5.1/applications/aws_dashboard/pages/endpoints/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2565 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/pages/endpoints/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2465 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/pages/endpoints/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.121404 sageworks-0.5.1/applications/aws_dashboard/pages/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)    11610 2024-03-30 22:43:51.000000 sageworks-0.5.1/applications/aws_dashboard/pages/feature_sets/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/pages/feature_sets/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/pages/feature_sets/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.121808 sageworks-0.5.1/applications/aws_dashboard/pages/main/
--rw-r--r--   0 briford    (501) staff       (20)     4899 2024-03-30 22:43:51.000000 sageworks-0.5.1/applications/aws_dashboard/pages/main/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2899 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/pages/main/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/pages/main/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.122197 sageworks-0.5.1/applications/aws_dashboard/pages/models/
--rw-r--r--   0 briford    (501) staff       (20)     3672 2024-03-30 22:43:51.000000 sageworks-0.5.1/applications/aws_dashboard/pages/models/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2020 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/pages/models/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2341 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/aws_dashboard/pages/models/page.py
--rw-r--r--   0 briford    (501) staff       (20)      394 2024-04-01 13:00:51.000000 sageworks-0.5.1/applications/aws_dashboard/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.5.1/applications/aws_dashboard/supervisord.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.109637 sageworks-0.5.1/applications/experiments/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.122941 sageworks-0.5.1/applications/experiments/compound_explorer/
--rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.5.1/applications/experiments/compound_explorer/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.5.1/applications/experiments/compound_explorer/README.md
--rw-r--r--   0 briford    (501) staff       (20)     3096 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/experiments/compound_explorer/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.123176 sageworks-0.5.1/applications/experiments/compound_explorer/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.5.1/applications/experiments/compound_explorer/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.5.1/applications/experiments/compound_explorer/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     7676 2024-03-30 22:43:51.000000 sageworks-0.5.1/applications/experiments/compound_explorer/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.5.1/applications/experiments/compound_explorer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.5.1/applications/experiments/compound_explorer/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.123529 sageworks-0.5.1/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.5.1/aws_setup/aws_account_check.py
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.5.1/aws_setup/aws_identity_check.py
--rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.5.1/aws_setup/build_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.123643 sageworks-0.5.1/aws_setup/event_bridge/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/event_bridge/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.124117 sageworks-0.5.1/aws_setup/event_bridge/dynamic_docker/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/event_bridge/dynamic_docker/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/event_bridge/dynamic_docker/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/event_bridge/dynamic_docker/cdk.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.124231 sageworks-0.5.1/aws_setup/event_bridge/dynamic_docker/lambda/
--rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.5.1/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
--rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.5.1/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.125126 sageworks-0.5.1/aws_setup/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_core/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_core/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.5.1/aws_setup/sageworks_core/app.py
--rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_core/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_core/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.5.1/aws_setup/sageworks_core/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.125362 sageworks-0.5.1/aws_setup/sageworks_core/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/aws_setup/sageworks_core/sageworks_core/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.5.1/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_core/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.125528 sageworks-0.5.1/aws_setup/sageworks_core/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_core/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.125734 sageworks-0.5.1/aws_setup/sageworks_core/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_core/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.126703 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.127055 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-01 13:22:58.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.127216 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.127423 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.128062 sageworks-0.5.1/aws_setup/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_lite/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_lite/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_lite/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_lite/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_lite/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.128296 sageworks-0.5.1/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     6849 2024-04-01 15:22:44.000000 sageworks-0.5.1/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.128921 sageworks-0.5.1/data/
--rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.5.1/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.5.1/data/test_data.csv
--rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.5.1/data/test_data.json
--rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.5.1/data/wine_dataset.csv
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.129209 sageworks-0.5.1/docs/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.129504 sageworks-0.5.1/docs/admin/
--rw-r--r--   0 briford    (501) staff       (20)     1825 2024-03-28 17:23:43.000000 sageworks-0.5.1/docs/admin/docker_push.md
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/admin/pypi_release.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.130493 sageworks-0.5.1/docs/api_classes/
--rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.5.1/docs/api_classes/data_source.md
--rw-r--r--   0 briford    (501) staff       (20)     5199 2024-03-28 17:23:43.000000 sageworks-0.5.1/docs/api_classes/endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.5.1/docs/api_classes/feature_set.md
--rw-r--r--   0 briford    (501) staff       (20)     5350 2024-03-30 23:05:32.000000 sageworks-0.5.1/docs/api_classes/meta.md
--rw-r--r--   0 briford    (501) staff       (20)     4356 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/api_classes/model.md
--rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/api_classes/monitor.md
--rw-r--r--   0 briford    (501) staff       (20)     3549 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/api_classes/overview.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.131219 sageworks-0.5.1/docs/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.5.1/docs/aws_setup/aws_access_management.md
--rw-r--r--   0 briford    (501) staff       (20)     7836 2024-01-23 15:36:53.000000 sageworks-0.5.1/docs/aws_setup/aws_tips_and_tricks.md
--rw-r--r--   0 briford    (501) staff       (20)     4229 2024-03-28 17:23:43.000000 sageworks-0.5.1/docs/aws_setup/core_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.5.1/docs/aws_setup/dashboard_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.5.1/docs/aws_setup/full_pipeline.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.131341 sageworks-0.5.1/docs/concepts/
--rw-r--r--   0 briford    (501) staff       (20)      907 2024-01-23 15:36:53.000000 sageworks-0.5.1/docs/concepts/model_monitoring.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.131477 sageworks-0.5.1/docs/core_classes/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.132482 sageworks-0.5.1/docs/core_classes/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.5.1/docs/core_classes/artifacts/artifact.md
--rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/core_classes/artifacts/athena_source.md
--rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.5.1/docs/core_classes/artifacts/data_source_abstract.md
--rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/core_classes/artifacts/endpoint_core.md
--rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/core_classes/artifacts/feature_set_core.md
--rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/core_classes/artifacts/model_core.md
--rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/core_classes/artifacts/monitor_core.md
--rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/core_classes/artifacts/overview.md
--rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/core_classes/overview.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.133442 sageworks-0.5.1/docs/core_classes/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/core_classes/transforms/data_loaders_heavy.md
--rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/core_classes/transforms/data_loaders_light.md
--rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.5.1/docs/core_classes/transforms/data_to_features.md
--rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/core_classes/transforms/features_to_model.md
--rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/core_classes/transforms/model_to_endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/core_classes/transforms/overview.md
--rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.5.1/docs/core_classes/transforms/pandas_transforms.md
--rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.5.1/docs/core_classes/transforms/transform.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.133556 sageworks-0.5.1/docs/glue/
--rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.5.1/docs/glue/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.135930 sageworks-0.5.1/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.5.1/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.5.1/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.5.1/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.5.1/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.5.1/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.5.1/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.5.1/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.5.1/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.5.1/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.5.1/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.5.1/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)     3417 2024-03-28 17:23:43.000000 sageworks-0.5.1/docs/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.136630 sageworks-0.5.1/docs/misc/
--rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.5.1/docs/misc/faq.md
--rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/misc/general_info.md
--rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/misc/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.5.1/docs/misc/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.136886 sageworks-0.5.1/docs/plugins/
--rw-r--r--   0 briford    (501) staff       (20)     3100 2024-04-01 00:11:00.000000 sageworks-0.5.1/docs/plugins/index.md
--rw-r--r--   0 briford    (501) staff       (20)      750 2024-03-31 15:49:43.000000 sageworks-0.5.1/docs/plugins/plugin_api_changes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.137022 sageworks-0.5.1/docs/repl/
--rw-r--r--   0 briford    (501) staff       (20)     2081 2024-03-28 17:23:43.000000 sageworks-0.5.1/docs/repl/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.137276 sageworks-0.5.1/docs/research/
--rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.5.1/docs/research/eda.md
--rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.5.1/docs/research/htg.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.140005 sageworks-0.5.1/examples/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.140128 sageworks-0.5.1/examples/ag-grid/
--rw-r--r--   0 briford    (501) staff       (20)      496 2024-03-31 22:06:56.000000 sageworks-0.5.1/examples/ag-grid/hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.5.1/examples/datasource_from_df.py
--rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.5.1/examples/datasource_from_s3.py
--rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.5.1/examples/datasource_query.py
--rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.5.1/examples/datasource_stats.py
--rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.5.1/examples/datasource_to_featureset.py
--rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.5.1/examples/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)      834 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.5.1/examples/endpoint_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.5.1/examples/featureset_eda.py
--rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/featureset_query.py
--rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.5.1/examples/featureset_to_model.py
--rw-r--r--   0 briford    (501) staff       (20)     1534 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/full_ml_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.5.1/examples/glue_hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.5.1/examples/glue_hello_world_with_log.py
--rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.5.1/examples/glue_load_s3_bucket.py
--rw-r--r--   0 briford    (501) staff       (20)      363 2024-03-30 22:43:51.000000 sageworks-0.5.1/examples/meta_list_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      328 2024-03-30 22:43:51.000000 sageworks-0.5.1/examples/meta_list_models.py
--rw-r--r--   0 briford    (501) staff       (20)      659 2024-03-30 22:43:51.000000 sageworks-0.5.1/examples/meta_model_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      548 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/model_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.5.1/examples/model_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.5.1/examples/monitor_setup.py
--rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.5.1/examples/monitor_usage.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.112254 sageworks-0.5.1/examples/plugins/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.140251 sageworks-0.5.1/examples/plugins/pages/
--rw-r--r--   0 briford    (501) staff       (20)     2474 2024-03-31 19:33:46.000000 sageworks-0.5.1/examples/plugins/pages/my_plugin_page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.140383 sageworks-0.5.1/examples/plugins/views/
--rw-r--r--   0 briford    (501) staff       (20)     1264 2024-03-31 19:19:35.000000 sageworks-0.5.1/examples/plugins/views/my_view_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.140646 sageworks-0.5.1/examples/plugins/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     1666 2024-03-31 18:52:26.000000 sageworks-0.5.1/examples/plugins/web_components/endpoint_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     1942 2024-03-31 22:06:56.000000 sageworks-0.5.1/examples/plugins/web_components/model_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.141029 sageworks-0.5.1/examples/sagemaker_pipelines/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/sagemaker_pipelines/all_steps.py
--rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/sagemaker_pipelines/hello.py
--rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/sagemaker_pipelines/ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.112482 sageworks-0.5.1/examples/sagemaker_pipelines/storage/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.141694 sageworks-0.5.1/examples/sagemaker_pipelines/storage/full_pipeline_experiment/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.142352 sageworks-0.5.1/examples/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.5.1/examples/storage/data_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.5.1/examples/storage/data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1371 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/storage/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.5.1/examples/storage/hello_world_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)     4378 2024-03-31 17:04:46.000000 sageworks-0.5.1/examples/storage/plugin_page_example.py
--rw-r--r--   0 briford    (501) staff       (20)     2750 2024-03-31 15:47:34.000000 sageworks-0.5.1/mkdocs.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.142895 sageworks-0.5.1/notebooks/
--rw-r--r--   0 briford    (501) staff       (20)   185443 2024-03-28 17:23:43.000000 sageworks-0.5.1/notebooks/ML_Pipeline_with_SageWorks.ipynb
--rw-r--r--   0 briford    (501) staff       (20)    36405 2024-03-28 17:23:43.000000 sageworks-0.5.1/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
--rw-r--r--   0 briford    (501) staff       (20)   511134 2024-03-28 17:23:43.000000 sageworks-0.5.1/notebooks/Outliers_in_SageWorks.ipynb
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.145401 sageworks-0.5.1/notebooks/images/
--rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.5.1/notebooks/images/athena_query_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.5.1/notebooks/images/aws_dashboard_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.5.1/notebooks/images/dashboard_aqsol_features.png
--rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.5.1/notebooks/images/model_screenshot.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.5.1/notebooks/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.5.1/notebooks/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)      431 2024-04-01 12:59:42.000000 sageworks-0.5.1/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.146646 sageworks-0.5.1/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.5.1/scripts/athena_ddl_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.5.1/scripts/copy_data_catalog_db.py
--rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.5.1/scripts/delete_redis_keys.py
--rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.5.1/scripts/glue_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.5.1/scripts/model_endpoint_sanity_check.py
--rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.5.1/scripts/onboard_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.5.1/scripts/onboard_models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.146892 sageworks-0.5.1/scripts/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.5.1/scripts/storage/dns_data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1723 2024-03-30 22:43:51.000000 sageworks-0.5.1/scripts/storage/generate_jsonl_data.py
--rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.5.1/scripts/test_feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)      533 2024-04-01 15:28:23.172223 sageworks-0.5.1/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1663 2024-03-27 20:32:27.000000 sageworks-0.5.1/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.113055 sageworks-0.5.1/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.147014 sageworks-0.5.1/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.147906 sageworks-0.5.1/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.1/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.148885 sageworks-0.5.1/src/sageworks/algorithms/dataframe/
--rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.5.1/src/sageworks/algorithms/dataframe/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/algorithms/dataframe/aggregation.py
--rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/algorithms/dataframe/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
--rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/algorithms/dataframe/feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)    12309 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/algorithms/dataframe/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/algorithms/dataframe/row_tagger.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.113421 sageworks-0.5.1/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.149043 sageworks-0.5.1/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.5.1/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.149170 sageworks-0.5.1/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.5.1/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.149290 sageworks-0.5.1/src/sageworks/algorithms/spark/
--rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.5.1/src/sageworks/algorithms/spark/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.150155 sageworks-0.5.1/src/sageworks/algorithms/sql/
--rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.5.1/src/sageworks/algorithms/sql/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     6192 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/algorithms/sql/column_stats.py
--rw-r--r--   0 briford    (501) staff       (20)     3645 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/algorithms/sql/correlations.py
--rw-r--r--   0 briford    (501) staff       (20)     3622 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/algorithms/sql/descriptive_stats.py
--rw-r--r--   0 briford    (501) staff       (20)    10174 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/algorithms/sql/outliers.py
--rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/algorithms/sql/sample_rows.py
--rw-r--r--   0 briford    (501) staff       (20)     3437 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/algorithms/sql/value_counts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.151024 sageworks-0.5.1/src/sageworks/api/
--rw-r--r--   0 briford    (501) staff       (20)      708 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/api/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/api/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/api/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     4242 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/api/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)    15642 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/api/meta.py
--rw-r--r--   0 briford    (501) staff       (20)     2577 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/api/model.py
--rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/api/monitor.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.151285 sageworks-0.5.1/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)    10908 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.152305 sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.152434 sageworks-0.5.1/src/sageworks/core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.153681 sageworks-0.5.1/src/sageworks/core/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    17938 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/core/artifacts/artifact.py
--rw-r--r--   0 briford    (501) staff       (20)    22432 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/core/artifacts/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/artifacts/data_source_abstract.py
--rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/artifacts/data_source_factory.py
--rw-r--r--   0 briford    (501) staff       (20)    36414 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/artifacts/endpoint_core.py
--rw-r--r--   0 briford    (501) staff       (20)    29123 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/artifacts/feature_set_core.py
--rw-r--r--   0 briford    (501) staff       (20)    35018 2024-03-29 21:27:39.000000 sageworks-0.5.1/src/sageworks/core/artifacts/model_core.py
--rw-r--r--   0 briford    (501) staff       (20)    21029 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/artifacts/monitor_core.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.154059 sageworks-0.5.1/src/sageworks/core/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.154193 sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.154432 sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.154931 sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.155072 sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.155181 sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.155290 sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.155412 sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.155743 sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.155877 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.155973 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.156180 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/heavy/chunk/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.156314 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.156438 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.156559 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/heavy/storage/
--rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.156957 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     4778 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.157104 sageworks-0.5.1/src/sageworks/core/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.115433 sageworks-0.5.1/src/sageworks/core/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.157207 sageworks-0.5.1/src/sageworks/core/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.157336 sageworks-0.5.1/src/sageworks/core/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.157554 sageworks-0.5.1/src/sageworks/core/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.157802 sageworks-0.5.1/src/sageworks/core/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.5.1/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)    10806 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.158056 sageworks-0.5.1/src/sageworks/core/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.159041 sageworks-0.5.1/src/sageworks/core/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/pandas_transforms/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     8604 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)    18139 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
--rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/core/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.159183 sageworks-0.5.1/src/sageworks/experiments/
--rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/experiments/view_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.159417 sageworks-0.5.1/src/sageworks/repl/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/repl/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    14538 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/repl/sageworks_shell.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.159692 sageworks-0.5.1/src/sageworks/resources/
--rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.5.1/src/sageworks/resources/open_source_api.key
--rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/resources/signature_verify_pub.pem
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.163721 sageworks-0.5.1/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.1/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15587 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/utils/aws_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5455 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/chem_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    16234 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/config_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/dashboard_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     4194 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/utils/datetime_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/docker_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.5.1/src/sageworks/utils/ecs_info.py
--rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/endpoint_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     3097 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/endpoint_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/extract_model_artifact.py
--rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/glue_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5757 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/license_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     1439 2024-03-28 17:32:59.000000 sageworks-0.5.1/src/sageworks/utils/markdown_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    13241 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    11623 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/plugin_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     9533 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/repl_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/s3_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/sageworks_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/sageworks_sqs.py
--rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.5.1/src/sageworks/utils/symbols.py
--rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/test_data_generator.py
--rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.5.1/src/sageworks/utils/trace_calls.py
--rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/utils/type_abbrev.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.164585 sageworks-0.5.1/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)     3318 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/views/artifacts_text_view.py
--rw-r--r--   0 briford    (501) staff       (20)     7008 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/views/artifacts_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3158 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/views/data_source_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2150 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/views/endpoint_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3206 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/views/feature_set_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2029 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/views/model_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/views/view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.166375 sageworks-0.5.1/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)      837 2023-12-24 17:18:24.000000 sageworks-0.5.1/src/sageworks/web_components/color_maps.py
--rw-r--r--   0 briford    (501) staff       (20)     4902 2024-03-31 15:44:39.000000 sageworks-0.5.1/src/sageworks/web_components/component_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     3521 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     5850 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/web_components/correlation_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     2970 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/web_components/dashboard_metric_plots.py
--rw-r--r--   0 briford    (501) staff       (20)     9335 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/web_components/data_details_markdown.py
--rw-r--r--   0 briford    (501) staff       (20)     4565 2024-03-28 17:35:30.000000 sageworks-0.5.1/src/sageworks/web_components/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)     3064 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/web_components/endpoint_metric_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.166861 sageworks-0.5.1/src/sageworks/web_components/experiments/
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/web_components/experiments/compound_details.py
--rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/web_components/experiments/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/web_components/experiments/outlier_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/web_components/experiments/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)      838 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/web_components/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     8550 2024-04-01 15:21:54.000000 sageworks-0.5.1/src/sageworks/web_components/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2270 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/web_components/model_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     6713 2024-03-31 15:44:39.000000 sageworks-0.5.1/src/sageworks/web_components/plugin_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     2941 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/web_components/regression_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     6535 2024-03-28 17:23:43.000000 sageworks-0.5.1/src/sageworks/web_components/table.py
--rw-r--r--   0 briford    (501) staff       (20)     5181 2024-03-30 22:43:51.000000 sageworks-0.5.1/src/sageworks/web_components/violin_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.171184 sageworks-0.5.1/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     4118 2024-04-01 15:28:22.000000 sageworks-0.5.1/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)    17057 2024-04-01 15:28:23.000000 sageworks-0.5.1/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2024-04-01 15:28:22.000000 sageworks-0.5.1/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)       74 2024-04-01 15:28:22.000000 sageworks-0.5.1/src/sageworks.egg-info/entry_points.txt
--rw-r--r--   0 briford    (501) staff       (20)      408 2024-04-01 15:28:22.000000 sageworks-0.5.1/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2024-04-01 15:28:22.000000 sageworks-0.5.1/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.167584 sageworks-0.5.1/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.168080 sageworks-0.5.1/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.5.1/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     2442 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.168336 sageworks-0.5.1/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.5.1/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.5.1/tests/aws_account/aws_service_broker_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.169075 sageworks-0.5.1/tests/connectors/
--rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/connectors/s3_bucket.py
--rw-r--r--   0 briford    (501) staff       (20)     5408 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/create_aqsol_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/create_basic_test_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/create_realtime_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     2379 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/create_training_adjusted_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/create_wine_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     4310 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/delete_test_artifacts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.169211 sageworks-0.5.1/tests/plugin_tests/
--rw-r--r--   0 briford    (501) staff       (20)     1888 2024-03-30 22:43:51.000000 sageworks-0.5.1/tests/plugin_tests/crashing_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.169475 sageworks-0.5.1/tests/specific/
--rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/specific/capital_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/specific/deletion_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.170255 sageworks-0.5.1/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     4864 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/transforms/model_metrics_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.5.1/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.5.1/tests/transforms/pandas_to_data_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 15:28:23.170887 sageworks-0.5.1/tests/web_components/
--rw-r--r--   0 briford    (501) staff       (20)      679 2024-03-30 22:43:51.000000 sageworks-0.5.1/tests/web_components/confusion_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)      675 2024-03-30 22:43:51.000000 sageworks-0.5.1/tests/web_components/correlation_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)     5210 2024-03-30 22:43:51.000000 sageworks-0.5.1/tests/web_components/plugin_interface_test.py
--rw-r--r--   0 briford    (501) staff       (20)     1115 2024-03-27 20:43:31.000000 sageworks-0.5.1/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.627915 sageworks-0.5.2/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.573795 sageworks-0.5.2/.github/
+-rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.5.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.5.2/.github/dependabot.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.574033 sageworks-0.5.2/.github/workflows/
+-rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.5.2/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.5.2/.github/workflows/python-lint.yml
+-rw-r--r--   0 briford    (501) staff       (20)     2008 2023-12-24 17:18:24.000000 sageworks-0.5.2/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      444 2024-03-28 17:23:43.000000 sageworks-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.5.2/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.5.2/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.5.2/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     4118 2024-04-01 16:27:58.627843 sageworks-0.5.2/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     2695 2024-03-28 17:23:43.000000 sageworks-0.5.2/README.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.5.2/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.564592 sageworks-0.5.2/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.575105 sageworks-0.5.2/applications/aws_dashboard/
+-rw-r--r--   0 briford    (501) staff       (20)     1071 2024-04-01 15:29:20.000000 sageworks-0.5.2/applications/aws_dashboard/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/Dockerfile_plugins
+-rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.5.2/applications/aws_dashboard/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1296 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.575477 sageworks-0.5.2/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    14995 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.5.2/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.5.2/applications/aws_dashboard/assets/trash.png
+-rwxr-xr-x   0 briford    (501) staff       (20)      644 2024-03-31 16:51:01.000000 sageworks-0.5.2/applications/aws_dashboard/dashboard
+-rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.5.2/applications/aws_dashboard/nginx.conf
+-rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/open_source_config.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.564513 sageworks-0.5.2/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.575842 sageworks-0.5.2/applications/aws_dashboard/pages/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)    11696 2024-03-30 22:43:51.000000 sageworks-0.5.2/applications/aws_dashboard/pages/data_sources/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/pages/data_sources/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/pages/data_sources/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.576498 sageworks-0.5.2/applications/aws_dashboard/pages/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)     3975 2024-03-30 22:43:51.000000 sageworks-0.5.2/applications/aws_dashboard/pages/endpoints/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2565 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/pages/endpoints/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2465 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/pages/endpoints/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.576971 sageworks-0.5.2/applications/aws_dashboard/pages/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)    11610 2024-03-30 22:43:51.000000 sageworks-0.5.2/applications/aws_dashboard/pages/feature_sets/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/pages/feature_sets/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/pages/feature_sets/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.577404 sageworks-0.5.2/applications/aws_dashboard/pages/main/
+-rw-r--r--   0 briford    (501) staff       (20)     4899 2024-03-30 22:43:51.000000 sageworks-0.5.2/applications/aws_dashboard/pages/main/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2899 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/pages/main/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/pages/main/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.577838 sageworks-0.5.2/applications/aws_dashboard/pages/models/
+-rw-r--r--   0 briford    (501) staff       (20)     3672 2024-03-30 22:43:51.000000 sageworks-0.5.2/applications/aws_dashboard/pages/models/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2020 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/pages/models/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2341 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/aws_dashboard/pages/models/page.py
+-rw-r--r--   0 briford    (501) staff       (20)      394 2024-04-01 13:00:51.000000 sageworks-0.5.2/applications/aws_dashboard/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.5.2/applications/aws_dashboard/supervisord.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.564648 sageworks-0.5.2/applications/experiments/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.578735 sageworks-0.5.2/applications/experiments/compound_explorer/
+-rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.5.2/applications/experiments/compound_explorer/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.5.2/applications/experiments/compound_explorer/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     3096 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/experiments/compound_explorer/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.579137 sageworks-0.5.2/applications/experiments/compound_explorer/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.5.2/applications/experiments/compound_explorer/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.5.2/applications/experiments/compound_explorer/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     7676 2024-03-30 22:43:51.000000 sageworks-0.5.2/applications/experiments/compound_explorer/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.5.2/applications/experiments/compound_explorer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.5.2/applications/experiments/compound_explorer/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.579608 sageworks-0.5.2/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.5.2/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.5.2/aws_setup/aws_identity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.5.2/aws_setup/build_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.579768 sageworks-0.5.2/aws_setup/event_bridge/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/event_bridge/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.580320 sageworks-0.5.2/aws_setup/event_bridge/dynamic_docker/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/event_bridge/dynamic_docker/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/event_bridge/dynamic_docker/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/event_bridge/dynamic_docker/cdk.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.580463 sageworks-0.5.2/aws_setup/event_bridge/dynamic_docker/lambda/
+-rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.5.2/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
+-rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.5.2/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.581318 sageworks-0.5.2/aws_setup/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_core/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_core/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.5.2/aws_setup/sageworks_core/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_core/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_core/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.5.2/aws_setup/sageworks_core/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.581537 sageworks-0.5.2/aws_setup/sageworks_core/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/aws_setup/sageworks_core/sageworks_core/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.5.2/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_core/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.581703 sageworks-0.5.2/aws_setup/sageworks_core/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_core/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.581913 sageworks-0.5.2/aws_setup/sageworks_core/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_core/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.582754 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.582977 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-01 15:32:28.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.583137 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.583406 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.584087 sageworks-0.5.2/aws_setup/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_lite/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_lite/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_lite/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_lite/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_lite/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.584334 sageworks-0.5.2/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     6849 2024-04-01 15:22:44.000000 sageworks-0.5.2/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.584979 sageworks-0.5.2/data/
+-rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.5.2/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.5.2/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.5.2/data/test_data.json
+-rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.5.2/data/wine_dataset.csv
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.585120 sageworks-0.5.2/docs/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.585369 sageworks-0.5.2/docs/admin/
+-rw-r--r--   0 briford    (501) staff       (20)     1825 2024-03-28 17:23:43.000000 sageworks-0.5.2/docs/admin/docker_push.md
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/admin/pypi_release.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.586264 sageworks-0.5.2/docs/api_classes/
+-rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.5.2/docs/api_classes/data_source.md
+-rw-r--r--   0 briford    (501) staff       (20)     5199 2024-03-28 17:23:43.000000 sageworks-0.5.2/docs/api_classes/endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.5.2/docs/api_classes/feature_set.md
+-rw-r--r--   0 briford    (501) staff       (20)     5350 2024-03-30 23:05:32.000000 sageworks-0.5.2/docs/api_classes/meta.md
+-rw-r--r--   0 briford    (501) staff       (20)     4356 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/api_classes/model.md
+-rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/api_classes/monitor.md
+-rw-r--r--   0 briford    (501) staff       (20)     3549 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/api_classes/overview.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.586969 sageworks-0.5.2/docs/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.5.2/docs/aws_setup/aws_access_management.md
+-rw-r--r--   0 briford    (501) staff       (20)     7836 2024-01-23 15:36:53.000000 sageworks-0.5.2/docs/aws_setup/aws_tips_and_tricks.md
+-rw-r--r--   0 briford    (501) staff       (20)     4229 2024-03-28 17:23:43.000000 sageworks-0.5.2/docs/aws_setup/core_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.5.2/docs/aws_setup/dashboard_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.5.2/docs/aws_setup/full_pipeline.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.587117 sageworks-0.5.2/docs/concepts/
+-rw-r--r--   0 briford    (501) staff       (20)      907 2024-01-23 15:36:53.000000 sageworks-0.5.2/docs/concepts/model_monitoring.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.587238 sageworks-0.5.2/docs/core_classes/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.588396 sageworks-0.5.2/docs/core_classes/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.5.2/docs/core_classes/artifacts/artifact.md
+-rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/core_classes/artifacts/athena_source.md
+-rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.5.2/docs/core_classes/artifacts/data_source_abstract.md
+-rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/core_classes/artifacts/endpoint_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/core_classes/artifacts/feature_set_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/core_classes/artifacts/model_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/core_classes/artifacts/monitor_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/core_classes/artifacts/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/core_classes/overview.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.589533 sageworks-0.5.2/docs/core_classes/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/core_classes/transforms/data_loaders_heavy.md
+-rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/core_classes/transforms/data_loaders_light.md
+-rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.5.2/docs/core_classes/transforms/data_to_features.md
+-rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/core_classes/transforms/features_to_model.md
+-rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/core_classes/transforms/model_to_endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/core_classes/transforms/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.5.2/docs/core_classes/transforms/pandas_transforms.md
+-rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.5.2/docs/core_classes/transforms/transform.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.589675 sageworks-0.5.2/docs/glue/
+-rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.5.2/docs/glue/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.591996 sageworks-0.5.2/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.5.2/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.5.2/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.5.2/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.5.2/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.5.2/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.5.2/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.5.2/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.5.2/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.5.2/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.5.2/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.5.2/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)     3417 2024-03-28 17:23:43.000000 sageworks-0.5.2/docs/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.592758 sageworks-0.5.2/docs/misc/
+-rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.5.2/docs/misc/faq.md
+-rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/misc/general_info.md
+-rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/misc/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.5.2/docs/misc/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.593045 sageworks-0.5.2/docs/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     3100 2024-04-01 00:11:00.000000 sageworks-0.5.2/docs/plugins/index.md
+-rw-r--r--   0 briford    (501) staff       (20)      750 2024-03-31 15:49:43.000000 sageworks-0.5.2/docs/plugins/plugin_api_changes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.593192 sageworks-0.5.2/docs/repl/
+-rw-r--r--   0 briford    (501) staff       (20)     2081 2024-03-28 17:23:43.000000 sageworks-0.5.2/docs/repl/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.593430 sageworks-0.5.2/docs/research/
+-rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.5.2/docs/research/eda.md
+-rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.5.2/docs/research/htg.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.596240 sageworks-0.5.2/examples/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.596385 sageworks-0.5.2/examples/ag-grid/
+-rw-r--r--   0 briford    (501) staff       (20)      496 2024-03-31 22:06:56.000000 sageworks-0.5.2/examples/ag-grid/hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.5.2/examples/datasource_from_df.py
+-rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.5.2/examples/datasource_from_s3.py
+-rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.5.2/examples/datasource_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.5.2/examples/datasource_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.5.2/examples/datasource_to_featureset.py
+-rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.5.2/examples/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      834 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.5.2/examples/endpoint_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.5.2/examples/featureset_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/featureset_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.5.2/examples/featureset_to_model.py
+-rw-r--r--   0 briford    (501) staff       (20)     1534 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/full_ml_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.5.2/examples/glue_hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.5.2/examples/glue_hello_world_with_log.py
+-rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.5.2/examples/glue_load_s3_bucket.py
+-rw-r--r--   0 briford    (501) staff       (20)      363 2024-03-30 22:43:51.000000 sageworks-0.5.2/examples/meta_list_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      328 2024-03-30 22:43:51.000000 sageworks-0.5.2/examples/meta_list_models.py
+-rw-r--r--   0 briford    (501) staff       (20)      659 2024-03-30 22:43:51.000000 sageworks-0.5.2/examples/meta_model_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)      548 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/model_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.5.2/examples/model_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.5.2/examples/monitor_setup.py
+-rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.5.2/examples/monitor_usage.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.567465 sageworks-0.5.2/examples/plugins/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.596530 sageworks-0.5.2/examples/plugins/pages/
+-rw-r--r--   0 briford    (501) staff       (20)     2474 2024-03-31 19:33:46.000000 sageworks-0.5.2/examples/plugins/pages/my_plugin_page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.596679 sageworks-0.5.2/examples/plugins/views/
+-rw-r--r--   0 briford    (501) staff       (20)     1264 2024-03-31 19:19:35.000000 sageworks-0.5.2/examples/plugins/views/my_view_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.596949 sageworks-0.5.2/examples/plugins/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     1666 2024-03-31 18:52:26.000000 sageworks-0.5.2/examples/plugins/web_components/endpoint_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     1942 2024-03-31 22:06:56.000000 sageworks-0.5.2/examples/plugins/web_components/model_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.597319 sageworks-0.5.2/examples/sagemaker_pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/sagemaker_pipelines/all_steps.py
+-rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/sagemaker_pipelines/hello.py
+-rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/sagemaker_pipelines/ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.567686 sageworks-0.5.2/examples/sagemaker_pipelines/storage/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.597972 sageworks-0.5.2/examples/sagemaker_pipelines/storage/full_pipeline_experiment/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.598580 sageworks-0.5.2/examples/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.5.2/examples/storage/data_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.5.2/examples/storage/data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1371 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/storage/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.5.2/examples/storage/hello_world_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     4378 2024-03-31 17:04:46.000000 sageworks-0.5.2/examples/storage/plugin_page_example.py
+-rw-r--r--   0 briford    (501) staff       (20)     2750 2024-03-31 15:47:34.000000 sageworks-0.5.2/mkdocs.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.599095 sageworks-0.5.2/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)   185443 2024-03-28 17:23:43.000000 sageworks-0.5.2/notebooks/ML_Pipeline_with_SageWorks.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)    36405 2024-03-28 17:23:43.000000 sageworks-0.5.2/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)   511134 2024-03-28 17:23:43.000000 sageworks-0.5.2/notebooks/Outliers_in_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.600736 sageworks-0.5.2/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.5.2/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.5.2/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.5.2/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.5.2/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.5.2/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.5.2/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      431 2024-04-01 12:59:42.000000 sageworks-0.5.2/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.602052 sageworks-0.5.2/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.5.2/scripts/athena_ddl_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.5.2/scripts/copy_data_catalog_db.py
+-rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.5.2/scripts/delete_redis_keys.py
+-rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.5.2/scripts/glue_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.5.2/scripts/model_endpoint_sanity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.5.2/scripts/onboard_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.5.2/scripts/onboard_models.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.602433 sageworks-0.5.2/scripts/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.5.2/scripts/storage/dns_data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1723 2024-03-30 22:43:51.000000 sageworks-0.5.2/scripts/storage/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.5.2/scripts/test_feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)      533 2024-04-01 16:27:58.628343 sageworks-0.5.2/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1663 2024-03-27 20:32:27.000000 sageworks-0.5.2/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.568260 sageworks-0.5.2/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.602575 sageworks-0.5.2/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.603503 sageworks-0.5.2/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.2/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.604418 sageworks-0.5.2/src/sageworks/algorithms/dataframe/
+-rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.5.2/src/sageworks/algorithms/dataframe/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/algorithms/dataframe/aggregation.py
+-rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/algorithms/dataframe/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
+-rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/algorithms/dataframe/feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)    12309 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/algorithms/dataframe/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/algorithms/dataframe/row_tagger.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.568616 sageworks-0.5.2/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.604544 sageworks-0.5.2/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.5.2/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.604673 sageworks-0.5.2/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.5.2/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.604803 sageworks-0.5.2/src/sageworks/algorithms/spark/
+-rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.5.2/src/sageworks/algorithms/spark/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.605853 sageworks-0.5.2/src/sageworks/algorithms/sql/
+-rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.5.2/src/sageworks/algorithms/sql/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     6192 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/algorithms/sql/column_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)     3645 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/algorithms/sql/correlations.py
+-rw-r--r--   0 briford    (501) staff       (20)     3622 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/algorithms/sql/descriptive_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)    10174 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/algorithms/sql/outliers.py
+-rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/algorithms/sql/sample_rows.py
+-rw-r--r--   0 briford    (501) staff       (20)     3437 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/algorithms/sql/value_counts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.606790 sageworks-0.5.2/src/sageworks/api/
+-rw-r--r--   0 briford    (501) staff       (20)      708 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/api/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/api/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/api/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     4242 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/api/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)    15642 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/api/meta.py
+-rw-r--r--   0 briford    (501) staff       (20)     2577 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/api/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/api/monitor.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.607071 sageworks-0.5.2/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)    10908 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.608089 sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.608214 sageworks-0.5.2/src/sageworks/core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.609378 sageworks-0.5.2/src/sageworks/core/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    17938 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/core/artifacts/artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)    22432 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/core/artifacts/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/artifacts/data_source_abstract.py
+-rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/artifacts/data_source_factory.py
+-rw-r--r--   0 briford    (501) staff       (20)    36414 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/artifacts/endpoint_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    29123 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/artifacts/feature_set_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    35018 2024-03-29 21:27:39.000000 sageworks-0.5.2/src/sageworks/core/artifacts/model_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    21029 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/artifacts/monitor_core.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.609737 sageworks-0.5.2/src/sageworks/core/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.609861 sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.610090 sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.610584 sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.610712 sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.610810 sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.610906 sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.611024 sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.611366 sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.611491 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.611595 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.611793 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/heavy/chunk/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.611921 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.612039 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.612165 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/heavy/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.612518 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     4778 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.612650 sageworks-0.5.2/src/sageworks/core/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.570595 sageworks-0.5.2/src/sageworks/core/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.612747 sageworks-0.5.2/src/sageworks/core/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.612870 sageworks-0.5.2/src/sageworks/core/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.613082 sageworks-0.5.2/src/sageworks/core/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.613331 sageworks-0.5.2/src/sageworks/core/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.5.2/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)    10806 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.613803 sageworks-0.5.2/src/sageworks/core/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.614683 sageworks-0.5.2/src/sageworks/core/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/pandas_transforms/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     8604 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)    18139 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
+-rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/core/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.614839 sageworks-0.5.2/src/sageworks/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/experiments/view_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.615089 sageworks-0.5.2/src/sageworks/repl/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/repl/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    14538 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/repl/sageworks_shell.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.615370 sageworks-0.5.2/src/sageworks/resources/
+-rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.5.2/src/sageworks/resources/open_source_api.key
+-rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/resources/signature_verify_pub.pem
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.619097 sageworks-0.5.2/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.2/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15587 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/utils/aws_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5455 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/chem_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    16234 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/config_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/dashboard_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     4194 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/utils/datetime_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/docker_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.5.2/src/sageworks/utils/ecs_info.py
+-rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/endpoint_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     3097 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/endpoint_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/extract_model_artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/glue_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5757 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/license_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     1439 2024-03-28 17:32:59.000000 sageworks-0.5.2/src/sageworks/utils/markdown_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    13241 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    11623 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/plugin_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     9533 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/repl_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/s3_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/sageworks_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/sageworks_sqs.py
+-rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.5.2/src/sageworks/utils/symbols.py
+-rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/test_data_generator.py
+-rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.5.2/src/sageworks/utils/trace_calls.py
+-rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/utils/type_abbrev.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.620140 sageworks-0.5.2/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)     3318 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/views/artifacts_text_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     7008 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/views/artifacts_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3158 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/views/data_source_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2150 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/views/endpoint_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3206 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/views/feature_set_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/views/model_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/views/view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.622387 sageworks-0.5.2/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)      837 2023-12-24 17:18:24.000000 sageworks-0.5.2/src/sageworks/web_components/color_maps.py
+-rw-r--r--   0 briford    (501) staff       (20)     4902 2024-03-31 15:44:39.000000 sageworks-0.5.2/src/sageworks/web_components/component_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3521 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     5850 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/web_components/correlation_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     2970 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/web_components/dashboard_metric_plots.py
+-rw-r--r--   0 briford    (501) staff       (20)     9335 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/web_components/data_details_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     4565 2024-03-28 17:35:30.000000 sageworks-0.5.2/src/sageworks/web_components/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     3064 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/web_components/endpoint_metric_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.622943 sageworks-0.5.2/src/sageworks/web_components/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/web_components/experiments/compound_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/web_components/experiments/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/web_components/experiments/outlier_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/web_components/experiments/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)      838 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/web_components/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     8716 2024-04-01 16:23:55.000000 sageworks-0.5.2/src/sageworks/web_components/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/web_components/model_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     6713 2024-03-31 15:44:39.000000 sageworks-0.5.2/src/sageworks/web_components/plugin_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     2941 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/web_components/regression_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     6535 2024-03-28 17:23:43.000000 sageworks-0.5.2/src/sageworks/web_components/table.py
+-rw-r--r--   0 briford    (501) staff       (20)     5181 2024-03-30 22:43:51.000000 sageworks-0.5.2/src/sageworks/web_components/violin_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.627408 sageworks-0.5.2/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     4118 2024-04-01 16:27:58.000000 sageworks-0.5.2/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)    17057 2024-04-01 16:27:58.000000 sageworks-0.5.2/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2024-04-01 16:27:58.000000 sageworks-0.5.2/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)       74 2024-04-01 16:27:58.000000 sageworks-0.5.2/src/sageworks.egg-info/entry_points.txt
+-rw-r--r--   0 briford    (501) staff       (20)      408 2024-04-01 16:27:58.000000 sageworks-0.5.2/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2024-04-01 16:27:58.000000 sageworks-0.5.2/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.623898 sageworks-0.5.2/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.624476 sageworks-0.5.2/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.5.2/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     2442 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.624759 sageworks-0.5.2/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.5.2/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.5.2/tests/aws_account/aws_service_broker_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.625612 sageworks-0.5.2/tests/connectors/
+-rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/connectors/s3_bucket.py
+-rw-r--r--   0 briford    (501) staff       (20)     5408 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/create_aqsol_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/create_basic_test_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/create_realtime_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     2379 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/create_training_adjusted_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/create_wine_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     4310 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/delete_test_artifacts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.625743 sageworks-0.5.2/tests/plugin_tests/
+-rw-r--r--   0 briford    (501) staff       (20)     1888 2024-03-30 22:43:51.000000 sageworks-0.5.2/tests/plugin_tests/crashing_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.626007 sageworks-0.5.2/tests/specific/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/specific/capital_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/specific/deletion_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.626830 sageworks-0.5.2/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     4864 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/transforms/model_metrics_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.5.2/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.5.2/tests/transforms/pandas_to_data_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 16:27:58.627189 sageworks-0.5.2/tests/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)      679 2024-03-30 22:43:51.000000 sageworks-0.5.2/tests/web_components/confusion_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      675 2024-03-30 22:43:51.000000 sageworks-0.5.2/tests/web_components/correlation_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     5210 2024-03-30 22:43:51.000000 sageworks-0.5.2/tests/web_components/plugin_interface_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     1115 2024-03-27 20:43:31.000000 sageworks-0.5.2/tox.ini
```

### Comparing `sageworks-0.5.1/.github/PULL_REQUEST_TEMPLATE.md` & `sageworks-0.5.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/.github/workflows/deploy-docs.yml` & `sageworks-0.5.2/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/.github/workflows/python-lint.yml` & `sageworks-0.5.2/.github/workflows/python-lint.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/.gitignore` & `sageworks-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/LICENSE` & `sageworks-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/Makefile` & `sageworks-0.5.2/Makefile`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/PKG-INFO` & `sageworks-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.5.1
+Version: 0.5.2
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sageworks-0.5.1/README.md` & `sageworks-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/Dockerfile` & `sageworks-0.5.2/applications/aws_dashboard/Dockerfile`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 RUN pip install --no-cache-dir -r requirements.txt
 
 # Copy the Nginx and Supervisor configuration files
 COPY nginx.conf /etc/nginx/sites-available/default
 COPY supervisord.conf /etc/supervisor/conf.d/supervisord.conf
 
 # Install Sageworks (changes often)
-RUN pip install --no-cache-dir sageworks==0.5.0
+RUN pip install --no-cache-dir sageworks==0.5.1
 
 # Copy the current directory contents into the container at /app
 COPY . /app
 
 # Grab the config file from build args, copy, and set ENV var
 ARG SAGEWORKS_CONFIG
 COPY $SAGEWORKS_CONFIG /app/sageworks_config.json
```

### Comparing `sageworks-0.5.1/applications/aws_dashboard/README.md` & `sageworks-0.5.2/applications/aws_dashboard/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/app.py` & `sageworks-0.5.2/applications/aws_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/assets/custom.css` & `sageworks-0.5.2/applications/aws_dashboard/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/assets/trash.png` & `sageworks-0.5.2/applications/aws_dashboard/assets/trash.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/dashboard` & `sageworks-0.5.2/applications/aws_dashboard/dashboard`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/open_source_config.json` & `sageworks-0.5.2/applications/aws_dashboard/open_source_config.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/data_sources/callbacks.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/data_sources/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/data_sources/layout.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/data_sources/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/data_sources/page.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/data_sources/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/endpoints/callbacks.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/endpoints/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/endpoints/layout.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/endpoints/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/endpoints/page.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/endpoints/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/feature_sets/callbacks.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/feature_sets/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/feature_sets/layout.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/feature_sets/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/feature_sets/page.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/feature_sets/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/main/callbacks.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/main/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/main/layout.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/main/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/main/page.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/main/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/models/callbacks.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/models/layout.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/models/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/aws_dashboard/pages/models/page.py` & `sageworks-0.5.2/applications/aws_dashboard/pages/models/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/experiments/compound_explorer/app.py` & `sageworks-0.5.2/applications/experiments/compound_explorer/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/experiments/compound_explorer/assets/custom.css` & `sageworks-0.5.2/applications/experiments/compound_explorer/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/experiments/compound_explorer/callbacks.py` & `sageworks-0.5.2/applications/experiments/compound_explorer/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/applications/experiments/compound_explorer/layout.py` & `sageworks-0.5.2/applications/experiments/compound_explorer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/aws_account_check.py` & `sageworks-0.5.2/aws_setup/aws_account_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/aws_identity_check.py` & `sageworks-0.5.2/aws_setup/aws_identity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/build_ml_pipeline.py` & `sageworks-0.5.2/aws_setup/build_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/event_bridge/dynamic_docker/app.py` & `sageworks-0.5.2/aws_setup/event_bridge/dynamic_docker/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/event_bridge/dynamic_docker/cdk.json` & `sageworks-0.5.2/aws_setup/event_bridge/dynamic_docker/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py` & `sageworks-0.5.2/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py` & `sageworks-0.5.2/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/sageworks_core/README.md` & `sageworks-0.5.2/aws_setup/sageworks_core/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/sageworks_core/app.py` & `sageworks-0.5.2/aws_setup/sageworks_core/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/sageworks_core/cdk.json` & `sageworks-0.5.2/aws_setup/sageworks_core/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py` & `sageworks-0.5.2/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py` & `sageworks-0.5.2/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/sageworks_dashboard_full/README.md` & `sageworks-0.5.2/aws_setup/sageworks_dashboard_full/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/sageworks_dashboard_full/app.py` & `sageworks-0.5.2/aws_setup/sageworks_dashboard_full/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/sageworks_dashboard_full/cdk.json` & `sageworks-0.5.2/aws_setup/sageworks_dashboard_full/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py` & `sageworks-0.5.2/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from aws_cdk.aws_ec2 import Subnet
 from aws_cdk.aws_certificatemanager import Certificate
 from aws_cdk.aws_ecs_patterns import ApplicationLoadBalancedFargateService
 from constructs import Construct
 
 # When you want a different version change this line
-dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_5_0_amd64"
+dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_5_1_amd64"
 
 
 class SageworksDashboardStackProps(StackProps):
     def __init__(
         self,
         sageworks_bucket: str,
         sageworks_api_key: str,
```

### Comparing `sageworks-0.5.1/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py` & `sageworks-0.5.2/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/sageworks_dashboard_lite/README.md` & `sageworks-0.5.2/aws_setup/sageworks_dashboard_lite/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/sageworks_dashboard_lite/app.py` & `sageworks-0.5.2/aws_setup/sageworks_dashboard_lite/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/sageworks_dashboard_lite/cdk.json` & `sageworks-0.5.2/aws_setup/sageworks_dashboard_lite/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py` & `sageworks-0.5.2/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/data/abalone.csv` & `sageworks-0.5.2/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/data/test_data.csv` & `sageworks-0.5.2/data/test_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/data/test_data.json` & `sageworks-0.5.2/data/test_data.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/data/wine_dataset.csv` & `sageworks-0.5.2/data/wine_dataset.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/admin/docker_push.md` & `sageworks-0.5.2/docs/admin/docker_push.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/admin/pypi_release.md` & `sageworks-0.5.2/docs/admin/pypi_release.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/api_classes/data_source.md` & `sageworks-0.5.2/docs/api_classes/data_source.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/api_classes/endpoint.md` & `sageworks-0.5.2/docs/api_classes/endpoint.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/api_classes/feature_set.md` & `sageworks-0.5.2/docs/api_classes/feature_set.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/api_classes/meta.md` & `sageworks-0.5.2/docs/api_classes/meta.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/api_classes/model.md` & `sageworks-0.5.2/docs/api_classes/model.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/api_classes/monitor.md` & `sageworks-0.5.2/docs/api_classes/monitor.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/api_classes/overview.md` & `sageworks-0.5.2/docs/api_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/aws_setup/aws_access_management.md` & `sageworks-0.5.2/docs/aws_setup/aws_access_management.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/aws_setup/aws_tips_and_tricks.md` & `sageworks-0.5.2/docs/aws_setup/aws_tips_and_tricks.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/aws_setup/core_stack.md` & `sageworks-0.5.2/docs/aws_setup/core_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/aws_setup/dashboard_stack.md` & `sageworks-0.5.2/docs/aws_setup/dashboard_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/aws_setup/full_pipeline.md` & `sageworks-0.5.2/docs/aws_setup/full_pipeline.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/concepts/model_monitoring.md` & `sageworks-0.5.2/docs/concepts/model_monitoring.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/core_classes/artifacts/overview.md` & `sageworks-0.5.2/docs/core_classes/artifacts/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/core_classes/overview.md` & `sageworks-0.5.2/docs/core_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/core_classes/transforms/overview.md` & `sageworks-0.5.2/docs/core_classes/transforms/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/core_classes/transforms/pandas_transforms.md` & `sageworks-0.5.2/docs/core_classes/transforms/pandas_transforms.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/core_classes/transforms/transform.md` & `sageworks-0.5.2/docs/core_classes/transforms/transform.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/glue/index.md` & `sageworks-0.5.2/docs/glue/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/images/big_spider.png` & `sageworks-0.5.2/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/images/graph_representation.png` & `sageworks-0.5.2/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/images/powered_aws_dark_blue.png` & `sageworks-0.5.2/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/images/powered_aws_transparent.png` & `sageworks-0.5.2/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/images/powered_aws_white.png` & `sageworks-0.5.2/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.5.2/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/images/sageworks.png` & `sageworks-0.5.2/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/images/sageworks_concepts.png` & `sageworks-0.5.2/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/images/scp.png` & `sageworks-0.5.2/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/images/scp_labs.png` & `sageworks-0.5.2/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/images/small_spider.png` & `sageworks-0.5.2/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/index.md` & `sageworks-0.5.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/misc/faq.md` & `sageworks-0.5.2/docs/misc/faq.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/misc/general_info.md` & `sageworks-0.5.2/docs/misc/general_info.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/misc/sageworks_classes_concepts.md` & `sageworks-0.5.2/docs/misc/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/misc/scp_consulting.md` & `sageworks-0.5.2/docs/misc/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/plugins/index.md` & `sageworks-0.5.2/docs/plugins/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/plugins/plugin_api_changes.md` & `sageworks-0.5.2/docs/plugins/plugin_api_changes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/repl/index.md` & `sageworks-0.5.2/docs/repl/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/research/eda.md` & `sageworks-0.5.2/docs/research/eda.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/docs/research/htg.md` & `sageworks-0.5.2/docs/research/htg.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/datasource_query.py` & `sageworks-0.5.2/examples/datasource_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/datasource_stats.py` & `sageworks-0.5.2/examples/datasource_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/endpoint_inference.py` & `sageworks-0.5.2/examples/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/featureset_eda.py` & `sageworks-0.5.2/examples/featureset_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/featureset_query.py` & `sageworks-0.5.2/examples/featureset_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/full_ml_pipeline.py` & `sageworks-0.5.2/examples/full_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/glue_hello_world.py` & `sageworks-0.5.2/examples/glue_hello_world.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/glue_hello_world_with_log.py` & `sageworks-0.5.2/examples/glue_hello_world_with_log.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/glue_load_s3_bucket.py` & `sageworks-0.5.2/examples/glue_load_s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/meta_model_metrics.py` & `sageworks-0.5.2/examples/meta_model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/model_metrics.py` & `sageworks-0.5.2/examples/model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/monitor_usage.py` & `sageworks-0.5.2/examples/monitor_usage.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/plugins/pages/my_plugin_page.py` & `sageworks-0.5.2/examples/plugins/pages/my_plugin_page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/plugins/views/my_view_plugin.py` & `sageworks-0.5.2/examples/plugins/views/my_view_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/plugins/web_components/endpoint_plugin.py` & `sageworks-0.5.2/examples/plugins/web_components/endpoint_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/plugins/web_components/model_plugin.py` & `sageworks-0.5.2/examples/plugins/web_components/model_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/sagemaker_pipelines/all_steps.py` & `sageworks-0.5.2/examples/sagemaker_pipelines/all_steps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/sagemaker_pipelines/ml_pipeline.py` & `sageworks-0.5.2/examples/sagemaker_pipelines/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py` & `sageworks-0.5.2/examples/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py` & `sageworks-0.5.2/examples/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/storage/data_to_data.py` & `sageworks-0.5.2/examples/storage/data_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/storage/data_to_features.py` & `sageworks-0.5.2/examples/storage/data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/storage/endpoint_inference.py` & `sageworks-0.5.2/examples/storage/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/storage/hello_world_pipeline.py` & `sageworks-0.5.2/examples/storage/hello_world_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/examples/storage/plugin_page_example.py` & `sageworks-0.5.2/examples/storage/plugin_page_example.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/mkdocs.yml` & `sageworks-0.5.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/notebooks/ML_Pipeline_with_SageWorks.ipynb` & `sageworks-0.5.2/notebooks/ML_Pipeline_with_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/notebooks/ML_Pipeline_with_SageWorks_2.ipynb` & `sageworks-0.5.2/notebooks/ML_Pipeline_with_SageWorks_2.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/notebooks/Outliers_in_SageWorks.ipynb` & `sageworks-0.5.2/notebooks/Outliers_in_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/notebooks/images/athena_query_aqsol.png` & `sageworks-0.5.2/notebooks/images/athena_query_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/notebooks/images/aws_dashboard_aqsol.png` & `sageworks-0.5.2/notebooks/images/aws_dashboard_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/notebooks/images/dashboard_aqsol_features.png` & `sageworks-0.5.2/notebooks/images/dashboard_aqsol_features.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/notebooks/images/model_screenshot.png` & `sageworks-0.5.2/notebooks/images/model_screenshot.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/notebooks/images/sageworks_concepts.png` & `sageworks-0.5.2/notebooks/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/notebooks/images/scp_labs.png` & `sageworks-0.5.2/notebooks/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/scripts/athena_ddl_mixed_case.py` & `sageworks-0.5.2/scripts/athena_ddl_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/scripts/copy_data_catalog_db.py` & `sageworks-0.5.2/scripts/copy_data_catalog_db.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/scripts/delete_redis_keys.py` & `sageworks-0.5.2/scripts/delete_redis_keys.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/scripts/glue_mixed_case.py` & `sageworks-0.5.2/scripts/glue_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/scripts/model_endpoint_sanity_check.py` & `sageworks-0.5.2/scripts/model_endpoint_sanity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/scripts/onboard_endpoints.py` & `sageworks-0.5.2/scripts/onboard_endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/scripts/onboard_models.py` & `sageworks-0.5.2/scripts/onboard_models.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/scripts/storage/dns_data_to_features.py` & `sageworks-0.5.2/scripts/storage/dns_data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/scripts/storage/generate_jsonl_data.py` & `sageworks-0.5.2/scripts/storage/generate_jsonl_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/scripts/test_feature_resolution.py` & `sageworks-0.5.2/scripts/test_feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/setup.cfg` & `sageworks-0.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/setup.py` & `sageworks-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/__init__.py` & `sageworks-0.5.2/src/sageworks/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/dataframe/aggregation.py` & `sageworks-0.5.2/src/sageworks/algorithms/dataframe/aggregation.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/dataframe/data_source_eda.py` & `sageworks-0.5.2/src/sageworks/algorithms/dataframe/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/dataframe/dimensionality_reduction.py` & `sageworks-0.5.2/src/sageworks/algorithms/dataframe/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/dataframe/feature_resolution.py` & `sageworks-0.5.2/src/sageworks/algorithms/dataframe/feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/dataframe/feature_spider.py` & `sageworks-0.5.2/src/sageworks/algorithms/dataframe/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/dataframe/row_tagger.py` & `sageworks-0.5.2/src/sageworks/algorithms/dataframe/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/spark/Readme.md` & `sageworks-0.5.2/src/sageworks/algorithms/spark/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/sql/Readme.md` & `sageworks-0.5.2/src/sageworks/algorithms/sql/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/sql/column_stats.py` & `sageworks-0.5.2/src/sageworks/algorithms/sql/column_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/sql/correlations.py` & `sageworks-0.5.2/src/sageworks/algorithms/sql/correlations.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/sql/descriptive_stats.py` & `sageworks-0.5.2/src/sageworks/algorithms/sql/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/sql/outliers.py` & `sageworks-0.5.2/src/sageworks/algorithms/sql/outliers.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/sql/sample_rows.py` & `sageworks-0.5.2/src/sageworks/algorithms/sql/sample_rows.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/algorithms/sql/value_counts.py` & `sageworks-0.5.2/src/sageworks/algorithms/sql/value_counts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/api/__init__.py` & `sageworks-0.5.2/src/sageworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/api/data_source.py` & `sageworks-0.5.2/src/sageworks/api/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/api/endpoint.py` & `sageworks-0.5.2/src/sageworks/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/api/feature_set.py` & `sageworks-0.5.2/src/sageworks/api/feature_set.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/api/meta.py` & `sageworks-0.5.2/src/sageworks/api/meta.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/api/model.py` & `sageworks-0.5.2/src/sageworks/api/model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/api/monitor.py` & `sageworks-0.5.2/src/sageworks/api/monitor.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.5.2/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_broker.py` & `sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_broker.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/connector.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py` & `sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py` & `sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py` & `sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.5.2/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/artifacts/__init__.py` & `sageworks-0.5.2/src/sageworks/core/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/artifacts/artifact.py` & `sageworks-0.5.2/src/sageworks/core/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/artifacts/athena_source.py` & `sageworks-0.5.2/src/sageworks/core/artifacts/athena_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/artifacts/data_source_abstract.py` & `sageworks-0.5.2/src/sageworks/core/artifacts/data_source_abstract.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/artifacts/data_source_factory.py` & `sageworks-0.5.2/src/sageworks/core/artifacts/data_source_factory.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/artifacts/endpoint_core.py` & `sageworks-0.5.2/src/sageworks/core/artifacts/endpoint_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/artifacts/feature_set_core.py` & `sageworks-0.5.2/src/sageworks/core/artifacts/feature_set_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/artifacts/model_core.py` & `sageworks-0.5.2/src/sageworks/core/artifacts/model_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/artifacts/monitor_core.py` & `sageworks-0.5.2/src/sageworks/core/artifacts/monitor_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/Readme.md` & `sageworks-0.5.2/src/sageworks/core/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/light/__init__.py` & `sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/light/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py` & `sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py` & `sageworks-0.5.2/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/light/clean_data.py` & `sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/light/clean_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.5.2/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py` & `sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py` & `sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py` & `sageworks-0.5.2/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/features_to_model/features_to_model.py` & `sageworks-0.5.2/src/sageworks/core/transforms/features_to_model/features_to_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.5.2/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.5.2/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/pandas_transforms/__init__.py` & `sageworks-0.5.2/src/sageworks/core/transforms/pandas_transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.5.2/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py` & `sageworks-0.5.2/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py` & `sageworks-0.5.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py` & `sageworks-0.5.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py` & `sageworks-0.5.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/core/transforms/transform.py` & `sageworks-0.5.2/src/sageworks/core/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/experiments/view_manager.py` & `sageworks-0.5.2/src/sageworks/experiments/view_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/repl/sageworks_shell.py` & `sageworks-0.5.2/src/sageworks/repl/sageworks_shell.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/aws_utils.py` & `sageworks-0.5.2/src/sageworks/utils/aws_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/cache.py` & `sageworks-0.5.2/src/sageworks/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/chem_utils.py` & `sageworks-0.5.2/src/sageworks/utils/chem_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/config_manager.py` & `sageworks-0.5.2/src/sageworks/utils/config_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/dashboard_metrics.py` & `sageworks-0.5.2/src/sageworks/utils/dashboard_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/datetime_utils.py` & `sageworks-0.5.2/src/sageworks/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.5.2/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/docker_utils.py` & `sageworks-0.5.2/src/sageworks/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/ecs_info.py` & `sageworks-0.5.2/src/sageworks/utils/ecs_info.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/endpoint_metrics.py` & `sageworks-0.5.2/src/sageworks/utils/endpoint_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/endpoint_utils.py` & `sageworks-0.5.2/src/sageworks/utils/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/extract_model_artifact.py` & `sageworks-0.5.2/src/sageworks/utils/extract_model_artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/glue_utils.py` & `sageworks-0.5.2/src/sageworks/utils/glue_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/license_manager.py` & `sageworks-0.5.2/src/sageworks/utils/license_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/markdown_utils.py` & `sageworks-0.5.2/src/sageworks/utils/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/pandas_utils.py` & `sageworks-0.5.2/src/sageworks/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/plugin_manager.py` & `sageworks-0.5.2/src/sageworks/utils/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/redis_cache.py` & `sageworks-0.5.2/src/sageworks/utils/redis_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/repl_utils.py` & `sageworks-0.5.2/src/sageworks/utils/repl_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/s3_utils.py` & `sageworks-0.5.2/src/sageworks/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/sageworks_cache.py` & `sageworks-0.5.2/src/sageworks/utils/sageworks_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.5.2/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.5.2/src/sageworks/utils/sageworks_logging.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.5.2/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/symbols.py` & `sageworks-0.5.2/src/sageworks/utils/symbols.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/test_data_generator.py` & `sageworks-0.5.2/src/sageworks/utils/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/trace_calls.py` & `sageworks-0.5.2/src/sageworks/utils/trace_calls.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/utils/type_abbrev.py` & `sageworks-0.5.2/src/sageworks/utils/type_abbrev.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/views/artifacts_text_view.py` & `sageworks-0.5.2/src/sageworks/views/artifacts_text_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/views/artifacts_web_view.py` & `sageworks-0.5.2/src/sageworks/views/artifacts_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/views/data_source_web_view.py` & `sageworks-0.5.2/src/sageworks/views/data_source_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/views/endpoint_web_view.py` & `sageworks-0.5.2/src/sageworks/views/endpoint_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/views/feature_set_web_view.py` & `sageworks-0.5.2/src/sageworks/views/feature_set_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/views/model_web_view.py` & `sageworks-0.5.2/src/sageworks/views/model_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/views/view.py` & `sageworks-0.5.2/src/sageworks/views/view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/color_maps.py` & `sageworks-0.5.2/src/sageworks/web_components/color_maps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/component_interface.py` & `sageworks-0.5.2/src/sageworks/web_components/component_interface.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.5.2/src/sageworks/web_components/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/correlation_matrix.py` & `sageworks-0.5.2/src/sageworks/web_components/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/dashboard_metric_plots.py` & `sageworks-0.5.2/src/sageworks/web_components/dashboard_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/data_details_markdown.py` & `sageworks-0.5.2/src/sageworks/web_components/data_details_markdown.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/endpoint_details.py` & `sageworks-0.5.2/src/sageworks/web_components/endpoint_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/endpoint_metric_plots.py` & `sageworks-0.5.2/src/sageworks/web_components/endpoint_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/experiments/compound_details.py` & `sageworks-0.5.2/src/sageworks/web_components/experiments/compound_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/experiments/histogram.py` & `sageworks-0.5.2/src/sageworks/web_components/experiments/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/experiments/outlier_plot.py` & `sageworks-0.5.2/src/sageworks/web_components/experiments/outlier_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/experiments/scatter_plot.py` & `sageworks-0.5.2/src/sageworks/web_components/experiments/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/line_chart.py` & `sageworks-0.5.2/src/sageworks/web_components/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/model_details.py` & `sageworks-0.5.2/src/sageworks/web_components/model_details.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 class ModelDetails(ComponentInterface):
     """Model Markdown Component"""
 
     def __init__(self):
         self.prefix_id = ""
         self.model = None
         super().__init__()
+        self.metrics_just_updated = False
 
     def create_component(self, component_id: str) -> html.Div:
         """Create a Markdown Component without any data.
         Args:
             component_id (str): The ID of the web component
         Returns:
             html.Div: A Container of Components for the Model Details
@@ -66,26 +67,28 @@
             summary = self.model_summary()
 
             # Populate the inference runs dropdown
             inference_runs, default_run = self.get_inference_runs()
 
             # Update the metrics for the default inference run
             metrics = self.inference_metrics(default_run)
+            self.metrics_just_updated = True
 
             # Return the updated components
             return header, summary, inference_runs, default_run, metrics
 
         @callback(
             Output(f"{self.prefix_id}-metrics", "children", allow_duplicate=True),
             Input(f"{self.prefix_id}-dropdown", "value"),
             prevent_initial_call=True,
         )
         def update_inference_run(inference_run):
             # Check for no inference run
-            if not inference_run:
+            if not inference_run or self.metrics_just_updated:
+                self.metrics_just_updated = False
                 return no_update
 
             # Update the model metrics
             metrics = self.inference_metrics(inference_run)
 
             return metrics
```

### Comparing `sageworks-0.5.1/src/sageworks/web_components/model_plot.py` & `sageworks-0.5.2/src/sageworks/web_components/model_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/plugin_interface.py` & `sageworks-0.5.2/src/sageworks/web_components/plugin_interface.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/regression_plot.py` & `sageworks-0.5.2/src/sageworks/web_components/regression_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/table.py` & `sageworks-0.5.2/src/sageworks/web_components/table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks/web_components/violin_plots.py` & `sageworks-0.5.2/src/sageworks/web_components/violin_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/src/sageworks.egg-info/PKG-INFO` & `sageworks-0.5.2/src/sageworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.5.1
+Version: 0.5.2
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sageworks-0.5.1/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.5.2/src/sageworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/artifacts/data_source_tests.py` & `sageworks-0.5.2/tests/artifacts/data_source_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/artifacts/endpoint_tests.py` & `sageworks-0.5.2/tests/artifacts/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/artifacts/feature_set_tests.py` & `sageworks-0.5.2/tests/artifacts/feature_set_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/artifacts/model_tests.py` & `sageworks-0.5.2/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/aws_account/aws_account_clamp_tests.py` & `sageworks-0.5.2/tests/aws_account/aws_account_clamp_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.5.2/tests/aws_account/aws_service_broker_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/connectors/data_catalog.py` & `sageworks-0.5.2/tests/connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/connectors/endpoints.py` & `sageworks-0.5.2/tests/connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/connectors/feature_store.py` & `sageworks-0.5.2/tests/connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/connectors/glue_jobs.py` & `sageworks-0.5.2/tests/connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/connectors/model_registry.py` & `sageworks-0.5.2/tests/connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/connectors/s3_bucket.py` & `sageworks-0.5.2/tests/connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/create_aqsol_artifacts.py` & `sageworks-0.5.2/tests/create_aqsol_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/create_basic_test_artifacts.py` & `sageworks-0.5.2/tests/create_basic_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/create_realtime_endpoint.py` & `sageworks-0.5.2/tests/create_realtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/create_training_adjusted_artifacts.py` & `sageworks-0.5.2/tests/create_training_adjusted_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/create_wine_artifacts.py` & `sageworks-0.5.2/tests/create_wine_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/delete_test_artifacts.py` & `sageworks-0.5.2/tests/delete_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/plugin_tests/crashing_plugin.py` & `sageworks-0.5.2/tests/plugin_tests/crashing_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/specific/capital_tests.py` & `sageworks-0.5.2/tests/specific/capital_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/specific/deletion_tests.py` & `sageworks-0.5.2/tests/specific/deletion_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/transforms/data_to_data_tests.py` & `sageworks-0.5.2/tests/transforms/data_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/transforms/data_to_features_tests.py` & `sageworks-0.5.2/tests/transforms/data_to_features_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/transforms/features_to_model_tests.py` & `sageworks-0.5.2/tests/transforms/features_to_model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/transforms/model_metrics_tests.py` & `sageworks-0.5.2/tests/transforms/model_metrics_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.5.2/tests/transforms/model_to_endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.5.2/tests/transforms/pandas_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/web_components/confusion_matrix_test.py` & `sageworks-0.5.2/tests/web_components/confusion_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/web_components/correlation_matrix_test.py` & `sageworks-0.5.2/tests/web_components/correlation_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tests/web_components/plugin_interface_test.py` & `sageworks-0.5.2/tests/web_components/plugin_interface_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.1/tox.ini` & `sageworks-0.5.2/tox.ini`

 * *Files identical despite different names*


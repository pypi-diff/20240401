# Comparing `tmp/scalifiai-client-1.2.0a4.tar.gz` & `tmp/scalifiai-client-1.2.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalifiai-client-1.2.0a4.tar", last modified: Mon Apr  1 15:38:14 2024, max compression
+gzip compressed data, was "scalifiai-client-1.2.0a5.tar", last modified: Mon Apr  1 15:41:05 2024, max compression
```

## Comparing `scalifiai-client-1.2.0a4.tar` & `scalifiai-client-1.2.0a5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:38:14.079123 scalifiai-client-1.2.0a4/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.2.0a4/LICENSE
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      899 2024-04-01 15:38:14.079123 scalifiai-client-1.2.0a4/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.2.0a4/README.md
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      971 2024-04-01 15:37:56.000000 scalifiai-client-1.2.0a4/pyproject.toml
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:38:14.071123 scalifiai-client-1.2.0a4/scalifiai/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a4/scalifiai/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6361 2024-04-01 15:37:36.000000 scalifiai-client-1.2.0a4/scalifiai/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-03-30 16:03:04.000000 scalifiai-client-1.2.0a4/scalifiai/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a4/scalifiai/credentials.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a4/scalifiai/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:38:14.071123 scalifiai-client-1.2.0a4/scalifiai/mcs/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-02-22 09:41:30.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:38:14.071123 scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:38:14.075123 scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/keras/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/keras/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       63 2024-02-19 07:02:09.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/keras/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-03-29 10:10:16.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/keras/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    11074 2024-03-31 04:37:07.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/keras/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-02-28 14:26:26.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/schema.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1800 2024-04-01 13:26:53.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/utils.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/main.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:38:14.075123 scalifiai-client-1.2.0a4/scalifiai/mcs/metadata/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/metadata/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-01 07:00:53.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/metadata/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-03-30 16:01:07.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/metadata/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13338 2024-04-01 15:35:11.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/metadata/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-02-28 12:22:03.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/metadata/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:38:14.075123 scalifiai-client-1.2.0a4/scalifiai/mcs/model/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/model/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-03-30 11:24:30.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/model/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-03-30 15:59:35.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/model/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    34019 2024-04-01 15:37:25.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/model/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/model/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:38:14.075123 scalifiai-client-1.2.0a4/scalifiai/mcs/model_version/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/model_version/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-03-30 11:20:38.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/model_version/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-03-30 15:58:50.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/model_version/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28423 2024-04-01 15:37:42.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/model_version/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a4/scalifiai/mcs/model_version/schemas.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-03-30 16:03:04.000000 scalifiai-client-1.2.0a4/scalifiai/request_manager.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:38:14.079123 scalifiai-client-1.2.0a4/scalifiai_client.egg-info/
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      899 2024-04-01 15:38:14.000000 scalifiai-client-1.2.0a4/scalifiai_client.egg-info/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1353 2024-04-01 15:38:14.000000 scalifiai-client-1.2.0a4/scalifiai_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-01 15:38:14.000000 scalifiai-client-1.2.0a4/scalifiai_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      138 2024-04-01 15:38:14.000000 scalifiai-client-1.2.0a4/scalifiai_client.egg-info/requires.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-01 15:38:14.000000 scalifiai-client-1.2.0a4/scalifiai_client.egg-info/top_level.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-01 15:38:14.079123 scalifiai-client-1.2.0a4/setup.cfg
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:41:05.178513 scalifiai-client-1.2.0a5/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.2.0a5/LICENSE
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      899 2024-04-01 15:41:05.178513 scalifiai-client-1.2.0a5/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.2.0a5/README.md
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      971 2024-04-01 15:40:53.000000 scalifiai-client-1.2.0a5/pyproject.toml
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:41:05.174513 scalifiai-client-1.2.0a5/scalifiai/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a5/scalifiai/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6401 2024-04-01 15:40:25.000000 scalifiai-client-1.2.0a5/scalifiai/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-03-30 16:03:04.000000 scalifiai-client-1.2.0a5/scalifiai/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a5/scalifiai/credentials.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a5/scalifiai/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:41:05.174513 scalifiai-client-1.2.0a5/scalifiai/mcs/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-02-22 09:41:30.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:41:05.174513 scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:41:05.174513 scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/keras/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/keras/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       63 2024-02-19 07:02:09.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/keras/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-03-29 10:10:16.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/keras/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    11074 2024-03-31 04:37:07.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/keras/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-02-28 14:26:26.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/schema.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1800 2024-04-01 13:26:53.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/utils.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/main.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:41:05.174513 scalifiai-client-1.2.0a5/scalifiai/mcs/metadata/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/metadata/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-01 07:00:53.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/metadata/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-03-30 16:01:07.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/metadata/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13378 2024-04-01 15:40:31.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/metadata/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-02-28 12:22:03.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/metadata/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:41:05.178513 scalifiai-client-1.2.0a5/scalifiai/mcs/model/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/model/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-03-30 11:24:30.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/model/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-03-30 15:59:35.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/model/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    34019 2024-04-01 15:37:25.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/model/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/model/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:41:05.178513 scalifiai-client-1.2.0a5/scalifiai/mcs/model_version/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/model_version/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-03-30 11:20:38.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/model_version/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-03-30 15:58:50.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/model_version/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28463 2024-04-01 15:40:35.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/model_version/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a5/scalifiai/mcs/model_version/schemas.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-03-30 16:03:04.000000 scalifiai-client-1.2.0a5/scalifiai/request_manager.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:41:05.178513 scalifiai-client-1.2.0a5/scalifiai_client.egg-info/
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      899 2024-04-01 15:41:05.000000 scalifiai-client-1.2.0a5/scalifiai_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1353 2024-04-01 15:41:05.000000 scalifiai-client-1.2.0a5/scalifiai_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-01 15:41:05.000000 scalifiai-client-1.2.0a5/scalifiai_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      138 2024-04-01 15:41:05.000000 scalifiai-client-1.2.0a5/scalifiai_client.egg-info/requires.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-01 15:41:05.000000 scalifiai-client-1.2.0a5/scalifiai_client.egg-info/top_level.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-01 15:41:05.178513 scalifiai-client-1.2.0a5/setup.cfg
```

### Comparing `scalifiai-client-1.2.0a4/PKG-INFO` & `scalifiai-client-1.2.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.2.0a4
+Version: 1.2.0a5
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,12 +12,12 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pandas>=1.3.0
 Requires-Dist: humanize>=2.0.0
 Requires-Dist: tzlocal>=2.1
 Provides-Extra: tf
-Requires-Dist: tensorflow==2.2.0; extra == "tf"
+Requires-Dist: tensorflow==2.0.0; extra == "tf"
 Requires-Dist: pydantic>=2.0; extra == "tf"
 Requires-Dist: pandas>=1.3.0; extra == "tf"
 Requires-Dist: humanize>=2.0.0; extra == "tf"
 Requires-Dist: tzlocal>=2.1; extra == "tf"
```

### Comparing `scalifiai-client-1.2.0a4/pyproject.toml` & `scalifiai-client-1.2.0a5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scalifiai-client"
-version = "1.2.0-alpha.4"
+version = "1.2.0-alpha.5"
 description = "SCALIFI AI NO CODE PLATFORM"
 readme = "README.md"
 authors = [{ name = "Scalifi Ai", email = "helpdesk@scalifiai.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -21,15 +21,15 @@
     "humanize >= 2.0.0",
     "tzlocal >= 2.1",
 ]
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
 tf = [
-    "tensorflow == 2.2.0",
+    "tensorflow == 2.0.0",
     "pydantic >= 2.0",
     "pandas >= 1.3.0",
     "humanize >= 2.0.0",
     "tzlocal >= 2.1",
 ]
 
 [project.urls]
```

### Comparing `scalifiai-client-1.2.0a4/scalifiai/base.py` & `scalifiai-client-1.2.0a5/scalifiai/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     def convert_datetime(self, value):
 
         if pd.isna(value) == False:
             value = pd.to_datetime(value)
             if (datetime.now(self.local_timezone) - value).days > 0:
                 value = humanize.naturaldate(value)
             else:
-                value = humanize.naturaltime(value)
+                value = humanize.naturaltime(value, when=datetime.now(self.local_timezone))
 
         return value
 
     def convert_size(self, value):
 
         if pd.isna(value) == False:
             value = humanize.naturalsize(value)
```

### Comparing `scalifiai-client-1.2.0a4/scalifiai/credentials.py` & `scalifiai-client-1.2.0a5/scalifiai/credentials.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/exceptions.py` & `scalifiai-client-1.2.0a5/scalifiai/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/exceptions.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/exceptions.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/keras/exceptions.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/keras/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/keras/main.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/keras/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/schema.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/schema.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/frameworks/utils.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/frameworks/utils.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/main.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/metadata/exceptions.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/metadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/metadata/main.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/metadata/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
             # TODO[VIMPORTANT] GENERALIZE THIS SO THAT WE CAN APPLY ANY FUNCTION TO ANY FIELDS BY SPECIFYINGIT IN THE VERBOSE COLUMNS CONFIG, CAN ALSO USE FUNCTIONS OF TABLE IN base.py
             if key in ["created_at", "updated_at"]:
                 final_value = pd.to_datetime(final_value)
                 if (datetime.now(self.local_timezone) - final_value).days > 0:
                     final_value = humanize.naturaldate(final_value)
                 else:
-                    final_value = humanize.naturaltime(final_value)
+                    final_value = humanize.naturaltime(final_value, when=datetime.now(self.local_timezone))
 
             # TODO[VIMPORTANT] GENERALIZE THIS SO THAT WE CAN APPLY ANY FUNCTION TO ANY FIELDS BY SPECIFYINGIT IN THE VERBOSE COLUMNS CONFIG, CAN ALSO USE FUNCTIONS OF TABLE IN base.py
             if key == "properties__file_size":
                 final_value = humanize.naturalsize(final_value)
 
             html_content += f"<tr><th>{final_key}</th><td>{final_value}</td></tr>"
         html_content += "</table>"
```

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/metadata/schemas.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/metadata/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/model/constants.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/model/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/model/exceptions.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/model/main.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/model/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/model/schemas.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/model/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/model_version/constants.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/model_version/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/model_version/exceptions.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/model_version/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/model_version/main.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/model_version/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
             # TODO[VIMPORTANT] GENERALIZE THIS SO THAT WE CAN APPLY ANY FUNCTION TO ANY FIELDS BY SPECIFYINGIT IN THE VERBOSE COLUMNS CONFIG, CAN ALSO USE FUNCTIONS OF TABLE IN base.py
             if key in ["created_at", "updated_at"]:
                 final_value = pd.to_datetime(final_value)
                 if (datetime.now(self.local_timezone) - final_value).days > 0:
                     final_value = humanize.naturaldate(final_value)
                 else:
-                    final_value = humanize.naturaltime(final_value)
+                    final_value = humanize.naturaltime(final_value, when=datetime.now(self.local_timezone))
 
             html_content += f"<tr><th>{final_key}</th><td>{final_value}</td></tr>"
         html_content += "</table>"
         return HTML(html_content)
 
     # TODO[VIMPORTANT] ADD THIS PROPERTY TO ALL SUB-MODULES
     @property
```

### Comparing `scalifiai-client-1.2.0a4/scalifiai/mcs/model_version/schemas.py` & `scalifiai-client-1.2.0a5/scalifiai/mcs/model_version/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai/request_manager.py` & `scalifiai-client-1.2.0a5/scalifiai/request_manager.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a4/scalifiai_client.egg-info/PKG-INFO` & `scalifiai-client-1.2.0a5/scalifiai_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.2.0a4
+Version: 1.2.0a5
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,12 +12,12 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pandas>=1.3.0
 Requires-Dist: humanize>=2.0.0
 Requires-Dist: tzlocal>=2.1
 Provides-Extra: tf
-Requires-Dist: tensorflow==2.2.0; extra == "tf"
+Requires-Dist: tensorflow==2.0.0; extra == "tf"
 Requires-Dist: pydantic>=2.0; extra == "tf"
 Requires-Dist: pandas>=1.3.0; extra == "tf"
 Requires-Dist: humanize>=2.0.0; extra == "tf"
 Requires-Dist: tzlocal>=2.1; extra == "tf"
```

### Comparing `scalifiai-client-1.2.0a4/scalifiai_client.egg-info/SOURCES.txt` & `scalifiai-client-1.2.0a5/scalifiai_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/scalifiai-client-1.1.0a2.tar.gz` & `tmp/scalifiai-client-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalifiai-client-1.1.0a2.tar", last modified: Sat Mar 30 19:38:13 2024, max compression
+gzip compressed data, was "scalifiai-client-1.2.0a1.tar", last modified: Mon Apr  1 15:14:14 2024, max compression
```

## Comparing `scalifiai-client-1.1.0a2.tar` & `scalifiai-client-1.2.0a1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-30 19:38:13.433029 scalifiai-client-1.1.0a2/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.1.0a2/LICENSE
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      722 2024-03-30 19:38:13.433029 scalifiai-client-1.1.0a2/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.1.0a2/README.md
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      876 2024-03-30 19:37:54.000000 scalifiai-client-1.1.0a2/pyproject.toml
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-30 19:38:13.425029 scalifiai-client-1.1.0a2/scalifiai/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-02-19 06:55:52.000000 scalifiai-client-1.1.0a2/scalifiai/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6361 2024-03-30 10:55:47.000000 scalifiai-client-1.1.0a2/scalifiai/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-03-30 16:03:04.000000 scalifiai-client-1.1.0a2/scalifiai/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-02-19 06:55:52.000000 scalifiai-client-1.1.0a2/scalifiai/credentials.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-03-30 13:31:27.000000 scalifiai-client-1.1.0a2/scalifiai/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-30 19:38:13.425029 scalifiai-client-1.1.0a2/scalifiai/mcs/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-02-22 09:41:30.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-02-19 06:55:52.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-03-30 13:31:27.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-30 19:38:13.429029 scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-02-19 06:55:52.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-03-30 13:31:27.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-30 19:38:13.429029 scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/keras/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/keras/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       63 2024-02-19 07:02:09.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/keras/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-03-29 10:10:16.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/keras/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    10882 2024-03-30 13:31:27.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/keras/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-02-28 14:26:26.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/schema.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1609 2024-03-30 19:37:29.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/utils.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-03-30 13:31:27.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/main.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-30 19:38:13.429029 scalifiai-client-1.1.0a2/scalifiai/mcs/metadata/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/metadata/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      385 2024-03-30 12:30:47.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/metadata/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-03-30 16:01:07.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/metadata/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13338 2024-03-30 13:31:28.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/metadata/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-02-28 12:22:03.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/metadata/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-30 19:38:13.429029 scalifiai-client-1.1.0a2/scalifiai/mcs/model/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/model/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-03-30 11:24:30.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/model/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-03-30 15:59:35.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/model/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    33979 2024-03-30 13:31:28.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/model/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-03-30 13:31:27.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/model/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-30 19:38:13.433029 scalifiai-client-1.1.0a2/scalifiai/mcs/model_version/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/model_version/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-03-30 11:20:38.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/model_version/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-03-30 15:58:50.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/model_version/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28423 2024-03-30 13:31:28.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/model_version/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-03-30 13:31:27.000000 scalifiai-client-1.1.0a2/scalifiai/mcs/model_version/schemas.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-03-30 16:03:04.000000 scalifiai-client-1.1.0a2/scalifiai/request_manager.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-30 19:38:13.433029 scalifiai-client-1.1.0a2/scalifiai_client.egg-info/
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      722 2024-03-30 19:38:13.000000 scalifiai-client-1.1.0a2/scalifiai_client.egg-info/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1353 2024-03-30 19:38:13.000000 scalifiai-client-1.1.0a2/scalifiai_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-03-30 19:38:13.000000 scalifiai-client-1.1.0a2/scalifiai_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       81 2024-03-30 19:38:13.000000 scalifiai-client-1.1.0a2/scalifiai_client.egg-info/requires.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-03-30 19:38:13.000000 scalifiai-client-1.1.0a2/scalifiai_client.egg-info/top_level.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-03-30 19:38:13.433029 scalifiai-client-1.1.0a2/setup.cfg
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:14:14.840153 scalifiai-client-1.2.0a1/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.2.0a1/LICENSE
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      899 2024-04-01 15:14:14.840153 scalifiai-client-1.2.0a1/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.2.0a1/README.md
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      971 2024-04-01 15:14:03.000000 scalifiai-client-1.2.0a1/pyproject.toml
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:14:14.832153 scalifiai-client-1.2.0a1/scalifiai/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a1/scalifiai/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6361 2024-03-30 10:55:47.000000 scalifiai-client-1.2.0a1/scalifiai/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-03-30 16:03:04.000000 scalifiai-client-1.2.0a1/scalifiai/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a1/scalifiai/credentials.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a1/scalifiai/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:14:14.832153 scalifiai-client-1.2.0a1/scalifiai/mcs/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-02-22 09:41:30.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:14:14.832153 scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:14:14.832153 scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/keras/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/keras/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       63 2024-02-19 07:02:09.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/keras/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-03-29 10:10:16.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/keras/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    11074 2024-03-31 04:37:07.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/keras/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-02-28 14:26:26.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/schema.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1800 2024-04-01 13:26:53.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/utils.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/main.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:14:14.836153 scalifiai-client-1.2.0a1/scalifiai/mcs/metadata/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/metadata/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-01 07:00:53.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/metadata/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-03-30 16:01:07.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/metadata/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13338 2024-03-30 13:31:28.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/metadata/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-02-28 12:22:03.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/metadata/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:14:14.836153 scalifiai-client-1.2.0a1/scalifiai/mcs/model/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/model/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-03-30 11:24:30.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/model/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-03-30 15:59:35.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/model/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    33979 2024-03-30 13:31:28.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/model/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/model/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:14:14.836153 scalifiai-client-1.2.0a1/scalifiai/mcs/model_version/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/model_version/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-03-30 11:20:38.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/model_version/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-03-30 15:58:50.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/model_version/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28423 2024-03-30 13:31:28.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/model_version/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a1/scalifiai/mcs/model_version/schemas.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-03-30 16:03:04.000000 scalifiai-client-1.2.0a1/scalifiai/request_manager.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:14:14.840153 scalifiai-client-1.2.0a1/scalifiai_client.egg-info/
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      899 2024-04-01 15:14:14.000000 scalifiai-client-1.2.0a1/scalifiai_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1353 2024-04-01 15:14:14.000000 scalifiai-client-1.2.0a1/scalifiai_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-01 15:14:14.000000 scalifiai-client-1.2.0a1/scalifiai_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      138 2024-04-01 15:14:14.000000 scalifiai-client-1.2.0a1/scalifiai_client.egg-info/requires.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-01 15:14:14.000000 scalifiai-client-1.2.0a1/scalifiai_client.egg-info/top_level.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-01 15:14:14.840153 scalifiai-client-1.2.0a1/setup.cfg
```

### Comparing `scalifiai-client-1.1.0a2/scalifiai/base.py` & `scalifiai-client-1.2.0a1/scalifiai/base.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/credentials.py` & `scalifiai-client-1.2.0a1/scalifiai/credentials.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/exceptions.py` & `scalifiai-client-1.2.0a1/scalifiai/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/exceptions.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/exceptions.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/keras/exceptions.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/keras/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/keras/main.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/keras/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     def infer_data_type(self, *, dtype):
 
         data_type = self.DATA_TYPE_CONVERSION.get(dtype, None)
 
         if data_type == None:
             raise KerasInvalidDataTypeModelException(
-                extra_info=f"Invalid data type: {dtype}"
+                extra_info=f"Invalid data type: {dtype} || Type(dtype): {type(dtype)}"
             )
 
         return data_type
 
     def infer_signature(self):
 
         inputs = None
@@ -153,22 +153,25 @@
         request_manager=None,
         upload_url=None,
         parent_action=None,
         model_instance=None,
     ):
 
         from scalifiai.mcs.model_version.main import ModelVersion
+        # import tensorflow as tf
 
         with tempfile.TemporaryDirectory(dir=base_dir_path) as temp_dir:
 
             temp_dir_path = Path(temp_dir)
             model_save_file_path = temp_dir_path / Path(MODEL_SAVE_FOLDER_NAME)
 
             try:
                 self.model.save(model_save_file_path, save_format="tf")
+                # self.model.save(model_save_file_path)
+                # tf.saved_model.save(self.model, model_save_file_path)
             except Exception as ex:
                 print(f"type(ex): {type(ex)}")
                 print(f"ex: {ex}")
                 try:
                     raise KerasInvalidModelException(extra_info=str(ex))
                 except Exception as ex:
                     raise KerasInvalidModelException()
```

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/schema.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/schema.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/frameworks/utils.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/frameworks/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 
     KERAS = (
         [
             "keras.src.engine.sequential",
             "keras.src.engine.functional",
             "keras.src.models.sequential",
             "keras.src.models.functional",
+            "tensorflow.python.keras.engine.sequential",
+            "tensorflow.python.keras.engine.functional",
+            "keras.engine.sequential",
+            "keras.engine.functional"
         ],
         "Keras - Tensorflow",
         KerasModelWrapper,
     )
 
     @classmethod
     def match_model(cls, model):
```

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/main.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/metadata/exceptions.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/metadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/metadata/main.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/metadata/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/metadata/schemas.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/metadata/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/model/constants.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/model/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/model/exceptions.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/model/main.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/model/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/model/schemas.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/model/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/model_version/constants.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/model_version/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/model_version/exceptions.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/model_version/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/model_version/main.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/model_version/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/mcs/model_version/schemas.py` & `scalifiai-client-1.2.0a1/scalifiai/mcs/model_version/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai/request_manager.py` & `scalifiai-client-1.2.0a1/scalifiai/request_manager.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.0a2/scalifiai_client.egg-info/SOURCES.txt` & `scalifiai-client-1.2.0a1/scalifiai_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*


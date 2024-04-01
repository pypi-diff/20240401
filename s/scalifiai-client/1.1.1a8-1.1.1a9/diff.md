# Comparing `tmp/scalifiai-client-1.1.1a8.tar.gz` & `tmp/scalifiai-client-1.1.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalifiai-client-1.1.1a8.tar", last modified: Mon Apr  1 08:20:23 2024, max compression
+gzip compressed data, was "scalifiai-client-1.1.1a9.tar", last modified: Mon Apr  1 08:26:00 2024, max compression
```

## Comparing `scalifiai-client-1.1.1a8.tar` & `scalifiai-client-1.1.1a9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:20:23.907555 scalifiai-client-1.1.1a8/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.1.1a8/LICENSE
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      798 2024-04-01 08:20:23.907555 scalifiai-client-1.1.1a8/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.1.1a8/README.md
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      927 2024-04-01 08:20:12.000000 scalifiai-client-1.1.1a8/pyproject.toml
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:20:23.899555 scalifiai-client-1.1.1a8/scalifiai/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a8/scalifiai/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6361 2024-03-30 10:55:47.000000 scalifiai-client-1.1.1a8/scalifiai/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-03-30 16:03:04.000000 scalifiai-client-1.1.1a8/scalifiai/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a8/scalifiai/credentials.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-03-30 13:31:27.000000 scalifiai-client-1.1.1a8/scalifiai/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:20:23.903555 scalifiai-client-1.1.1a8/scalifiai/mcs/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-02-22 09:41:30.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-03-30 13:31:27.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:20:23.903555 scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-03-30 13:31:27.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:20:23.903555 scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/keras/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/keras/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       63 2024-02-19 07:02:09.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/keras/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-03-29 10:10:16.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/keras/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    11074 2024-03-31 04:37:07.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/keras/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-02-28 14:26:26.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/schema.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1665 2024-04-01 08:04:56.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/utils.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-03-30 13:31:27.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/main.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:20:23.903555 scalifiai-client-1.1.1a8/scalifiai/mcs/metadata/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/metadata/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-01 07:00:53.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/metadata/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-03-30 16:01:07.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/metadata/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13338 2024-03-30 13:31:28.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/metadata/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-02-28 12:22:03.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/metadata/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:20:23.903555 scalifiai-client-1.1.1a8/scalifiai/mcs/model/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/model/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-03-30 11:24:30.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/model/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-03-30 15:59:35.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/model/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    33979 2024-03-30 13:31:28.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/model/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-03-30 13:31:27.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/model/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:20:23.907555 scalifiai-client-1.1.1a8/scalifiai/mcs/model_version/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/model_version/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-03-30 11:20:38.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/model_version/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-03-30 15:58:50.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/model_version/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28423 2024-03-30 13:31:28.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/model_version/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-03-30 13:31:27.000000 scalifiai-client-1.1.1a8/scalifiai/mcs/model_version/schemas.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-03-30 16:03:04.000000 scalifiai-client-1.1.1a8/scalifiai/request_manager.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:20:23.907555 scalifiai-client-1.1.1a8/scalifiai_client.egg-info/
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      798 2024-04-01 08:20:23.000000 scalifiai-client-1.1.1a8/scalifiai_client.egg-info/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1353 2024-04-01 08:20:23.000000 scalifiai-client-1.1.1a8/scalifiai_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-01 08:20:23.000000 scalifiai-client-1.1.1a8/scalifiai_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      112 2024-04-01 08:20:23.000000 scalifiai-client-1.1.1a8/scalifiai_client.egg-info/requires.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-01 08:20:23.000000 scalifiai-client-1.1.1a8/scalifiai_client.egg-info/top_level.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-01 08:20:23.907555 scalifiai-client-1.1.1a8/setup.cfg
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:26:00.150222 scalifiai-client-1.1.1a9/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.1.1a9/LICENSE
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      766 2024-04-01 08:26:00.146222 scalifiai-client-1.1.1a9/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.1.1a9/README.md
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      901 2024-04-01 08:23:36.000000 scalifiai-client-1.1.1a9/pyproject.toml
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:26:00.142222 scalifiai-client-1.1.1a9/scalifiai/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a9/scalifiai/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6361 2024-03-30 10:55:47.000000 scalifiai-client-1.1.1a9/scalifiai/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-03-30 16:03:04.000000 scalifiai-client-1.1.1a9/scalifiai/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a9/scalifiai/credentials.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-03-30 13:31:27.000000 scalifiai-client-1.1.1a9/scalifiai/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:26:00.142222 scalifiai-client-1.1.1a9/scalifiai/mcs/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-02-22 09:41:30.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-03-30 13:31:27.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:26:00.142222 scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-03-30 13:31:27.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:26:00.142222 scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/keras/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/keras/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       63 2024-02-19 07:02:09.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/keras/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-03-29 10:10:16.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/keras/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    11074 2024-03-31 04:37:07.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/keras/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-02-28 14:26:26.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/schema.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1665 2024-04-01 08:04:56.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/utils.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-03-30 13:31:27.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/main.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:26:00.142222 scalifiai-client-1.1.1a9/scalifiai/mcs/metadata/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/metadata/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-01 07:00:53.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/metadata/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-03-30 16:01:07.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/metadata/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13338 2024-03-30 13:31:28.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/metadata/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-02-28 12:22:03.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/metadata/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:26:00.146222 scalifiai-client-1.1.1a9/scalifiai/mcs/model/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/model/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-03-30 11:24:30.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/model/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-03-30 15:59:35.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/model/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    33979 2024-03-30 13:31:28.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/model/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-03-30 13:31:27.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/model/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:26:00.146222 scalifiai-client-1.1.1a9/scalifiai/mcs/model_version/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/model_version/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-03-30 11:20:38.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/model_version/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-03-30 15:58:50.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/model_version/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28423 2024-03-30 13:31:28.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/model_version/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-03-30 13:31:27.000000 scalifiai-client-1.1.1a9/scalifiai/mcs/model_version/schemas.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-03-30 16:03:04.000000 scalifiai-client-1.1.1a9/scalifiai/request_manager.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 08:26:00.146222 scalifiai-client-1.1.1a9/scalifiai_client.egg-info/
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      766 2024-04-01 08:26:00.000000 scalifiai-client-1.1.1a9/scalifiai_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1353 2024-04-01 08:26:00.000000 scalifiai-client-1.1.1a9/scalifiai_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-01 08:26:00.000000 scalifiai-client-1.1.1a9/scalifiai_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       95 2024-04-01 08:26:00.000000 scalifiai-client-1.1.1a9/scalifiai_client.egg-info/requires.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-01 08:26:00.000000 scalifiai-client-1.1.1a9/scalifiai_client.egg-info/top_level.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-01 08:26:00.150222 scalifiai-client-1.1.1a9/setup.cfg
```

### Comparing `scalifiai-client-1.1.1a8/PKG-INFO` & `scalifiai-client-1.1.1a9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.1.1a8
+Version: 1.1.1a9
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pandas>=1.3.0
 Requires-Dist: humanize>=2.0.0
 Requires-Dist: tzlocal>=2.1
-Requires-Dist: requests>=2.15.0
 Provides-Extra: tf
-Requires-Dist: tensorflow>=2.4.0; extra == "tf"
+Requires-Dist: tensorflow>=2.0.0; extra == "tf"
 Requires-Dist: pandas>=1.3.0; extra == "tf"
```

### Comparing `scalifiai-client-1.1.1a8/pyproject.toml` & `scalifiai-client-1.1.1a9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scalifiai-client"
-version = "1.1.1-alpha.8"
+version = "1.1.1-alpha.9"
 description = "SCALIFI AI NO CODE PLATFORM"
 readme = "README.md"
 authors = [{ name = "Scalifi Ai", email = "helpdesk@scalifiai.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -16,19 +16,18 @@
 ]
 keywords = ["ai", "ml", "artificial intelligence", "machine learning", "no-code", "no code", "low-code", "low code", "big-data", "big data"]
 dependencies = [
     "pydantic >= 2.0",
     "pandas >= 1.3.0",
     "humanize >= 2.0.0",
     "tzlocal >= 2.1",
-    "requests >= 2.15.0",
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 
 [project.optional-dependencies]
 tf = [
-    "tensorflow >= 2.4.0",
+    "tensorflow >= 2.0.0",
     "pandas >= 1.3.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Ai-Bloc-24"
```

### Comparing `scalifiai-client-1.1.1a8/scalifiai/base.py` & `scalifiai-client-1.1.1a9/scalifiai/base.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/credentials.py` & `scalifiai-client-1.1.1a9/scalifiai/credentials.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/exceptions.py` & `scalifiai-client-1.1.1a9/scalifiai/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/exceptions.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/exceptions.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/keras/exceptions.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/keras/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/keras/main.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/keras/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/schema.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/schema.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/frameworks/utils.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/frameworks/utils.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/main.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/metadata/exceptions.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/metadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/metadata/main.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/metadata/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/metadata/schemas.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/metadata/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/model/constants.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/model/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/model/exceptions.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/model/main.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/model/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/model/schemas.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/model/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/model_version/constants.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/model_version/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/model_version/exceptions.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/model_version/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/model_version/main.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/model_version/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/mcs/model_version/schemas.py` & `scalifiai-client-1.1.1a9/scalifiai/mcs/model_version/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai/request_manager.py` & `scalifiai-client-1.1.1a9/scalifiai/request_manager.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.1.1a8/scalifiai_client.egg-info/PKG-INFO` & `scalifiai-client-1.1.1a9/scalifiai_client.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.1.1a8
+Version: 1.1.1a9
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pandas>=1.3.0
 Requires-Dist: humanize>=2.0.0
 Requires-Dist: tzlocal>=2.1
-Requires-Dist: requests>=2.15.0
 Provides-Extra: tf
-Requires-Dist: tensorflow>=2.4.0; extra == "tf"
+Requires-Dist: tensorflow>=2.0.0; extra == "tf"
 Requires-Dist: pandas>=1.3.0; extra == "tf"
```

### Comparing `scalifiai-client-1.1.1a8/scalifiai_client.egg-info/SOURCES.txt` & `scalifiai-client-1.1.1a9/scalifiai_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*


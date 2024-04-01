# Comparing `tmp/yayawallet-python-sdk-0.1.8.tar.gz` & `tmp/yayawallet-python-sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yayawallet-python-sdk-0.1.8.tar", last modified: Sat Mar 30 07:59:00 2024, max compression
+gzip compressed data, was "yayawallet-python-sdk-0.1.9.tar", last modified: Sat Mar 30 08:05:02 2024, max compression
```

## Comparing `yayawallet-python-sdk-0.1.8.tar` & `yayawallet-python-sdk-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 07:59:00.157537 yayawallet-python-sdk-0.1.8/
--rw-rw-rw-   0        0        0      132 2024-03-30 07:59:00.155559 yayawallet-python-sdk-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      108 2024-03-27 11:46:10.000000 yayawallet-python-sdk-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-03-30 07:59:00.157537 yayawallet-python-sdk-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      219 2024-03-30 07:52:21.000000 yayawallet-python-sdk-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-30 07:59:00.095409 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/
--rw-rw-rw-   0        0        0        0 2024-03-30 07:36:36.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 07:59:00.142696 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-03-29 08:25:45.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/__init__.py
--rw-rw-rw-   0        0        0      340 2024-03-27 06:52:07.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/airtime.py
--rw-rw-rw-   0        0        0     2596 2024-03-27 06:52:07.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/equb.py
--rw-rw-rw-   0        0        0      216 2024-03-27 06:52:07.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/institution.py
--rw-rw-rw-   0        0        0      409 2024-03-27 06:52:07.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/invitation.py
--rw-rw-rw-   0        0        0     1829 2024-03-27 11:33:38.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/recurring_contract.py
--rw-rw-rw-   0        0        0      639 2024-03-29 11:12:46.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/saving.py
--rw-rw-rw-   0        0        0     1251 2024-03-27 06:52:07.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/transaction.py
--rw-rw-rw-   0        0        0     1020 2024-03-27 06:52:07.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/transfer.py
--rw-rw-rw-   0        0        0      299 2024-03-30 07:58:16.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/user.py
-drwxrwxrwx   0        0        0        0 2024-03-30 07:59:00.152290 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/functions/
--rw-rw-rw-   0        0        0        0 2024-03-29 08:25:54.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/functions/__init__.py
--rw-rw-rw-   0        0        0     1677 2024-03-30 07:36:23.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/functions/api_request.py
--rw-rw-rw-   0        0        0      419 2024-03-27 06:52:07.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/functions/generate_signature.py
--rw-rw-rw-   0        0        0      347 2024-03-30 07:36:12.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/functions/get_time.py
-drwxrwxrwx   0        0        0        0 2024-03-30 07:59:00.154515 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk.egg-info/
--rw-rw-rw-   0        0        0      132 2024-03-30 07:59:00.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      808 2024-03-30 07:59:00.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 07:59:00.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-03-30 07:59:00.000000 yayawallet-python-sdk-0.1.8/yayawallet_python_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-30 08:05:02.726228 yayawallet-python-sdk-0.1.9/
+-rw-rw-rw-   0        0        0      132 2024-03-30 08:05:02.724226 yayawallet-python-sdk-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2024-03-27 11:46:10.000000 yayawallet-python-sdk-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-30 08:05:02.726228 yayawallet-python-sdk-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      219 2024-03-30 08:04:46.000000 yayawallet-python-sdk-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-30 08:05:02.671072 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/
+-rw-rw-rw-   0        0        0        0 2024-03-30 07:36:36.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-30 08:05:02.710422 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-03-29 08:25:45.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0      340 2024-03-27 06:52:07.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/airtime.py
+-rw-rw-rw-   0        0        0     2596 2024-03-27 06:52:07.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/equb.py
+-rw-rw-rw-   0        0        0      216 2024-03-27 06:52:07.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/institution.py
+-rw-rw-rw-   0        0        0      409 2024-03-27 06:52:07.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/invitation.py
+-rw-rw-rw-   0        0        0     1829 2024-03-27 11:33:38.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/recurring_contract.py
+-rw-rw-rw-   0        0        0      639 2024-03-29 11:12:46.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/saving.py
+-rw-rw-rw-   0        0        0     1251 2024-03-27 06:52:07.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/transaction.py
+-rw-rw-rw-   0        0        0     1020 2024-03-27 06:52:07.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/transfer.py
+-rw-rw-rw-   0        0        0      299 2024-03-30 07:58:16.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/user.py
+drwxrwxrwx   0        0        0        0 2024-03-30 08:05:02.715309 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/functions/
+-rw-rw-rw-   0        0        0        0 2024-03-29 08:25:54.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/functions/__init__.py
+-rw-rw-rw-   0        0        0     1677 2024-03-30 07:36:23.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/functions/api_request.py
+-rw-rw-rw-   0        0        0      424 2024-03-30 08:04:28.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/functions/generate_signature.py
+-rw-rw-rw-   0        0        0      347 2024-03-30 07:36:12.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/functions/get_time.py
+drwxrwxrwx   0        0        0        0 2024-03-30 08:05:02.715309 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0      132 2024-03-30 08:05:02.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      808 2024-03-30 08:05:02.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-30 08:05:02.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-03-30 08:05:02.000000 yayawallet-python-sdk-0.1.9/yayawallet_python_sdk.egg-info/top_level.txt
```

### Comparing `yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/equb.py` & `yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/equb.py`

 * *Files identical despite different names*

### Comparing `yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/recurring_contract.py` & `yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/recurring_contract.py`

 * *Files identical despite different names*

### Comparing `yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/saving.py` & `yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/saving.py`

 * *Files identical despite different names*

### Comparing `yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/transaction.py` & `yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/transaction.py`

 * *Files identical despite different names*

### Comparing `yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/api/transfer.py` & `yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/api/transfer.py`

 * *Files identical despite different names*

### Comparing `yayawallet-python-sdk-0.1.8/yayawallet_python_sdk/functions/api_request.py` & `yayawallet-python-sdk-0.1.9/yayawallet_python_sdk/functions/api_request.py`

 * *Files identical despite different names*

### Comparing `yayawallet-python-sdk-0.1.8/yayawallet_python_sdk.egg-info/SOURCES.txt` & `yayawallet-python-sdk-0.1.9/yayawallet_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/upload_manager-1.1.0.tar.gz` & `tmp/upload_manager-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upload_manager-1.1.0.tar", last modified: Mon Jun 19 08:31:08 2023, max compression
+gzip compressed data, was "/Users/dharmesh/workspace/python/bbuploadmanager/dist/.tmp-y2fmxa4f/upload_manager-1.1.1.tar", last modified: Mon Apr  1 12:23:33 2024, max compression
```

## Comparing `upload_manager-1.1.0.tar` & `upload_manager-1.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2023-06-19 08:31:08.866213 upload_manager-1.1.0/
--rw-r--r--   0 dharmesh   (502) staff       (20)     1144 2021-02-10 09:04:07.000000 upload_manager-1.1.0/LICENSE.md
--rw-r--r--   0 dharmesh   (502) staff       (20)      114 2021-03-02 13:09:30.000000 upload_manager-1.1.0/MANIFEST.in
--rw-r--r--   0 dharmesh   (502) staff       (20)     2703 2023-06-19 08:31:08.865967 upload_manager-1.1.0/PKG-INFO
--rw-r--r--   0 dharmesh   (502) staff       (20)     2132 2021-03-02 13:17:30.000000 upload_manager-1.1.0/README.md
-drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2023-06-19 08:31:08.856236 upload_manager-1.1.0/images/
--rw-r--r--   0 dharmesh   (502) staff       (20)   200603 2021-03-02 12:37:59.000000 upload_manager-1.1.0/images/dashboard.png
--rw-rw-r--   0 dharmesh   (502) staff       (20)       67 2021-02-10 13:25:58.000000 upload_manager-1.1.0/requirements.txt
--rw-r--r--   0 dharmesh   (502) staff       (20)       38 2023-06-19 08:31:08.866282 upload_manager-1.1.0/setup.cfg
--rw-r--r--   0 dharmesh   (502) staff       (20)      981 2023-06-19 08:30:35.000000 upload_manager-1.1.0/setup.py
-drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2023-06-19 08:31:08.858377 upload_manager-1.1.0/tests/
--rw-r--r--   0 dharmesh   (502) staff       (20)        0 2021-02-10 06:21:51.000000 upload_manager-1.1.0/tests/__init__.py
--rw-r--r--   0 dharmesh   (502) staff       (20)      621 2021-02-10 13:58:22.000000 upload_manager-1.1.0/tests/test_s3.py
-drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2023-06-19 08:31:08.863682 upload_manager-1.1.0/upload_manager/
--rw-rw-r--   0 dharmesh   (502) staff       (20)        0 2020-08-07 09:11:53.000000 upload_manager-1.1.0/upload_manager/__init__.py
--rw-r--r--   0 dharmesh   (502) staff       (20)     1196 2022-11-04 06:16:29.000000 upload_manager-1.1.0/upload_manager/admin.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)      138 2021-03-02 12:35:59.000000 upload_manager-1.1.0/upload_manager/apps.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)      626 2020-08-07 09:11:53.000000 upload_manager-1.1.0/upload_manager/file_operator.py
-drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2023-06-19 08:31:08.865697 upload_manager-1.1.0/upload_manager/migrations/
--rw-rw-r--   0 dharmesh   (502) staff       (20)     1477 2020-08-07 09:11:53.000000 upload_manager-1.1.0/upload_manager/migrations/0001_initial.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)        0 2020-08-07 09:11:53.000000 upload_manager-1.1.0/upload_manager/migrations/__init__.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)     1527 2020-08-07 09:11:53.000000 upload_manager-1.1.0/upload_manager/models.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)     4503 2021-02-01 17:23:37.000000 upload_manager-1.1.0/upload_manager/s3.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)     6052 2021-03-01 11:28:31.000000 upload_manager-1.1.0/upload_manager/service.py
--rw-r--r--   0 dharmesh   (502) staff       (20)      169 2023-06-19 07:21:57.000000 upload_manager-1.1.0/upload_manager/urls.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)      445 2020-08-07 09:11:53.000000 upload_manager-1.1.0/upload_manager/utils.py
--rw-r--r--   0 dharmesh   (502) staff       (20)     1747 2023-06-19 07:21:57.000000 upload_manager-1.1.0/upload_manager/views.py
-drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2023-06-19 08:31:08.865092 upload_manager-1.1.0/upload_manager.egg-info/
--rw-r--r--   0 dharmesh   (502) staff       (20)     2703 2023-06-19 08:31:08.000000 upload_manager-1.1.0/upload_manager.egg-info/PKG-INFO
--rw-r--r--   0 dharmesh   (502) staff       (20)      632 2023-06-19 08:31:08.000000 upload_manager-1.1.0/upload_manager.egg-info/SOURCES.txt
--rw-r--r--   0 dharmesh   (502) staff       (20)        1 2023-06-19 08:31:08.000000 upload_manager-1.1.0/upload_manager.egg-info/dependency_links.txt
--rw-r--r--   0 dharmesh   (502) staff       (20)       67 2023-06-19 08:31:08.000000 upload_manager-1.1.0/upload_manager.egg-info/requires.txt
--rw-r--r--   0 dharmesh   (502) staff       (20)       21 2023-06-19 08:31:08.000000 upload_manager-1.1.0/upload_manager.egg-info/top_level.txt
+drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2024-04-01 12:23:33.000000 upload_manager-1.1.1/
+-rw-r--r--   0 dharmesh   (502) staff       (20)     1144 2021-02-10 09:04:07.000000 upload_manager-1.1.1/LICENSE.md
+-rw-r--r--   0 dharmesh   (502) staff       (20)      114 2021-03-02 13:09:30.000000 upload_manager-1.1.1/MANIFEST.in
+-rw-r--r--   0 dharmesh   (502) staff       (20)     2703 2024-04-01 12:23:33.000000 upload_manager-1.1.1/PKG-INFO
+-rw-r--r--   0 dharmesh   (502) staff       (20)     2132 2021-03-02 13:17:30.000000 upload_manager-1.1.1/README.md
+drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2024-04-01 12:23:33.000000 upload_manager-1.1.1/images/
+-rw-r--r--   0 dharmesh   (502) staff       (20)   200603 2021-03-02 12:37:59.000000 upload_manager-1.1.1/images/dashboard.png
+-rw-rw-r--   0 dharmesh   (502) staff       (20)       67 2021-02-10 13:25:58.000000 upload_manager-1.1.1/requirements.txt
+-rw-r--r--   0 dharmesh   (502) staff       (20)       38 2024-04-01 12:23:33.000000 upload_manager-1.1.1/setup.cfg
+-rw-r--r--   0 dharmesh   (502) staff       (20)      981 2024-04-01 12:21:32.000000 upload_manager-1.1.1/setup.py
+drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2024-04-01 12:23:33.000000 upload_manager-1.1.1/tests/
+-rw-r--r--   0 dharmesh   (502) staff       (20)        0 2021-02-10 06:21:51.000000 upload_manager-1.1.1/tests/__init__.py
+-rw-r--r--   0 dharmesh   (502) staff       (20)      621 2021-02-10 13:58:22.000000 upload_manager-1.1.1/tests/test_s3.py
+drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2024-04-01 12:23:33.000000 upload_manager-1.1.1/upload_manager/
+-rw-rw-r--   0 dharmesh   (502) staff       (20)        0 2020-08-07 09:11:53.000000 upload_manager-1.1.1/upload_manager/__init__.py
+-rw-r--r--   0 dharmesh   (502) staff       (20)     1196 2022-11-04 06:16:29.000000 upload_manager-1.1.1/upload_manager/admin.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)      138 2021-03-02 12:35:59.000000 upload_manager-1.1.1/upload_manager/apps.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)      626 2020-08-07 09:11:53.000000 upload_manager-1.1.1/upload_manager/file_operator.py
+drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2024-04-01 12:23:33.000000 upload_manager-1.1.1/upload_manager/migrations/
+-rw-rw-r--   0 dharmesh   (502) staff       (20)     1477 2020-08-07 09:11:53.000000 upload_manager-1.1.1/upload_manager/migrations/0001_initial.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)        0 2020-08-07 09:11:53.000000 upload_manager-1.1.1/upload_manager/migrations/__init__.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)     1527 2020-08-07 09:11:53.000000 upload_manager-1.1.1/upload_manager/models.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)     4503 2021-02-01 17:23:37.000000 upload_manager-1.1.1/upload_manager/s3.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)     6052 2021-03-01 11:28:31.000000 upload_manager-1.1.1/upload_manager/service.py
+-rw-r--r--   0 dharmesh   (502) staff       (20)      169 2023-06-19 07:21:57.000000 upload_manager-1.1.1/upload_manager/urls.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)      445 2020-08-07 09:11:53.000000 upload_manager-1.1.1/upload_manager/utils.py
+-rw-r--r--   0 dharmesh   (502) staff       (20)     1793 2024-04-01 12:09:00.000000 upload_manager-1.1.1/upload_manager/views.py
+drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2024-04-01 12:23:33.000000 upload_manager-1.1.1/upload_manager.egg-info/
+-rw-r--r--   0 dharmesh   (502) staff       (20)     2703 2024-04-01 12:23:33.000000 upload_manager-1.1.1/upload_manager.egg-info/PKG-INFO
+-rw-r--r--   0 dharmesh   (502) staff       (20)      632 2024-04-01 12:23:33.000000 upload_manager-1.1.1/upload_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 dharmesh   (502) staff       (20)        1 2024-04-01 12:23:33.000000 upload_manager-1.1.1/upload_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 dharmesh   (502) staff       (20)       67 2024-04-01 12:23:33.000000 upload_manager-1.1.1/upload_manager.egg-info/requires.txt
+-rw-r--r--   0 dharmesh   (502) staff       (20)       21 2024-04-01 12:23:33.000000 upload_manager-1.1.1/upload_manager.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `upload_manager-1.1.0/LICENSE.md` & `upload_manager-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `upload_manager-1.1.0/PKG-INFO` & `upload_manager-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upload_manager
-Version: 1.1.0
+Version: 1.1.1
 Summary: Upload manager
 Home-page: https://github.com/Bigbasket/bbuploadmanager
 Author: bb-tech
 Author-email: asodiyadharmesh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `upload_manager-1.1.0/README.md` & `upload_manager-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `upload_manager-1.1.0/images/dashboard.png` & `upload_manager-1.1.1/images/dashboard.png`

 * *Files identical despite different names*

### Comparing `upload_manager-1.1.0/setup.py` & `upload_manager-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open('requirements.txt') as infile:
     requirements = infile.read().splitlines()
 
 setuptools.setup(
     name="upload_manager",
-    version="1.1.0",
+    version="1.1.1",
     author="bb-tech",
     author_email="asodiyadharmesh@gmail.com",
     description="Upload manager",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/Bigbasket/bbuploadmanager",
     include_package_data=True,
```

### Comparing `upload_manager-1.1.0/tests/test_s3.py` & `upload_manager-1.1.1/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.1.0/upload_manager/admin.py` & `upload_manager-1.1.1/upload_manager/admin.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.1.0/upload_manager/file_operator.py` & `upload_manager-1.1.1/upload_manager/file_operator.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.1.0/upload_manager/migrations/0001_initial.py` & `upload_manager-1.1.1/upload_manager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.1.0/upload_manager/models.py` & `upload_manager-1.1.1/upload_manager/models.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.1.0/upload_manager/s3.py` & `upload_manager-1.1.1/upload_manager/s3.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.1.0/upload_manager/service.py` & `upload_manager-1.1.1/upload_manager/service.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.1.0/upload_manager/views.py` & `upload_manager-1.1.1/upload_manager/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     body = request.body.decode('utf-8')
     body_json = json.loads(body)
 
     s3_download_path = body_json.get('s3_download_path')  
     status = body_json['status']
 
     if not status or status != UploadManager.COMPLETED and status != UploadManager.IN_PROCESS \
-            and status != UploadManager.FAILED:
+            and status != UploadManager.FAILED and status != UploadManager.VALIDATION_FAILED:
         logger.warn("Invalid status %s received for upload manager id %s", status, upload_id)
         return HttpResponseBadRequest("Invalid status")
     try:
         upload.status = status
         if s3_download_path:
             upload.s3_download_path = s3_download_path
         upload.save()
```

### Comparing `upload_manager-1.1.0/upload_manager.egg-info/PKG-INFO` & `upload_manager-1.1.1/upload_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upload-manager
-Version: 1.1.0
+Version: 1.1.1
 Summary: Upload manager
 Home-page: https://github.com/Bigbasket/bbuploadmanager
 Author: bb-tech
 Author-email: asodiyadharmesh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `upload_manager-1.1.0/upload_manager.egg-info/SOURCES.txt` & `upload_manager-1.1.1/upload_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*


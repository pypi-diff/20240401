# Comparing `tmp/secsend-1.0.0rc0.tar.gz` & `tmp/secsend-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secsend-1.0.0rc0.tar", last modified: Tue Sep  6 07:56:04 2022, max compression
+gzip compressed data, was "secsend-1.1.0.tar", last modified: Mon Apr  1 13:46:47 2024, max compression
```

## Comparing `secsend-1.0.0rc0.tar` & `secsend-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 07:56:04.946637 secsend-1.0.0rc0/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-09-06 07:56:04.946637 secsend-1.0.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6393 2022-09-06 07:55:50.000000 secsend-1.0.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 07:56:04.942637 secsend-1.0.0rc0/bin/
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-09-06 07:55:50.000000 secsend-1.0.0rc0/bin/secadmin
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-09-06 07:55:50.000000 secsend-1.0.0rc0/bin/secdownload
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-09-06 07:55:50.000000 secsend-1.0.0rc0/bin/secupload
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 07:56:04.942637 secsend-1.0.0rc0/secsend/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-06 07:55:50.000000 secsend-1.0.0rc0/secsend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-09-06 07:55:50.000000 secsend-1.0.0rc0/secsend/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-09-06 07:55:50.000000 secsend-1.0.0rc0/secsend/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     5100 2022-09-06 07:55:50.000000 secsend-1.0.0rc0/secsend/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3003 2022-09-06 07:55:50.000000 secsend-1.0.0rc0/secsend/crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-09-06 07:55:50.000000 secsend-1.0.0rc0/secsend/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     6953 2022-09-06 07:55:50.000000 secsend-1.0.0rc0/secsend/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-09-06 07:55:50.000000 secsend-1.0.0rc0/secsend/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 07:56:04.946637 secsend-1.0.0rc0/secsend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-09-06 07:56:04.000000 secsend-1.0.0rc0/secsend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-09-06 07:56:04.000000 secsend-1.0.0rc0/secsend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 07:56:04.000000 secsend-1.0.0rc0/secsend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-06 07:56:04.000000 secsend-1.0.0rc0/secsend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-06 07:56:04.000000 secsend-1.0.0rc0/secsend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 07:56:04.946637 secsend-1.0.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-09-06 07:55:50.000000 secsend-1.0.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:46:47.829955 secsend-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-01 13:46:47.829955 secsend-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-01 13:46:38.000000 secsend-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:46:47.829955 secsend-1.1.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-01 13:46:38.000000 secsend-1.1.0/bin/secadmin
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-01 13:46:38.000000 secsend-1.1.0/bin/secdownload
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-01 13:46:38.000000 secsend-1.1.0/bin/secupload
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:46:47.829955 secsend-1.1.0/secsend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:46:38.000000 secsend-1.1.0/secsend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-01 13:46:38.000000 secsend-1.1.0/secsend/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-01 13:46:38.000000 secsend-1.1.0/secsend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-01 13:46:38.000000 secsend-1.1.0/secsend/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-01 13:46:38.000000 secsend-1.1.0/secsend/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-01 13:46:38.000000 secsend-1.1.0/secsend/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-01 13:46:38.000000 secsend-1.1.0/secsend/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-01 13:46:38.000000 secsend-1.1.0/secsend/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:46:47.829955 secsend-1.1.0/secsend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-01 13:46:47.000000 secsend-1.1.0/secsend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-01 13:46:47.000000 secsend-1.1.0/secsend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:46:47.000000 secsend-1.1.0/secsend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 13:46:47.000000 secsend-1.1.0/secsend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 13:46:47.000000 secsend-1.1.0/secsend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:46:47.829955 secsend-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-01 13:46:38.000000 secsend-1.1.0/setup.py
```

### Comparing `secsend-1.0.0rc0/README.md` & `secsend-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 Copy `docker.env.example` to `docker.env`, and modify its content to configure
 secsend (e.g. file size limit).
 
 Then, run secsend with docker:
 
 ```
-# docker run --env-file docker.env -p 8000:80 -v /path/to/data/storage:/data secsend:v1.0.0rc0
+# docker run --env-file docker.env -p 8000:80 -v /path/to/data/storage:/data aguinet/secsend:v1.1.0
 ```
 
 `/path/to/data/storage` will contain the uploaded files and associated metadata.
 
 If you have changed `SECSEND_LISTEN_PORT` in `docker.env`, change the `-p`
 option accordingly.
```

### Comparing `secsend-1.0.0rc0/bin/secadmin` & `secsend-1.1.0/bin/secadmin`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     actions = parser.add_mutually_exclusive_group(required=True)
     actions.add_argument("-d", action='store_true', dest='delete', help="Delete (incomplete) file")
     parser.add_argument("dest", type=str, help="Admin URL of the uploaded file")
     args = parser.parse_args()
 
     url = DownloadURL.from_url(args.dest)
     if not isinstance(url.id, RootID):
-        print("Error: please use the Admin URL to resume the upload", file=sys.stderr)
+        print("Error: please use the Admin URL to delete the file", file=sys.stderr)
         sys.exit(1)
 
     client = ClientAPI(requests.Session(), url.server)
     if args.delete:
         client.delete(url.id)
         print("File deleted with success")
```

### Comparing `secsend-1.0.0rc0/bin/secdownload` & `secsend-1.1.0/bin/secdownload`

 * *Files identical despite different names*

### Comparing `secsend-1.0.0rc0/bin/secupload` & `secsend-1.1.0/bin/secupload`

 * *Files identical despite different names*

### Comparing `secsend-1.0.0rc0/secsend/cli.py` & `secsend-1.1.0/secsend/cli.py`

 * *Files identical despite different names*

### Comparing `secsend-1.0.0rc0/secsend/client.py` & `secsend-1.1.0/secsend/client.py`

 * *Files identical despite different names*

### Comparing `secsend-1.0.0rc0/secsend/crypto.py` & `secsend-1.1.0/secsend/crypto.py`

 * *Files identical despite different names*

### Comparing `secsend-1.0.0rc0/secsend/metadata.py` & `secsend-1.1.0/secsend/metadata.py`

 * *Files identical despite different names*

### Comparing `secsend-1.0.0rc0/secsend/stream.py` & `secsend-1.1.0/secsend/stream.py`

 * *Files identical despite different names*

### Comparing `secsend-1.0.0rc0/secsend/utils.py` & `secsend-1.1.0/secsend/utils.py`

 * *Files identical despite different names*

### Comparing `secsend-1.0.0rc0/setup.py` & `secsend-1.1.0/setup.py`

 * *Files identical despite different names*


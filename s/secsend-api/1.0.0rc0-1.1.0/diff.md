# Comparing `tmp/secsend_api-1.0.0rc0.tar.gz` & `tmp/secsend_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secsend_api-1.0.0rc0.tar", last modified: Tue Sep  6 07:56:05 2022, max compression
+gzip compressed data, was "secsend_api-1.1.0.tar", last modified: Mon Apr  1 13:46:48 2024, max compression
```

## Comparing `secsend_api-1.0.0rc0.tar` & `secsend_api-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 07:56:05.322643 secsend_api-1.0.0rc0/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-09-06 07:56:05.322643 secsend_api-1.0.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6393 2022-09-06 07:55:50.000000 secsend_api-1.0.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 07:56:05.322643 secsend_api-1.0.0rc0/secsend_api/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-06 07:55:50.000000 secsend_api-1.0.0rc0/secsend_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-09-06 07:55:50.000000 secsend_api-1.0.0rc0/secsend_api/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8540 2022-09-06 07:55:50.000000 secsend_api-1.0.0rc0/secsend_api/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-09-06 07:55:50.000000 secsend_api-1.0.0rc0/secsend_api/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     4704 2022-09-06 07:55:50.000000 secsend_api-1.0.0rc0/secsend_api/backend_files.py
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-09-06 07:55:50.000000 secsend_api-1.0.0rc0/secsend_api/cors.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-09-06 07:55:50.000000 secsend_api-1.0.0rc0/secsend_api/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-09-06 07:55:50.000000 secsend_api-1.0.0rc0/secsend_api/options.py
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-06 07:55:50.000000 secsend_api-1.0.0rc0/secsend_api/prod.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-09-06 07:55:50.000000 secsend_api-1.0.0rc0/secsend_api/timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 07:56:05.322643 secsend_api-1.0.0rc0/secsend_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-09-06 07:56:05.000000 secsend_api-1.0.0rc0/secsend_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-06 07:56:05.000000 secsend_api-1.0.0rc0/secsend_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 07:56:05.000000 secsend_api-1.0.0rc0/secsend_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-06 07:56:05.000000 secsend_api-1.0.0rc0/secsend_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-06 07:56:05.000000 secsend_api-1.0.0rc0/secsend_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 07:56:05.322643 secsend_api-1.0.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-09-06 07:55:50.000000 secsend_api-1.0.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:46:48.185955 secsend_api-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-01 13:46:48.185955 secsend_api-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-01 13:46:38.000000 secsend_api-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:46:48.181955 secsend_api-1.1.0/secsend_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 13:46:38.000000 secsend_api-1.1.0/secsend_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-01 13:46:38.000000 secsend_api-1.1.0/secsend_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-01 13:46:38.000000 secsend_api-1.1.0/secsend_api/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-01 13:46:38.000000 secsend_api-1.1.0/secsend_api/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-01 13:46:38.000000 secsend_api-1.1.0/secsend_api/backend_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-01 13:46:38.000000 secsend_api-1.1.0/secsend_api/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-01 13:46:38.000000 secsend_api-1.1.0/secsend_api/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-01 13:46:38.000000 secsend_api-1.1.0/secsend_api/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 13:46:38.000000 secsend_api-1.1.0/secsend_api/prod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-01 13:46:38.000000 secsend_api-1.1.0/secsend_api/timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:46:48.185955 secsend_api-1.1.0/secsend_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-01 13:46:48.000000 secsend_api-1.1.0/secsend_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-01 13:46:48.000000 secsend_api-1.1.0/secsend_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:46:48.000000 secsend_api-1.1.0/secsend_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-01 13:46:48.000000 secsend_api-1.1.0/secsend_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 13:46:48.000000 secsend_api-1.1.0/secsend_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:46:48.185955 secsend_api-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-01 13:46:38.000000 secsend_api-1.1.0/setup.py
```

### Comparing `secsend_api-1.0.0rc0/README.md` & `secsend_api-1.1.0/README.md`

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

### Comparing `secsend_api-1.0.0rc0/secsend_api/app.py` & `secsend_api-1.1.0/secsend_api/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             "Content-Length": length
         },
         _range=_range,
         chunk_size=1024*1024*10,
     )
 
 @bp.post("/delete/<id_>")
-async def upload_finish(request, id_):
+async def delete_id(request, id_):
     rid = RootID.from_str(id_)
     fid = rid.file_id()
     f = get_backend(request).open(fid)
     f.check_validity()
     f.delete()
     return response.json({})
 
@@ -204,17 +204,17 @@
             import secsend_webapp
             html_root = secsend_webapp.root
         except ImportError:
             html_root = None
 
     if html_root is not None:
         app.ctx.html_root = html_root
-        app.static("/", os.path.join(html_root, "index.html"))
-        app.static("/", html_root)
-        app.static("/dl", os.path.join(html_root, "dl.html"))
+        app.static("/", html_root, name="webapp")
+        app.static("/", os.path.join(html_root, "index.html"), name="webapp_index")
+        app.static("/dl", os.path.join(html_root, "dl.html"), name="dl")
     else:
         print("Warning: no html_root has been specified, sanic won't serve the webapp", file=sys.stderr)
 
     # Set backend
     try:
         backend_files_root = app.config.BACKEND_FILES_ROOT
     except AttributeError:
```

### Comparing `secsend_api-1.0.0rc0/secsend_api/backend.py` & `secsend_api-1.1.0/secsend_api/backend.py`

 * *Files identical despite different names*

### Comparing `secsend_api-1.0.0rc0/secsend_api/backend_files.py` & `secsend_api-1.1.0/secsend_api/backend_files.py`

 * *Files identical despite different names*

### Comparing `secsend_api-1.0.0rc0/secsend_api/cors.py` & `secsend_api-1.1.0/secsend_api/cors.py`

 * *Files identical despite different names*

### Comparing `secsend_api-1.0.0rc0/secsend_api/metadata.py` & `secsend_api-1.1.0/secsend_api/metadata.py`

 * *Files identical despite different names*

### Comparing `secsend_api-1.0.0rc0/secsend_api/options.py` & `secsend_api-1.1.0/secsend_api/options.py`

 * *Files identical despite different names*

### Comparing `secsend_api-1.0.0rc0/setup.py` & `secsend_api-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,15 +12,16 @@
       url=about['__url__'],
       author=about['__author__'],
       author_email=about['__author_email__'],
       license=about['__license__'],
       packages=['secsend_api'],
       install_requires=[
           'jsonschema==4.15.*',
-          'sanic==21.12.*',
+          'sanic==23.12.1'
       ],
       extras_require={
           'dev': [
-              'sanic-testing==0.8.3',
+              'sanic-testing==23.12.0',
+              'pytest_asyncio==0.23.6'
           ],
       }
 )
```


# Comparing `tmp/esrt-1.21.0.tar.gz` & `tmp/esrt-1.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esrt-1.21.0.tar", last modified: Sat Mar 30 19:38:44 2024, max compression
+gzip compressed data, was "esrt-1.22.0.tar", last modified: Mon Apr  1 14:30:18 2024, max compression
```

## Comparing `esrt-1.21.0.tar` & `esrt-1.22.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:38:44.240269 esrt-1.21.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-03-30 19:38:44.240269 esrt-1.21.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-03-30 19:38:28.000000 esrt-1.21.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-03-30 19:38:28.000000 esrt-1.21.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 19:38:44.240269 esrt-1.21.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:38:44.236269 esrt-1.21.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:38:44.236269 esrt-1.21.0/src/esrt/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-30 19:38:28.000000 esrt-1.21.0/src/esrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-03-30 19:38:28.000000 esrt-1.21.0/src/esrt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-30 19:38:28.000000 esrt-1.21.0/src/esrt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-30 19:38:28.000000 esrt-1.21.0/src/esrt/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-30 19:38:28.000000 esrt-1.21.0/src/esrt/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-30 19:38:28.000000 esrt-1.21.0/src/esrt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:38:44.240269 esrt-1.21.0/src/esrt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-03-30 19:38:44.000000 esrt-1.21.0/src/esrt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-30 19:38:44.000000 esrt-1.21.0/src/esrt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 19:38:44.000000 esrt-1.21.0/src/esrt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-30 19:38:44.000000 esrt-1.21.0/src/esrt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-30 19:38:44.000000 esrt-1.21.0/src/esrt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-30 19:38:44.000000 esrt-1.21.0/src/esrt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:30:18.353363 esrt-1.22.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-04-01 14:30:18.353363 esrt-1.22.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-04-01 14:30:01.000000 esrt-1.22.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-01 14:30:01.000000 esrt-1.22.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:30:18.353363 esrt-1.22.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:30:18.349363 esrt-1.22.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:30:18.353363 esrt-1.22.0/src/esrt/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-01 14:30:01.000000 esrt-1.22.0/src/esrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-04-01 14:30:01.000000 esrt-1.22.0/src/esrt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-01 14:30:01.000000 esrt-1.22.0/src/esrt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-01 14:30:01.000000 esrt-1.22.0/src/esrt/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-01 14:30:01.000000 esrt-1.22.0/src/esrt/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-01 14:30:01.000000 esrt-1.22.0/src/esrt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:30:18.353363 esrt-1.22.0/src/esrt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-04-01 14:30:18.000000 esrt-1.22.0/src/esrt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-01 14:30:18.000000 esrt-1.22.0/src/esrt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:30:18.000000 esrt-1.22.0/src/esrt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 14:30:18.000000 esrt-1.22.0/src/esrt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-01 14:30:18.000000 esrt-1.22.0/src/esrt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 14:30:18.000000 esrt-1.22.0/src/esrt.egg-info/top_level.txt
```

### Comparing `esrt-1.21.0/PKG-INFO` & `esrt-1.22.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esrt
-Version: 1.21.0
+Version: 1.22.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: elasticsearch==6.8.2
 Requires-Dist: typer-slim[standard]>=0.12.0
 Requires-Dist: uvicorn>=0.2.14
 
 # esrt - Elasticsearch Request Tool
```

### Comparing `esrt-1.21.0/README.md` & `esrt-1.22.0/README.md`

 * *Files identical despite different names*

### Comparing `esrt-1.21.0/pyproject.toml` & `esrt-1.22.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "esrt"
-version = "1.21.0"
+version = "1.22.0"
 requires-python = ">=3.9"
 readme = "README.md"
 dependencies = [
     "elasticsearch==6.8.2",
     "typer-slim[standard]>=0.12.0",
     # uvicorn.importer.import_from_string
     "uvicorn>=0.2.14",
```

### Comparing `esrt-1.21.0/src/esrt/__main__.py` & `esrt-1.22.0/src/esrt/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,18 @@
 _foutput_annotated = t.Annotated[
     typer.FileTextWrite, typer.Option('-o', '--output', metavar='FILE', help='Output file')
 ]
 #
 _doc_type_annotated = t.Annotated[
     t.Optional[str], typer.Option('-t', '--type', metavar='DOC_TYPE', help='Document type')
 ]
+#
+_chunk_size_annotated = t.Annotated[
+    int, typer.Option('-c', '--chunk-size', envvar='ESRT_TRANSMIT_CHUNK_SIZE')
+]
 
 
 @app.command(name='e', no_args_is_help=True, short_help=Help.e_search)
 @app.command(name='search', no_args_is_help=True, short_help=Help.e_search)
 def search(
     host: _host_annotated,
     finput_body: t.Annotated[t.Optional[typer.FileText], _finput_annotation] = None,
@@ -230,22 +234,23 @@
             '--handler',
             parser=import_from_string,
             help='A callable handle actions. e.g. --handler esrt:DocHandler',
         ),
     ] = t.cast(t.Callable[[t.Iterable[str]], t.Iterable[str]], 'esrt:DocHandler'),
     doc_type: _doc_type_annotated = None,
     #
-    chunk_size: t.Annotated[int, typer.Option('-c', '--chunk-size')] = 500,
+    chunk_size: _chunk_size_annotated = 500,
     max_chunk_bytes: t.Annotated[int, typer.Option('--max-chunk-bytes')] = 100 * 1024 * 1024,
     raise_on_error: t.Annotated[bool, typer.Option(' /--no-raise-on-error')] = True,
     raise_on_exception: t.Annotated[bool, typer.Option(' /--no-raise-on-exception')] = True,
     max_retries: t.Annotated[int, typer.Option('--max-retries')] = 3,
     initial_backoff: t.Annotated[int, typer.Option('--initial-backoff')] = 2,
     max_backoff: t.Annotated[int, typer.Option('--max-backoff')] = 600,
 ):
+    return print(f'{chunk_size = }')
     client = es.Client(host=host)
     with redirect_stdout(sys.stderr):
         print(client)
         print('waiting for seconds to start', end=' ', flush=True)
         for i in range(5, -1, -1):
             print(i, end=' ', flush=True)
             time.sleep(1)
```

### Comparing `esrt-1.21.0/src/esrt/handlers.py` & `esrt-1.22.0/src/esrt/handlers.py`

 * *Files identical despite different names*

### Comparing `esrt-1.21.0/src/esrt/utils.py` & `esrt-1.22.0/src/esrt/utils.py`

 * *Files identical despite different names*

### Comparing `esrt-1.21.0/src/esrt.egg-info/PKG-INFO` & `esrt-1.22.0/src/esrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esrt
-Version: 1.21.0
+Version: 1.22.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: elasticsearch==6.8.2
 Requires-Dist: typer-slim[standard]>=0.12.0
 Requires-Dist: uvicorn>=0.2.14
 
 # esrt - Elasticsearch Request Tool
```


# Comparing `tmp/dstool-0.0.5.tar.gz` & `tmp/dstool-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dstool-0.0.5.tar", last modified: Thu Aug 11 18:25:05 2022, max compression
+gzip compressed data, was "dstool-0.1.0.tar", last modified: Mon Apr  1 14:52:28 2024, max compression
```

## Comparing `dstool-0.0.5.tar` & `dstool-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,36 @@
-drwxrwxr-x   0 xiayao    (1000) xiayao    (1000)        0 2022-08-11 18:25:05.257699 dstool-0.0.5/
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)      827 2022-08-11 18:25:05.257699 dstool-0.0.5/PKG-INFO
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)        0 2022-08-11 17:55:10.000000 dstool-0.0.5/README.md
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)       85 2022-08-11 17:55:10.000000 dstool-0.0.5/pyproject.toml
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)       38 2022-08-11 18:25:05.257699 dstool-0.0.5/setup.cfg
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)     1182 2022-08-11 18:24:52.000000 dstool-0.0.5/setup.py
-drwxrwxr-x   0 xiayao    (1000) xiayao    (1000)        0 2022-08-11 18:25:05.257699 dstool-0.0.5/src/
-drwxrwxr-x   0 xiayao    (1000) xiayao    (1000)        0 2022-08-11 18:25:05.257699 dstool-0.0.5/src/dstool/
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)        0 2022-08-11 17:55:10.000000 dstool-0.0.5/src/dstool/__init__.py
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)      254 2022-08-11 17:55:10.000000 dstool-0.0.5/src/dstool/class_utils.py
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)     1512 2022-08-11 18:22:42.000000 dstool-0.0.5/src/dstool/database.py
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)     1778 2022-08-11 17:55:10.000000 dstool-0.0.5/src/dstool/debugger.py
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)     1190 2022-08-11 17:55:10.000000 dstool-0.0.5/src/dstool/distance.py
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)     1201 2022-08-11 17:55:42.000000 dstool-0.0.5/src/dstool/measure.py
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)      686 2022-08-11 17:55:47.000000 dstool-0.0.5/src/dstool/parallel.py
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)     1009 2022-08-11 17:55:51.000000 dstool-0.0.5/src/dstool/storage.py
-drwxrwxr-x   0 xiayao    (1000) xiayao    (1000)        0 2022-08-11 18:25:05.257699 dstool-0.0.5/src/dstool.egg-info/
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)      827 2022-08-11 18:25:05.000000 dstool-0.0.5/src/dstool.egg-info/PKG-INFO
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)      387 2022-08-11 18:25:05.000000 dstool-0.0.5/src/dstool.egg-info/SOURCES.txt
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)        1 2022-08-11 18:25:05.000000 dstool-0.0.5/src/dstool.egg-info/dependency_links.txt
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)       26 2022-08-11 18:25:05.000000 dstool-0.0.5/src/dstool.egg-info/requires.txt
--rw-rw-r--   0 xiayao    (1000) xiayao    (1000)        7 2022-08-11 18:25:05.000000 dstool-0.0.5/src/dstool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.112434 dstool-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 14:52:15.000000 dstool-0.1.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-01 14:52:15.000000 dstool-0.1.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 14:52:15.000000 dstool-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-01 14:52:15.000000 dstool-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-01 14:52:28.112434 dstool-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-01 14:52:15.000000 dstool-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.104434 dstool-0.1.0/dstool/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.108434 dstool-0.1.0/dstool/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/decorators/class_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/decorators/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/decorators/measure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.108434 dstool-0.1.0/dstool/parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/parallel/parallel_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.108434 dstool-0.1.0/dstool/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-01 14:52:15.000000 dstool-0.1.0/dstool/plot/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.108434 dstool-0.1.0/dstool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-01 14:52:28.000000 dstool-0.1.0/dstool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-01 14:52:28.000000 dstool-0.1.0/dstool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:52:28.000000 dstool-0.1.0/dstool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 14:52:28.000000 dstool-0.1.0/dstool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-01 14:52:28.000000 dstool-0.1.0/dstool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 14:52:28.000000 dstool-0.1.0/dstool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:52:28.112434 dstool-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-01 14:52:15.000000 dstool-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:28.108434 dstool-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:15.000000 dstool-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-01 14:52:15.000000 dstool-0.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 14:52:15.000000 dstool-0.1.0/tests/test_base.py
```

### Comparing `dstool-0.0.5/src/dstool/debugger.py` & `dstool-0.1.0/dstool/decorators/debugger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from sys import settrace
 from typing import Callable
 
 
-def stacktrace(func=None, exclude_files=['conda', 'miniconda3', 'Anaconda']):
+def stacktrace(func=None, exclude_files=["conda", "miniconda3", "Anaconda"]):
 
     def tracer_func(frame, event, arg):
         co = frame.f_code
         func_name = co.co_name
         caller_filename = frame.f_back.f_code.co_filename
-        if func_name == 'write':
+        if func_name == "write":
             return  # ignore write() calls from print statements
         for file in exclude_files:
             if file in caller_filename:
                 return  # ignore in ipython notebooks
         args = str(
-            tuple([frame.f_locals[arg] for arg in frame.f_code.co_varnames]))
-        if args.endswith(',)'):
-            args = args[:-2] + ')'
-        if event == 'call':
-            print(f'-> Executing: {func_name}{args}')
+            tuple([frame.f_locals[arg] for arg in frame.f_code.co_varnames])
+        )
+        if args.endswith(",)"):
+            args = args[:-2] + ")"
+        if event == "call":
+            print(f"-> Executing: {func_name}{args}")
             return tracer_func
-        elif event == 'return':
-            print(f'-> Returning: {func_name}{args} -> {repr(arg)}')
+        elif event == "return":
+            print(f"-> Returning: {func_name}{args} -> {repr(arg)}")
         return
 
     def decorator(func: Callable):
 
         def inner(*args, **kwargs):
             settrace(tracer_func)
             func(*args, **kwargs)
@@ -41,16 +42,16 @@
         return decorator(func)
 
 
 def traceclass(cls: type):
 
     def make_traced(cls: type, method_name: str, method: Callable):
         def traced_method(*args, **kwargs):
-            print(f'--> Executing: {cls.__name__}::{method_name}()')
+            print(f"--> Executing: {cls.__name__}::{method_name}()")
             return method(*args, **kwargs)
 
         return traced_method
 
     for name in cls.__dict__.keys():
-        if callable(getattr(cls, name)) and name != '__class__':
+        if callable(getattr(cls, name)) and name != "__class__":
             setattr(cls, name, make_traced(cls, name, getattr(cls, name)))
     return cls
```

### Comparing `dstool-0.0.5/src/dstool/measure.py` & `dstool-0.1.0/dstool/decorators/measure.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,46 @@
+import contextlib
 from timeit import default_timer
 from typing import Callable
-import contextlib
+
 import joblib
 
+
 @contextlib.contextmanager
 def tqdm_joblib(tqdm_object):
-    """Context manager to patch joblib to report into tqdm progress bar given as argument"""
+    """Context manager to patch joblib to report
+    into tqdm progress bar given as argument"""
+
     class TqdmBatchCompletionCallback(joblib.parallel.BatchCompletionCallBack):
         def __call__(self, *args, **kwargs):
             tqdm_object.update(n=self.batch_size)
             return super().__call__(*args, **kwargs)
 
     old_batch_callback = joblib.parallel.BatchCompletionCallBack
     joblib.parallel.BatchCompletionCallBack = TqdmBatchCompletionCallback
     try:
         yield tqdm_object
     finally:
         joblib.parallel.BatchCompletionCallBack = old_batch_callback
         tqdm_object.close()
 
+
 def measure(func: Callable):
 
     def inner(*args, **kwargs):
         start = default_timer()
         func(*args, **kwargs)
         elapsed_sec = default_timer - start
-        print(f'Elapsed: {elapsed_sec:.3f} secs')
+        print(f"Elapsed: {elapsed_sec:.3f} secs")
 
     return inner
 
+
 def repeat(n: int = 1):
     def decorator(func: Callable):
         def inner(*args, **kwargs):
             for _ in range(n):
                 func(*args, **kwargs)
+
         return inner
+
     return decorator
```

### Comparing `dstool-0.0.5/src/dstool/parallel.py` & `dstool-0.1.0/dstool/parallel/parallel_func.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from multiprocessing import cpu_count
 from typing import Callable
 
 from joblib import Parallel, delayed
 
-def parallel(func=None,
-             args=(),
-             merge_func=lambda x: x,
-             parallelism=cpu_count()):
+
+def parallel(
+    func=None, args=(), merge_func=lambda x: x, parallelism=cpu_count()
+):
 
     def decorator(func: Callable):
 
         def inner(*args, **kwargs):
             results = Parallel(n_jobs=parallelism)(
-                delayed(func)(*args, **kwargs) for i in range(parallelism))
+                delayed(func)(*args, **kwargs) for i in range(parallelism)
+            )
             return merge_func(results)
 
         return inner
 
     if func is None:
         # decorator was used like @parallel(...)
         return decorator
```


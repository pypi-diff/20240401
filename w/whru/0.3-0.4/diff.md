# Comparing `tmp/whru-0.3.tar.gz` & `tmp/whru-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whru-0.3.tar", last modified: Mon Apr  1 07:28:04 2024, max compression
+gzip compressed data, was "whru-0.4.tar", last modified: Mon Apr  1 13:48:23 2024, max compression
```

## Comparing `whru-0.3.tar` & `whru-0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 07:28:04.762056 whru-0.3/
--rw-r--r--   0 whr       (1100) whr       (1100)      198 2024-04-01 07:28:04.762056 whru-0.3/PKG-INFO
--rw-rw-r--   0 whr       (1100) whr       (1100)      177 2024-04-01 06:57:20.000000 whru-0.3/README.md
--rw-rw-r--   0 whr       (1100) whr       (1100)       38 2024-04-01 07:28:04.762056 whru-0.3/setup.cfg
--rw-rw-r--   0 whr       (1100) whr       (1100)      315 2024-04-01 07:26:34.000000 whru-0.3/setup.py
-drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 07:28:04.758056 whru-0.3/tests/
--rw-rw-r--   0 whr       (1100) whr       (1100)       89 2024-04-01 01:39:12.000000 whru-0.3/tests/test_log.py
--rw-rw-r--   0 whr       (1100) whr       (1100)      347 2024-04-01 02:47:58.000000 whru-0.3/tests/test_tensorboard_log.py
--rw-rw-r--   0 whr       (1100) whr       (1100)      317 2024-04-01 02:07:20.000000 whru-0.3/tests/test_utils.py
-drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 07:28:04.758056 whru-0.3/whru/
--rw-rw-r--   0 whr       (1100) whr       (1100)       81 2024-04-01 07:20:09.000000 whru-0.3/whru/__init__.py
-drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 07:28:04.758056 whru-0.3/whru/log/
--rw-rw-r--   0 whr       (1100) whr       (1100)       18 2024-04-01 01:39:08.000000 whru-0.3/whru/log/__init__.py
--rw-rw-r--   0 whr       (1100) whr       (1100)     1045 2024-04-01 01:40:03.000000 whru-0.3/whru/log/log.py
-drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 07:28:04.758056 whru-0.3/whru/tensorboard/
--rw-rw-r--   0 whr       (1100) whr       (1100)       38 2024-04-01 02:02:46.000000 whru-0.3/whru/tensorboard/__init__.py
--rw-rw-r--   0 whr       (1100) whr       (1100)      144 2024-04-01 01:56:19.000000 whru-0.3/whru/tensorboard/log.py
--rw-rw-r--   0 whr       (1100) whr       (1100)      375 2024-03-20 00:39:25.000000 whru-0.3/whru/tensorboard/read.py
-drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 07:28:04.758056 whru-0.3/whru/utils/
--rw-rw-r--   0 whr       (1100) whr       (1100)       20 2024-04-01 01:58:26.000000 whru-0.3/whru/utils/__init__.py
--rw-rw-r--   0 whr       (1100) whr       (1100)        0 2024-04-01 02:44:02.000000 whru-0.3/whru/utils/path.py
--rw-rw-r--   0 whr       (1100) whr       (1100)     1126 2024-03-20 06:27:20.000000 whru-0.3/whru/utils/producer_consumer.py
--rw-rw-r--   0 whr       (1100) whr       (1100)      645 2024-04-01 02:47:07.000000 whru-0.3/whru/utils/utils.py
-drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 07:28:04.758056 whru-0.3/whru.egg-info/
--rw-r--r--   0 whr       (1100) whr       (1100)      198 2024-04-01 07:28:04.000000 whru-0.3/whru.egg-info/PKG-INFO
--rw-rw-r--   0 whr       (1100) whr       (1100)      451 2024-04-01 07:28:04.000000 whru-0.3/whru.egg-info/SOURCES.txt
--rw-rw-r--   0 whr       (1100) whr       (1100)        1 2024-04-01 07:28:04.000000 whru-0.3/whru.egg-info/dependency_links.txt
--rw-rw-r--   0 whr       (1100) whr       (1100)       31 2024-04-01 07:28:04.000000 whru-0.3/whru.egg-info/requires.txt
--rw-rw-r--   0 whr       (1100) whr       (1100)        5 2024-04-01 07:28:04.000000 whru-0.3/whru.egg-info/top_level.txt
+drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 13:48:23.566198 whru-0.4/
+-rw-r--r--   0 whr       (1100) whr       (1100)      198 2024-04-01 13:48:23.566198 whru-0.4/PKG-INFO
+-rw-rw-r--   0 whr       (1100) whr       (1100)      203 2024-04-01 07:39:05.000000 whru-0.4/README.md
+-rw-rw-r--   0 whr       (1100) whr       (1100)       38 2024-04-01 13:48:23.566198 whru-0.4/setup.cfg
+-rw-rw-r--   0 whr       (1100) whr       (1100)      315 2024-04-01 13:47:31.000000 whru-0.4/setup.py
+drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 13:48:23.566198 whru-0.4/tests/
+-rw-rw-r--   0 whr       (1100) whr       (1100)      276 2024-04-01 13:45:27.000000 whru-0.4/tests/test_log.py
+-rw-rw-r--   0 whr       (1100) whr       (1100)      347 2024-04-01 13:42:45.000000 whru-0.4/tests/test_tensorboard_log.py
+-rw-rw-r--   0 whr       (1100) whr       (1100)      317 2024-04-01 02:07:20.000000 whru-0.4/tests/test_utils.py
+drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 13:48:23.566198 whru-0.4/whru/
+-rw-rw-r--   0 whr       (1100) whr       (1100)       83 2024-04-01 13:40:31.000000 whru-0.4/whru/__init__.py
+drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 13:48:23.566198 whru-0.4/whru/log/
+-rw-rw-r--   0 whr       (1100) whr       (1100)       18 2024-04-01 01:39:08.000000 whru-0.4/whru/log/__init__.py
+-rw-rw-r--   0 whr       (1100) whr       (1100)     1297 2024-04-01 13:36:33.000000 whru-0.4/whru/log/log.py
+drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 13:48:23.566198 whru-0.4/whru/tensorboard/
+-rw-rw-r--   0 whr       (1100) whr       (1100)       40 2024-04-01 13:40:18.000000 whru-0.4/whru/tensorboard/__init__.py
+-rw-rw-r--   0 whr       (1100) whr       (1100)      375 2024-03-20 00:39:25.000000 whru-0.4/whru/tensorboard/read.py
+-rw-rw-r--   0 whr       (1100) whr       (1100)      144 2024-04-01 01:56:19.000000 whru-0.4/whru/tensorboard/write.py
+drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 13:48:23.566198 whru-0.4/whru/utils/
+-rw-rw-r--   0 whr       (1100) whr       (1100)       20 2024-04-01 01:58:26.000000 whru-0.4/whru/utils/__init__.py
+-rw-rw-r--   0 whr       (1100) whr       (1100)        0 2024-04-01 02:44:02.000000 whru-0.4/whru/utils/path.py
+-rw-rw-r--   0 whr       (1100) whr       (1100)     1126 2024-03-20 06:27:20.000000 whru-0.4/whru/utils/producer_consumer.py
+-rw-rw-r--   0 whr       (1100) whr       (1100)      645 2024-04-01 02:47:07.000000 whru-0.4/whru/utils/utils.py
+drwxrwxr-x   0 whr       (1100) whr       (1100)        0 2024-04-01 13:48:23.566198 whru-0.4/whru.egg-info/
+-rw-r--r--   0 whr       (1100) whr       (1100)      198 2024-04-01 13:48:23.000000 whru-0.4/whru.egg-info/PKG-INFO
+-rw-rw-r--   0 whr       (1100) whr       (1100)      453 2024-04-01 13:48:23.000000 whru-0.4/whru.egg-info/SOURCES.txt
+-rw-rw-r--   0 whr       (1100) whr       (1100)        1 2024-04-01 13:48:23.000000 whru-0.4/whru.egg-info/dependency_links.txt
+-rw-rw-r--   0 whr       (1100) whr       (1100)       31 2024-04-01 13:48:23.000000 whru-0.4/whru.egg-info/requires.txt
+-rw-rw-r--   0 whr       (1100) whr       (1100)        5 2024-04-01 13:48:23.000000 whru-0.4/whru.egg-info/top_level.txt
```

### Comparing `whru-0.3/whru/log/log.py` & `whru-0.4/whru/log/log.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import logging
 
 
-def get_logger(log_level, name):
+def get_logger(log_level, logger_name, log_file:str=None):
     # 2023-08-02 19:23:44 [0] "/home/whr/fs_gnn/dist_gcn_train.py", line 844, DEBUG: torch.Size([512, 500])
     # note: 如果是多进程，对logging模块的初始化需要在每个进程中都运行一次
     # 并且，logging模块是线程安全的，但并不是进程安全的
     # 如果要保证进程安全，需要将其它进程的消息汇总到一个进程，然后由同一进程中的某些logger（标识进程）来完成
     log_format = f'%(asctime)s %(name)s "%(pathname)s", line %(lineno)d, %(levelname)s: %(message)s\n'
 
     assert (
         log_level in logging._nameToLevel.keys()
     ), f"log_level should be one of {logging._nameToLevel.keys()}"
 
     handler = logging.StreamHandler()
     handler.setLevel(logging._nameToLevel[log_level])
     formatter = logging.Formatter(fmt=log_format)
     handler.setFormatter(formatter)
-    logger = logging.getLogger(name)
+    logger = logging.getLogger(logger_name)
     logger.setLevel(logging._nameToLevel[log_level])
     logger.addHandler(handler)
 
+    if log_file:
+        handler_file = logging.FileHandler(log_file)
+        handler_file.setLevel(logging._nameToLevel[log_level])
+        handler_file.setFormatter(formatter)
+        logger.addHandler(handler_file)
+
     return logger
```

### Comparing `whru-0.3/whru/utils/producer_consumer.py` & `whru-0.4/whru/utils/producer_consumer.py`

 * *Files identical despite different names*

### Comparing `whru-0.3/whru/utils/utils.py` & `whru-0.4/whru/utils/utils.py`

 * *Files identical despite different names*


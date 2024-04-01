# Comparing `tmp/telegram_collector-0.0.5.tar.gz` & `tmp/telegram_collector-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_collector-0.0.5.tar", last modified: Mon Apr  1 07:30:47 2024, max compression
+gzip compressed data, was "telegram_collector-0.0.6.tar", last modified: Mon Apr  1 14:42:30 2024, max compression
```

## Comparing `telegram_collector-0.0.5.tar` & `telegram_collector-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 07:30:47.442625 telegram_collector-0.0.5/
--rw-rw-rw-   0        0        0      287 2024-04-01 07:30:47.440573 telegram_collector-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-01 07:30:47.442625 telegram_collector-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      735 2024-04-01 07:25:53.000000 telegram_collector-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:30:47.429794 telegram_collector-0.0.5/telegram_collector/
--rw-rw-rw-   0        0        0     5381 2024-04-01 06:08:14.000000 telegram_collector-0.0.5/telegram_collector/__init__.py
--rw-rw-rw-   0        0        0      361 2024-04-01 07:25:42.000000 telegram_collector-0.0.5/telegram_collector/__main__.py
--rw-rw-rw-   0        0        0     2528 2024-04-01 05:08:12.000000 telegram_collector-0.0.5/telegram_collector/util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:30:47.440573 telegram_collector-0.0.5/telegram_collector.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-01 07:30:47.000000 telegram_collector-0.0.5/telegram_collector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-04-01 07:30:47.000000 telegram_collector-0.0.5/telegram_collector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 07:30:47.000000 telegram_collector-0.0.5/telegram_collector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      248 2024-04-01 07:30:47.000000 telegram_collector-0.0.5/telegram_collector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-01 07:30:47.000000 telegram_collector-0.0.5/telegram_collector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-01 07:30:47.000000 telegram_collector-0.0.5/telegram_collector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 14:42:30.297953 telegram_collector-0.0.6/
+-rw-rw-rw-   0        0        0      287 2024-04-01 14:42:30.294764 telegram_collector-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-01 14:42:30.297953 telegram_collector-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      735 2024-04-01 14:42:25.000000 telegram_collector-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:42:30.270366 telegram_collector-0.0.6/telegram_collector/
+-rw-rw-rw-   0        0        0     5418 2024-04-01 14:42:14.000000 telegram_collector-0.0.6/telegram_collector/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-04-01 07:25:42.000000 telegram_collector-0.0.6/telegram_collector/__main__.py
+-rw-rw-rw-   0        0        0     2528 2024-04-01 05:08:12.000000 telegram_collector-0.0.6/telegram_collector/util.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:42:30.292264 telegram_collector-0.0.6/telegram_collector.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-04-01 14:42:30.000000 telegram_collector-0.0.6/telegram_collector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-04-01 14:42:30.000000 telegram_collector-0.0.6/telegram_collector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 14:42:30.000000 telegram_collector-0.0.6/telegram_collector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      248 2024-04-01 14:42:30.000000 telegram_collector-0.0.6/telegram_collector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-01 14:42:30.000000 telegram_collector-0.0.6/telegram_collector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-01 14:42:30.000000 telegram_collector-0.0.6/telegram_collector.egg-info/top_level.txt
```

### Comparing `telegram_collector-0.0.5/telegram_collector/__init__.py` & `telegram_collector-0.0.6/telegram_collector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
             await self.__terminate_client()
 
     # 流式汇总增量消息
     async def __send_current_message_src_to_dest(self):
         async def callback(event):
             message = event.message
             src_dialog_id = event.message.chat_id
+            print('get: ', message)
             if message_is_video_or_photo(message) and src_dialog_id in self.src_dialog_ids:
                 await self.__send_messages([message])
 
         self.client.add_event_handler(callback, events.NewMessage(incoming=True))
         try:
             while True:
                 await asyncio.sleep(1)
```

### Comparing `telegram_collector-0.0.5/telegram_collector/util.py` & `telegram_collector-0.0.6/telegram_collector/util.py`

 * *Files identical despite different names*


# Comparing `tmp/telegram_bot_reporter-0.1.6.tar.gz` & `tmp/telegram_bot_reporter-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_bot_reporter-0.1.6.tar", max compression
+gzip compressed data, was "telegram_bot_reporter-0.1.7.tar", max compression
```

## Comparing `telegram_bot_reporter-0.1.6.tar` & `telegram_bot_reporter-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1020 2024-03-30 08:06:04.026651 telegram_bot_reporter-0.1.6/README.md
--rw-r--r--   0        0        0     2293 2024-03-30 10:03:38.824937 telegram_bot_reporter-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      111 2024-03-30 10:03:53.561341 telegram_bot_reporter-0.1.6/src/telegram_bot_reporter/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 06:03:42.268386 telegram_bot_reporter-0.1.6/src/telegram_bot_reporter/core/__init__.py
--rw-r--r--   0        0        0     2684 2024-03-30 10:03:53.473339 telegram_bot_reporter-0.1.6/src/telegram_bot_reporter/core/async_bot.py
--rw-r--r--   0        0        0     1089 2024-03-30 10:02:08.169747 telegram_bot_reporter-0.1.6/src/telegram_bot_reporter/core/base_bot.py
--rw-r--r--   0        0        0     2531 2024-03-30 10:03:53.473339 telegram_bot_reporter-0.1.6/src/telegram_bot_reporter/core/sync_bot.py
--rw-r--r--   0        0        0     1657 1970-01-01 00:00:00.000000 telegram_bot_reporter-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1020 2024-03-30 08:06:04.026651 telegram_bot_reporter-0.1.7/README.md
+-rw-r--r--   0        0        0     2293 2024-04-01 17:44:54.787154 telegram_bot_reporter-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      111 2024-03-30 10:03:53.561341 telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 06:03:42.268386 telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/__init__.py
+-rw-r--r--   0        0        0     2684 2024-03-30 10:03:53.473339 telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/async_bot.py
+-rw-r--r--   0        0        0      921 2024-04-01 17:44:27.743363 telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/base_bot.py
+-rw-r--r--   0        0        0     2531 2024-03-30 10:03:53.473339 telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/sync_bot.py
+-rw-r--r--   0        0        0     1657 1970-01-01 00:00:00.000000 telegram_bot_reporter-0.1.7/PKG-INFO
```

### Comparing `telegram_bot_reporter-0.1.6/README.md` & `telegram_bot_reporter-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `telegram_bot_reporter-0.1.6/pyproject.toml` & `telegram_bot_reporter-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telegram-bot-reporter"
-version = "0.1.6"
+version = "0.1.7"
 description = "Library for sending messages and files using a Telegram bot."
 authors = ["deskent <battenetciz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Deskent/bot_reporter"
 homepage = "https://pypi.org/project/telegram-bot-reporter/"
```

### Comparing `telegram_bot_reporter-0.1.6/src/telegram_bot_reporter/core/async_bot.py` & `telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/async_bot.py`

 * *Files identical despite different names*

### Comparing `telegram_bot_reporter-0.1.6/src/telegram_bot_reporter/core/base_bot.py` & `telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/base_bot.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,17 +18,13 @@
         bot_token: str,
         chat_id: str | int,
         timeout: int = 10,
         parse_mode: str = "HTML",
         prefix: str = "",
     ):
         self._token = bot_token
-        if not self._token:
-            raise ValueError("Token cannot be empty")
         self._chat_id: str = str(chat_id)
-        if not self._chat_id:
-            raise ValueError("Chat id cannot be empty")
         self._timeout = timeout
         self._parse_mode = parse_mode
         self._prefix = prefix
         self._headers: dict = {"Content-Type": "application/json"}
         self._url = f"https://api.telegram.org/bot{self._token}"
```

### Comparing `telegram_bot_reporter-0.1.6/src/telegram_bot_reporter/core/sync_bot.py` & `telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/sync_bot.py`

 * *Files identical despite different names*

### Comparing `telegram_bot_reporter-0.1.6/PKG-INFO` & `telegram_bot_reporter-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-bot-reporter
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library for sending messages and files using a Telegram bot.
 Home-page: https://pypi.org/project/telegram-bot-reporter/
 License: MIT
 Author: deskent
 Author-email: battenetciz@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


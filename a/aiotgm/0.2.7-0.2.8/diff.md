# Comparing `tmp/aiotgm-0.2.7.tar.gz` & `tmp/aiotgm-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotgm-0.2.7.tar", last modified: Wed Mar 27 15:47:53 2024, max compression
+gzip compressed data, was "aiotgm-0.2.8.tar", last modified: Mon Apr  1 12:35:58 2024, max compression
```

## Comparing `aiotgm-0.2.7.tar` & `aiotgm-0.2.8.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-03-27 15:47:53.264504 aiotgm-0.2.7/
--rw-r--r--   0 kali      (1000) root         (0)    35149 2023-12-11 13:46:43.000000 aiotgm-0.2.7/LICENSE
--rw-r--r--   0 kali      (1000) root         (0)    42093 2024-03-27 15:47:53.264504 aiotgm-0.2.7/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)     1238 2024-03-14 20:23:30.000000 aiotgm-0.2.7/README.md
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-03-27 15:47:53.256504 aiotgm-0.2.7/aiotgm/
--rw-r--r--   0 kali      (1000) root         (0)      321 2024-03-27 15:46:13.000000 aiotgm-0.2.7/aiotgm/__init__.py
--rw-r--r--   0 kali      (1000) root         (0)      740 2024-03-23 08:23:03.000000 aiotgm-0.2.7/aiotgm/_logging.py
--rw-r--r--   0 kali      (1000) root         (0)    27723 2024-03-27 11:17:13.000000 aiotgm-0.2.7/aiotgm/api.py
--rw-r--r--   0 kali      (1000) root         (0)   264849 2024-03-27 11:56:20.000000 aiotgm-0.2.7/aiotgm/client.py
--rw-r--r--   0 kali      (1000) root         (0)     3123 2024-02-29 15:03:03.000000 aiotgm-0.2.7/aiotgm/constants.py
--rw-r--r--   0 kali      (1000) root         (0)   198270 2024-03-22 17:14:17.000000 aiotgm-0.2.7/aiotgm/types.py
--rw-r--r--   0 kali      (1000) root         (0)     8374 2024-03-22 16:53:52.000000 aiotgm-0.2.7/aiotgm/update_manager.py
--rw-r--r--   0 kali      (1000) root         (0)      623 2024-03-17 17:13:52.000000 aiotgm-0.2.7/aiotgm/utils.py
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-03-27 15:47:53.264504 aiotgm-0.2.7/aiotgm.egg-info/
--rw-r--r--   0 kali      (1000) root         (0)    42093 2024-03-27 15:47:53.000000 aiotgm-0.2.7/aiotgm.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)      369 2024-03-27 15:47:53.000000 aiotgm-0.2.7/aiotgm.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) root         (0)        1 2024-03-27 15:47:53.000000 aiotgm-0.2.7/aiotgm.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) root         (0)       48 2024-03-27 15:47:53.000000 aiotgm-0.2.7/aiotgm.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) root         (0)        7 2024-03-27 15:47:53.000000 aiotgm-0.2.7/aiotgm.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) root         (0)      441 2024-03-27 15:46:10.000000 aiotgm-0.2.7/pyproject.toml
--rw-r--r--   0 kali      (1000) root         (0)       38 2024-03-27 15:47:53.264504 aiotgm-0.2.7/setup.cfg
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-03-27 15:47:53.264504 aiotgm-0.2.7/tests/
--rw-r--r--   0 kali      (1000) root         (0)     1471 2024-03-14 20:26:02.000000 aiotgm-0.2.7/tests/test_func_ok.py
--rw-r--r--   0 kali      (1000) root         (0)   147188 2024-03-27 12:05:44.000000 aiotgm-0.2.7/tests/test_types.py
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 12:35:58.276560 aiotgm-0.2.8/
+-rw-r--r--   0 kali      (1000) root         (0)    35149 2023-12-11 13:46:43.000000 aiotgm-0.2.8/LICENSE
+-rw-r--r--   0 kali      (1000) root         (0)    42093 2024-04-01 12:35:58.276560 aiotgm-0.2.8/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)     1238 2024-03-14 20:23:30.000000 aiotgm-0.2.8/README.md
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 12:35:58.276560 aiotgm-0.2.8/aiotgm/
+-rw-r--r--   0 kali      (1000) root         (0)      320 2024-04-01 12:34:03.000000 aiotgm-0.2.8/aiotgm/__init__.py
+-rw-r--r--   0 kali      (1000) root         (0)    27730 2024-03-30 13:15:28.000000 aiotgm-0.2.8/aiotgm/api.py
+-rw-r--r--   0 kali      (1000) root         (0)   267285 2024-03-30 12:22:23.000000 aiotgm-0.2.8/aiotgm/client.py
+-rw-r--r--   0 kali      (1000) root         (0)     3123 2024-02-29 15:03:03.000000 aiotgm-0.2.8/aiotgm/constants.py
+-rw-r--r--   0 kali      (1000) root         (0)      740 2024-04-01 12:33:00.000000 aiotgm-0.2.8/aiotgm/logging.py
+-rw-r--r--   0 kali      (1000) root         (0)   271955 2024-04-01 11:17:22.000000 aiotgm-0.2.8/aiotgm/types.py
+-rw-r--r--   0 kali      (1000) root         (0)     8374 2024-03-22 16:53:52.000000 aiotgm-0.2.8/aiotgm/update_manager.py
+-rw-r--r--   0 kali      (1000) root         (0)      623 2024-03-17 17:13:52.000000 aiotgm-0.2.8/aiotgm/utils.py
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 12:35:58.276560 aiotgm-0.2.8/aiotgm.egg-info/
+-rw-r--r--   0 kali      (1000) root         (0)    42093 2024-04-01 12:35:58.000000 aiotgm-0.2.8/aiotgm.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)      348 2024-04-01 12:35:58.000000 aiotgm-0.2.8/aiotgm.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) root         (0)        1 2024-04-01 12:35:58.000000 aiotgm-0.2.8/aiotgm.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) root         (0)       48 2024-04-01 12:35:58.000000 aiotgm-0.2.8/aiotgm.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-01 12:35:58.000000 aiotgm-0.2.8/aiotgm.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) root         (0)      441 2024-04-01 12:33:56.000000 aiotgm-0.2.8/pyproject.toml
+-rw-r--r--   0 kali      (1000) root         (0)       38 2024-04-01 12:35:58.276560 aiotgm-0.2.8/setup.cfg
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 12:35:58.276560 aiotgm-0.2.8/tests/
+-rw-r--r--   0 kali      (1000) root         (0)     1471 2024-03-14 20:26:02.000000 aiotgm-0.2.8/tests/test_func_ok.py
```

### Comparing `aiotgm-0.2.7/LICENSE` & `aiotgm-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotgm-0.2.7/PKG-INFO` & `aiotgm-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgm
-Version: 0.2.7
+Version: 0.2.8
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `aiotgm-0.2.7/README.md` & `aiotgm-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `aiotgm-0.2.7/aiotgm/_logging.py` & `aiotgm-0.2.8/aiotgm/logging.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.2.7/aiotgm/api.py` & `aiotgm-0.2.8/aiotgm/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 def _format_url(token: str, method: str, /) -> str:
     return '/bot{}/{}'.format(token, method)
 
 
 class TelegramError(Exception):
     '''
-    Class to handle unsuccessful requests to the Telegram Bot API.
+    Class to handle unsuccessful requests to the Telegram Bot API Server.
 
     :param error_code: The status code of the unsuccessful request.
     :type error_code: :obj:`int`
     :param description: Description of why the request was unsuccessful.
     :type description: :obj:`str`
     '''
     def __init__(self, error_code: int, description: str):
```

### Comparing `aiotgm-0.2.7/aiotgm/client.py` & `aiotgm-0.2.8/aiotgm/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,15 @@
     # 18 UpdateManagers
 
     def manage_message(self, checker: Callable[[Message], Any] = lambda message: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *message* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.Message`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.Message` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -182,14 +183,15 @@
         return wrap
 
     def manage_edited_message(self, checker: Callable[[Message], Any] = lambda edited_message: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *edited_message* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.Message`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.Message` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -211,14 +213,15 @@
         return wrap
 
     def manage_channel_post(self, checker: Callable[[Message], Any] = lambda channel_post: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *channel_post* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.Message`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.Message` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -240,14 +243,15 @@
         return wrap
 
     def manage_edited_channel_post(self, checker: Callable[[Message], Any] = lambda edited_channel_post: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *edited_channel_post* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.Message`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.Message` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -269,14 +273,15 @@
         return wrap
 
     def manage_message_reaction(self, checker: Callable[[MessageReactionUpdated], Any] = lambda message_reaction: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *message_reaction* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.MessageReactionUpdated`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.MessageReactionUpdated` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -298,14 +303,15 @@
         return wrap
 
     def manage_message_reaction_count(self, checker: Callable[[MessageReactionCountUpdated], Any] = lambda message_reaction_count: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *message_reaction_count* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.MessageReactionCountUpdated`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.MessageReactionCountUpdated` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -327,14 +333,15 @@
         return wrap
 
     def manage_inline_query(self, checker: Callable[[InlineQuery], Any] = lambda inline_query: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *inline_query* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.InlineQuery`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.InlineQuery` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -356,14 +363,15 @@
         return wrap
 
     def manage_chosen_inline_result(self, checker: Callable[[ChosenInlineResult], Any] = lambda chosen_inline_result: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *chosen_inline_result* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.ChosenInlineResult`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.ChosenInlineResult` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -385,14 +393,15 @@
         return wrap
 
     def manage_callback_query(self, checker: Callable[[CallbackQuery], Any] = lambda callback_query: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *callback_query* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.CallbackQuery`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.CallbackQuery` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -414,14 +423,15 @@
         return wrap
 
     def manage_shipping_query(self, checker: Callable[[ShippingQuery], Any] = lambda shipping_query: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *shipping_query* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.ShippingQuery`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.ShippingQuery` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -443,14 +453,15 @@
         return wrap
 
     def manage_pre_checkout_query(self, checker: Callable[[PreCheckoutQuery], Any] = lambda pre_checkout_query: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *pre_checkout_query* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.PreCheckoutQuery`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.PreCheckoutQuery` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -472,14 +483,15 @@
         return wrap
 
     def manage_poll(self, checker: Callable[[Poll], Any] = lambda poll: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *poll* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.Poll`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.Poll` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -501,14 +513,15 @@
         return wrap
 
     def manage_poll_answer(self, checker: Callable[[PollAnswer], Any] = lambda poll_answer: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *poll_answer* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.PollAnswer`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.PollAnswer` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -530,14 +543,15 @@
         return wrap
 
     def manage_my_chat_member(self, checker: Callable[[ChatMemberUpdated], Any] = lambda my_chat_member: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *my_chat_member* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.ChatMemberUpdated`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.ChatMemberUpdated` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -559,14 +573,15 @@
         return wrap
 
     def manage_chat_member(self, checker: Callable[[ChatMemberUpdated], Any] = lambda chat_member: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *chat_member* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.ChatMemberUpdated`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.ChatMemberUpdated` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -588,14 +603,15 @@
         return wrap
 
     def manage_chat_join_request(self, checker: Callable[[ChatJoinRequest], Any] = lambda chat_join_request: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *chat_join_request* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.ChatJoinRequest`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.ChatJoinRequest` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -617,14 +633,15 @@
         return wrap
 
     def manage_chat_boost(self, checker: Callable[[ChatBoostUpdated], Any] = lambda chat_boost: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *chat_boost* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.ChatBoostUpdated`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.ChatBoostUpdated` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -646,14 +663,15 @@
         return wrap
 
     def manage_removed_chat_boost(self, checker: Callable[[ChatBoostRemoved], Any] = lambda removed_chat_boost: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *removed_chat_boost* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.ChatBoostRemoved`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.ChatBoostRemoved` update.
 
         Usage:
 
         .. code-block:: python3
 
             import aiotgm
             import asyncio
@@ -1274,15 +1292,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.MessageId`
         '''
         params = {
             'chat_id': chat_id,
             'from_chat_id': from_chat_id,
             'message_id': message_id
         }
@@ -2966,15 +2984,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'animation': animation
         }
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
@@ -3044,15 +3062,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'audio': audio
         }
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
@@ -3143,15 +3161,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'phone_number': phone_number,
             'first_name': first_name
         }
@@ -3192,15 +3210,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id
         }
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if emoji is not None: params['emoji'] = emoji
@@ -3254,15 +3272,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'document': document
         }
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
@@ -3493,15 +3511,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'latitude': latitude,
             'longitude': longitude
         }
@@ -3596,15 +3614,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'text': text
         }
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
@@ -3658,15 +3676,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'photo': photo
         }
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
@@ -3742,15 +3760,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'question': question,
             'options': options
         }
@@ -3802,15 +3820,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'sticker': sticker
         }
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
@@ -3870,15 +3888,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'latitude': latitude,
             'longitude': longitude,
             'title': title,
@@ -3952,15 +3970,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'video': video
         }
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
@@ -4018,15 +4036,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'video_note': video_note
         }
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
@@ -4082,15 +4100,15 @@
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
-        :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardMarkup` or :obj:`~aiotgm.types.ReplyKeyboardRemove` or :obj:`~aiotgm.types.ForceReply`, optional
+        :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'voice': voice
         }
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
```

### Comparing `aiotgm-0.2.7/aiotgm/constants.py` & `aiotgm-0.2.8/aiotgm/constants.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.2.7/aiotgm/update_manager.py` & `aiotgm-0.2.8/aiotgm/update_manager.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.2.7/aiotgm/utils.py` & `aiotgm-0.2.8/aiotgm/utils.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.2.7/aiotgm.egg-info/PKG-INFO` & `aiotgm-0.2.8/aiotgm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgm
-Version: 0.2.7
+Version: 0.2.8
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `aiotgm-0.2.7/tests/test_func_ok.py` & `aiotgm-0.2.8/tests/test_func_ok.py`

 * *Files identical despite different names*


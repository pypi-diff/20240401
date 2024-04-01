# Comparing `tmp/aiotgm-0.2.9.tar.gz` & `tmp/aiotgm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotgm-0.2.9.tar", last modified: Mon Apr  1 12:40:14 2024, max compression
+gzip compressed data, was "aiotgm-0.3.0.tar", last modified: Mon Apr  1 15:32:35 2024, max compression
```

## Comparing `aiotgm-0.2.9.tar` & `aiotgm-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 12:40:14.632573 aiotgm-0.2.9/
--rw-r--r--   0 kali      (1000) root         (0)    35149 2023-12-11 13:46:43.000000 aiotgm-0.2.9/LICENSE
--rw-r--r--   0 kali      (1000) root         (0)    42093 2024-04-01 12:40:14.632573 aiotgm-0.2.9/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)     1238 2024-03-14 20:23:30.000000 aiotgm-0.2.9/README.md
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 12:40:14.628573 aiotgm-0.2.9/aiotgm/
--rw-r--r--   0 kali      (1000) root         (0)      320 2024-04-01 12:39:11.000000 aiotgm-0.2.9/aiotgm/__init__.py
--rw-r--r--   0 kali      (1000) root         (0)    27730 2024-03-30 13:15:28.000000 aiotgm-0.2.9/aiotgm/api.py
--rw-r--r--   0 kali      (1000) root         (0)   267285 2024-03-30 12:22:23.000000 aiotgm-0.2.9/aiotgm/client.py
--rw-r--r--   0 kali      (1000) root         (0)     3123 2024-02-29 15:03:03.000000 aiotgm-0.2.9/aiotgm/constants.py
--rw-r--r--   0 kali      (1000) root         (0)      740 2024-04-01 12:33:00.000000 aiotgm-0.2.9/aiotgm/logging.py
--rw-r--r--   0 kali      (1000) root         (0)   271955 2024-04-01 11:17:22.000000 aiotgm-0.2.9/aiotgm/types.py
--rw-r--r--   0 kali      (1000) root         (0)     8374 2024-03-22 16:53:52.000000 aiotgm-0.2.9/aiotgm/update_manager.py
--rw-r--r--   0 kali      (1000) root         (0)      623 2024-03-17 17:13:52.000000 aiotgm-0.2.9/aiotgm/utils.py
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 12:40:14.632573 aiotgm-0.2.9/aiotgm.egg-info/
--rw-r--r--   0 kali      (1000) root         (0)    42093 2024-04-01 12:40:14.000000 aiotgm-0.2.9/aiotgm.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)      348 2024-04-01 12:40:14.000000 aiotgm-0.2.9/aiotgm.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) root         (0)        1 2024-04-01 12:40:14.000000 aiotgm-0.2.9/aiotgm.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) root         (0)       48 2024-04-01 12:40:14.000000 aiotgm-0.2.9/aiotgm.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-01 12:40:14.000000 aiotgm-0.2.9/aiotgm.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) root         (0)      441 2024-04-01 12:39:08.000000 aiotgm-0.2.9/pyproject.toml
--rw-r--r--   0 kali      (1000) root         (0)       38 2024-04-01 12:40:14.632573 aiotgm-0.2.9/setup.cfg
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 12:40:14.632573 aiotgm-0.2.9/tests/
--rw-r--r--   0 kali      (1000) root         (0)     1471 2024-03-14 20:26:02.000000 aiotgm-0.2.9/tests/test_func_ok.py
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 15:32:35.916658 aiotgm-0.3.0/
+-rw-r--r--   0 kali      (1000) root         (0)    35149 2023-12-11 13:46:43.000000 aiotgm-0.3.0/LICENSE
+-rw-r--r--   0 kali      (1000) root         (0)    42093 2024-04-01 15:32:35.916658 aiotgm-0.3.0/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)     1238 2024-03-14 20:23:30.000000 aiotgm-0.3.0/README.md
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 15:32:35.908658 aiotgm-0.3.0/aiotgm/
+-rw-r--r--   0 kali      (1000) root         (0)      320 2024-04-01 15:32:31.000000 aiotgm-0.3.0/aiotgm/__init__.py
+-rw-r--r--   0 kali      (1000) root         (0)    27730 2024-03-30 13:15:28.000000 aiotgm-0.3.0/aiotgm/api.py
+-rw-r--r--   0 kali      (1000) root         (0)   273097 2024-04-01 15:19:49.000000 aiotgm-0.3.0/aiotgm/client.py
+-rw-r--r--   0 kali      (1000) root         (0)     3123 2024-02-29 15:03:03.000000 aiotgm-0.3.0/aiotgm/constants.py
+-rw-r--r--   0 kali      (1000) root         (0)      740 2024-04-01 12:33:00.000000 aiotgm-0.3.0/aiotgm/logging.py
+-rw-r--r--   0 kali      (1000) root         (0)   275718 2024-04-01 15:29:33.000000 aiotgm-0.3.0/aiotgm/types.py
+-rw-r--r--   0 kali      (1000) root         (0)     8932 2024-04-01 15:14:03.000000 aiotgm-0.3.0/aiotgm/update_manager.py
+-rw-r--r--   0 kali      (1000) root         (0)      623 2024-03-17 17:13:52.000000 aiotgm-0.3.0/aiotgm/utils.py
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 15:32:35.912658 aiotgm-0.3.0/aiotgm.egg-info/
+-rw-r--r--   0 kali      (1000) root         (0)    42093 2024-04-01 15:32:35.000000 aiotgm-0.3.0/aiotgm.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)      348 2024-04-01 15:32:35.000000 aiotgm-0.3.0/aiotgm.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) root         (0)        1 2024-04-01 15:32:35.000000 aiotgm-0.3.0/aiotgm.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) root         (0)       48 2024-04-01 15:32:35.000000 aiotgm-0.3.0/aiotgm.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-01 15:32:35.000000 aiotgm-0.3.0/aiotgm.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) root         (0)      441 2024-04-01 15:32:28.000000 aiotgm-0.3.0/pyproject.toml
+-rw-r--r--   0 kali      (1000) root         (0)       38 2024-04-01 15:32:35.916658 aiotgm-0.3.0/setup.cfg
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 15:32:35.912658 aiotgm-0.3.0/tests/
+-rw-r--r--   0 kali      (1000) root         (0)     1471 2024-03-14 20:26:02.000000 aiotgm-0.3.0/tests/test_func_ok.py
```

### Comparing `aiotgm-0.2.9/LICENSE` & `aiotgm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotgm-0.2.9/PKG-INFO` & `aiotgm-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgm
-Version: 0.2.9
+Version: 0.3.0
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `aiotgm-0.2.9/README.md` & `aiotgm-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aiotgm-0.2.9/aiotgm/api.py` & `aiotgm-0.3.0/aiotgm/api.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.2.9/aiotgm/client.py` & `aiotgm-0.3.0/aiotgm/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     UpdateManager,
     _run_coroutine,
     _is_next_function,
     MESSAGE_MANAGER,
     EDITED_MESSAGE_MANAGER, 
     CHANNEL_POST_MANAGER, 
     EDITED_CHANNEL_POST_MANAGER,
+    BUSINESS_CONNECTION_MANAGER,
+    BUSINESS_MESSAGE_MANAGER,
+    EDITED_BUSINESS_MESSAGE_MANAGER,
     MESSAGE_REACTION_MANAGER,
     MESSAGE_REACTION_COUNT_MANAGER,
     INLINE_QUERY_MANAGER,
     CHOSEN_INLINE_RESULT_MANAGER,
     CALLBACK_QUERY_MANAGER,
     SHIPPING_QUERY_MANAGER,
     PRE_CHECKOUT_QUERY_MANAGER,
@@ -83,14 +86,17 @@
         self.parse_mode = parse_mode
         self.protect_content = protect_content
 
         self._message_manager = UpdateManager(MESSAGE_MANAGER, Message)
         self._edited_message_manager = UpdateManager(EDITED_MESSAGE_MANAGER, Message)
         self._channel_post_manager = UpdateManager(CHANNEL_POST_MANAGER, Message)
         self._edited_channel_post_manager = UpdateManager(EDITED_CHANNEL_POST_MANAGER, Message)
+        self._business_connection_manager = UpdateManager(BUSINESS_CONNECTION_MANAGER, BusinessConnection)
+        self._business_message_manager = UpdateManager(BUSINESS_MESSAGE_MANAGER, Message)
+        self._edited_business_message_manager = UpdateManager(EDITED_BUSINESS_MESSAGE_MANAGER, Message)
         self._message_reaction_manager = UpdateManager(MESSAGE_REACTION_MANAGER, MessageReactionUpdated)
         self._message_reaction_count_manager = UpdateManager(MESSAGE_REACTION_COUNT_MANAGER, MessageReactionCountUpdated)
         self._inline_query_manager = UpdateManager(INLINE_QUERY_MANAGER, InlineQuery)
         self._chosen_inline_result_manager = UpdateManager(CHOSEN_INLINE_RESULT_MANAGER, ChosenInlineResult)
         self._callback_query_manager = UpdateManager(CALLBACK_QUERY_MANAGER, CallbackQuery)
         self._shipping_query_manager = UpdateManager(SHIPPING_QUERY_MANAGER, ShippingQuery)
         self._pre_checkout_query_manager = UpdateManager(PRE_CHECKOUT_QUERY_MANAGER, PreCheckoutQuery)
@@ -146,15 +152,15 @@
         return self._protect_content
 
     @protect_content.setter
     def protect_content(self, val: Optional[bool]):
         self._protect_content = True if val else None
 
 
-    # 18 UpdateManagers
+    # UpdateManagers
 
     def manage_message(self, checker: Callable[[Message], Any] = lambda message: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *message* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.Message`.
         Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.Message` update.
@@ -268,14 +274,104 @@
         :param checker: A function that takes only one argument to check an incoming *edited_channel_post* :obj:`~aiotgm.types.Update`. E.g. a lambda function.
         :type checker: :obj:`Callable[[Message], Any]`
         '''
         def wrap(coroutine: Callable[[Message], Awaitable]):
             self._edited_channel_post_manager.add_rule(checker, coroutine)
         return wrap
 
+    def manage_business_connection(self, checker: Callable[[BusinessConnection], Any] = lambda business_connection: ..., /):
+        '''
+        You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
+        inside this decorator to manage an incoming *business_connection* :obj:`~aiotgm.types.Update`.
+        The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.BusinessConnection`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.BusinessConnection` update.
+
+        Usage:
+
+        .. code-block:: python3
+
+            import aiotgm
+            import asyncio
+            from aiotgm.types import BusinessConnection
+
+            bot = aiotgm.Client('<your_api_token>')
+
+            @bot.manage_business_connection(lambda business_connection: business_connection.user.id == xyz)
+            async def foo(business_connection: BusinessConnection):
+                ...
+
+            asyncio.run(bot.long_polling())
+
+        :param checker: A function that takes only one argument to check an incoming *business_connection* :obj:`~aiotgm.types.Update`. E.g. a lambda function.
+        :type checker: :obj:`Callable[[BusinessConnection], Any]`
+        '''
+        def wrap(coroutine: Callable[[BusinessConnection], Awaitable]):
+            self._business_connection_manager.add_rule(checker, coroutine)
+        return wrap
+
+    def manage_business_message(self, checker: Callable[[Message], Any] = lambda business_message: ..., /):
+        '''
+        You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
+        inside this decorator to manage an incoming *business_message* :obj:`~aiotgm.types.Update`.
+        The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.Message`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.Message` update.
+
+        Usage:
+
+        .. code-block:: python3
+
+            import aiotgm
+            import asyncio
+            from aiotgm.types import Message
+
+            bot = aiotgm.Client('<your_api_token>')
+
+            @bot.manage_business_message(lambda business_message: business_message.chat.id == xyz)
+            async def foo(business_message: Message):
+                ...
+
+            asyncio.run(bot.long_polling())
+
+        :param checker: A function that takes only one argument to check an incoming *business_message* :obj:`~aiotgm.types.Update`. E.g. a lambda function.
+        :type checker: :obj:`Callable[[Message], Any]`
+        '''
+        def wrap(coroutine: Callable[[Message], Awaitable]):
+            self._business_message_manager.add_rule(checker, coroutine)
+        return wrap
+
+    def manage_edited_business_message(self, checker: Callable[[Message], Any] = lambda edited_business_message: ..., /):
+        '''
+        You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
+        inside this decorator to manage an incoming *edited_business_message* :obj:`~aiotgm.types.Update`.
+        The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.Message`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.Message` update.
+
+        Usage:
+
+        .. code-block:: python3
+
+            import aiotgm
+            import asyncio
+            from aiotgm.types import Message
+
+            bot = aiotgm.Client('<your_api_token>')
+
+            @bot.manage_business_message(lambda edited_business_message: edited_business_message.chat.id == xyz)
+            async def foo(edited_business_message: Message):
+                ...
+
+            asyncio.run(bot.long_polling())
+
+        :param checker: A function that takes only one argument to check an incoming *edited_business_message* :obj:`~aiotgm.types.Update`. E.g. a lambda function.
+        :type checker: :obj:`Callable[[Message], Any]`
+        '''
+        def wrap(coroutine: Callable[[Message], Awaitable]):
+            self._business_message_manager.add_rule(checker, coroutine)
+        return wrap
+
     def manage_message_reaction(self, checker: Callable[[MessageReactionUpdated], Any] = lambda message_reaction: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *message_reaction* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.MessageReactionUpdated`.
         Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.MessageReactionUpdated` update.
 
@@ -803,14 +899,35 @@
         elif update.edited_channel_post:
             obj: Message = update.edited_channel_post
             for rule in self._edited_channel_post_manager:
                 result = await _run_coroutine(rule, obj)
                 if not _is_next_function(result):
                     return
 
+        elif update.business_connection:
+            obj: BusinessConnection = update.business_connection
+            for rule in self._business_connection_manager:
+                result = await _run_coroutine(rule, obj)
+                if not _is_next_function(result):
+                    return
+
+        elif update.business_message:
+            obj: Message = update.business_message
+            for rule in self._business_message_manager:
+                result = await _run_coroutine(rule, obj)
+                if not _is_next_function(result):
+                    return
+
+        elif update.edited_business_message:
+            obj: Message = update.edited_business_message
+            for rule in self._edited_business_message_manager:
+                result = await _run_coroutine(rule, obj)
+                if not _is_next_function(result):
+                    return
+
         elif update.message_reaction:
             obj: MessageReactionUpdated = update.message_reaction
             for rule in self._message_reaction_manager:
                 result = await _run_coroutine(rule, obj)
                 if not _is_next_function(result):
                     return
```

### Comparing `aiotgm-0.2.9/aiotgm/constants.py` & `aiotgm-0.3.0/aiotgm/constants.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.2.9/aiotgm/logging.py` & `aiotgm-0.3.0/aiotgm/logging.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.2.9/aiotgm/types.py` & `aiotgm-0.3.0/aiotgm/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     'BotCommandScopeChat',
     'BotCommandScopeChatAdministrators',
     'BotCommandScopeChatMember',
     'BotCommandScopeDefault',
     'BotDescription',
     'BotName',
     'BotShortDescription',
+    'BusinessConnection',
     'CallbackGame',
     'CallbackQuery',
     'Chat',
     'ChatAdministratorRights',
     'ChatBoost',
     'ChatBoostAdded',
     'ChatBoostRemoved',
@@ -549,14 +550,95 @@
     def __init__(
         self,
         short_description: str
     ):
         self.short_description = short_description
 
 
+class BusinessConnection(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#businessconnection
+
+    Describes the connection of the bot with a business account.
+
+    :param id: Unique identifier of the business connection.
+    :type id: :obj:`str`
+    :param user: Business account user that created the business connection.
+    :type user: :obj:`~aiotgm.types.User`
+    :param user_chat_id: Identifier of a private chat with the user who created the business connection. This number may have more than 32 significant bits and some programming languages may have difficulty/silent defects in interpreting it. But it has at most 52 significant bits, so a 64-bit integer or double-precision float type are safe for storing this identifier.
+    :type user_chat_id: :obj:`int`
+    :param date: Date the connection was established in Unix time.
+    :type date: :obj:`int`
+    :param can_reply: :obj:`True`, if the bot can act on behalf of the business account in chats that were active in the last 24 hours.
+    :type can_reply: :obj:`bool`
+    :param is_enabled: :obj:`True`, if the connection is active.
+    :type is_enabled: :obj:`bool`
+    '''
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['id'] = res.get('id')
+        obj['user'] = User._dese(res.get('user'))
+        obj['user_chat_id'] = res.get('user_chat_id')
+        obj['date'] = res.get('date')
+        obj['can_reply'] = res.get('can_reply')
+        obj['is_enabled'] = res.get('is_enabled')
+        return cls(**obj)
+
+    def __init__(
+        self,
+        id: str,
+        user: User,
+        user_chat_id: int,
+        date: int,
+        can_reply: bool,
+        is_enabled: bool,
+    ):
+        self.id = id
+        self.user = user
+        self.user_chat_id = user_chat_id
+        self.date = date
+        self.can_reply = can_reply
+        self.is_enabled = is_enabled
+
+
+class BusinessMessagesDeleted(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#businessmessagesdeleted
+
+    This object is received when messages are deleted from a connected business account.
+
+    :param business_connection_id: Unique identifier of the business connection.
+    :type business_connection_id: :obj:`str`
+    :param chat: Information about a chat in the business account. The bot may not have access to the chat or the corresponding user.
+    :type chat: :obj:`~aiotgm.types.Chat`
+    :param message_ids: A JSON-serialized list of identifiers of deleted messages in the chat of the business account.
+    :type message_ids: :obj:`list` of :obj:`int`
+    '''
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['business_connection_id'] = res.get('business_connection_id')
+        obj['chat'] = Chat._dese(res.get('chat'))
+        obj['message_ids'] = res.get('message_ids')
+        return cls(**obj)
+
+    def __init__(
+        self,
+        business_connection_id: str,
+        chat: Chat,
+        message_ids: list[int]
+    ):
+        self.business_connection_id = business_connection_id
+        self.message_ids = chat
+        self.message_ids = message_ids
+
+
 class CallbackGame(TelegramType):
     '''
     https://core.telegram.org/bots/api#callbackgame
 
     A placeholder, currently holds no information. Use `BotFather <https://t.me/botfather>`_ to set up your game.
     '''
     @classmethod
@@ -6771,14 +6853,17 @@
     def _dese(cls, res: dict):
         obj = {}
         obj['update_id'] = res.get('update_id')
         obj['message'] = Message._dese(res.get('message'))
         obj['edited_message'] = Message._dese(res.get('edited_message'))
         obj['channel_post'] = Message._dese(res.get('channel_post'))
         obj['edited_channel_post'] = Message._dese(res.get('edited_channel_post'))
+        obj['business_connection'] = BusinessConnection._dese(res.get('business_connection'))
+        obj['business_message'] = Message._dese(res.get('business_message'))
+        obj['edited_business_message'] = Message._dese(res.get('edited_business_message'))
         obj['message_reaction'] = MessageReactionUpdated._dese(res.get('message_reaction'))
         obj['message_reaction_count'] = MessageReactionCountUpdated._dese(res.get('message_reaction_count'))
         obj['inline_query'] = InlineQuery._dese(res.get('inline_query'))
         obj['chosen_inline_result'] = ChosenInlineResult._dese(res.get('chosen_inline_result'))
         obj['callback_query'] = CallbackQuery._dese(res.get('callback_query'))
         obj['shipping_query'] = ShippingQuery._dese(res.get('shipping_query'))
         obj['pre_checkout_query'] = PreCheckoutQuery._dese(res.get('pre_checkout_query'))
@@ -6794,14 +6879,17 @@
     def __init__(
         self,
         update_id: int,
         message: Optional[Message] = None,
         edited_message: Optional[Message] = None,
         channel_post: Optional[Message] = None,
         edited_channel_post: Optional[Message] = None,
+        business_connection: Optional[BusinessConnection] = None,
+        business_message: Optional[Message] = None,
+        edited_business_message: Optional[Message] = None,
         message_reaction: Optional[MessageReactionUpdated] = None,
         message_reaction_count: Optional[MessageReactionCountUpdated] = None,
         inline_query: Optional[InlineQuery] = None,
         chosen_inline_result: Optional[ChosenInlineResult] = None,
         callback_query: Optional[CallbackQuery] = None,
         shipping_query: Optional[ShippingQuery] = None,
         pre_checkout_query: Optional[PreCheckoutQuery] = None,
@@ -6814,14 +6902,17 @@
         removed_chat_boost: Optional[ChatBoostRemoved] = None
     ):
         self.update_id = update_id
         self.message = message
         self.edited_message = edited_message
         self.channel_post = channel_post
         self.edited_channel_post = edited_channel_post
+        self.business_connection = business_connection
+        self.business_message = business_message
+        self.edited_business_message = edited_business_message
         self.message_reaction = message_reaction
         self.message_reaction_count = message_reaction_count
         self.inline_query = inline_query
         self.chosen_inline_result = chosen_inline_result
         self.callback_query = callback_query
         self.shipping_query = shipping_query
         self.pre_checkout_query = pre_checkout_query
```

### Comparing `aiotgm-0.2.9/aiotgm/update_manager.py` & `aiotgm-0.3.0/aiotgm/update_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 )
 from . import logger
 
 MESSAGE_MANAGER = 'message_manager'
 EDITED_MESSAGE_MANAGER = 'edited_message_manager'
 CHANNEL_POST_MANAGER = 'channel_post_manager'
 EDITED_CHANNEL_POST_MANAGER = 'edited_channel_post_manager'
+BUSINESS_CONNECTION_MANAGER = 'business_connection_manager'
+BUSINESS_MESSAGE_MANAGER = 'business_message_manager'
+EDITED_BUSINESS_MESSAGE_MANAGER = 'edited_business_message_manager'
 MESSAGE_REACTION_MANAGER = 'message_reaction_manager'
 MESSAGE_REACTION_COUNT_MANAGER = 'message_reaction_count_manager'
 INLINE_QUERY_MANAGER = 'inline_query_manager'
 CHOSEN_INLINE_RESULT_MANAGER = 'chosen_inline_result_manager'
 CALLBACK_QUERY_MANAGER = 'callback_query_manager'
 SHIPPING_QUERY_MANAGER = 'shipping_query_manager'
 PRE_CHECKOUT_QUERY_MANAGER = 'pre_checkout_query_manager'
@@ -32,14 +35,17 @@
 REMOVED_CHAT_BOOST_MANAGER = 'removed_chat_boost_manager'
 
 EXAMPLES = {
     MESSAGE_MANAGER : ("message", "lambda message: message.chat.id == xyz"),
     EDITED_MESSAGE_MANAGER : ("edited_message", "lambda edited_message: edited_message.chat.id == xyz"),
     CHANNEL_POST_MANAGER : ("channel_post", "lambda channel_post: channel_post.chat.id == xyz"),
     EDITED_CHANNEL_POST_MANAGER : ("edited_channel_post", "lambda edited_channel_post: edited_channel_post.chat.id == xyz"),
+    BUSINESS_CONNECTION_MANAGER: ("business_connection", "lambda business_connection: business_connection.user.id == xyz"),
+    BUSINESS_MESSAGE_MANAGER: ("business_message", "lambda business_message: business_message.chat.id == xyz"),
+    EDITED_BUSINESS_MESSAGE_MANAGER: ("edited_business_message", "lambda edited_business_message: edited_business_message.chat.id == xyz"),
     MESSAGE_REACTION_MANAGER: ("message_reaction", "lambda message_reaction: message_reaction.chat.id == xyz"),
     MESSAGE_REACTION_COUNT_MANAGER: ("message_reaction_count", "lambda message_reaction_count: message_reaction_count.chat.id == xyz"),
     INLINE_QUERY_MANAGER : ("inline_query", "lambda inline_query: inline_query.from_user.id == xyz"),
     CHOSEN_INLINE_RESULT_MANAGER : ("chosen_inline_result", "lambda chosen_inline_result: chosen_inline_result.from_user.id == xyz"),
     CALLBACK_QUERY_MANAGER : ("callback_query", "lambda callback_query: callback_query.from_user.id == xyz"),
     SHIPPING_QUERY_MANAGER : ("shipping_query", "lambda shipping_query: shipping_query.from_user.id == xyz"),
     PRE_CHECKOUT_QUERY_MANAGER : ("pre_checkout_query", "lambda pre_checkout_query: pre_checkout_query.from_user.id == xyz"),
```

### Comparing `aiotgm-0.2.9/aiotgm/utils.py` & `aiotgm-0.3.0/aiotgm/utils.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.2.9/aiotgm.egg-info/PKG-INFO` & `aiotgm-0.3.0/aiotgm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgm
-Version: 0.2.9
+Version: 0.3.0
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `aiotgm-0.2.9/tests/test_func_ok.py` & `aiotgm-0.3.0/tests/test_func_ok.py`

 * *Files identical despite different names*


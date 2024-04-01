# Comparing `tmp/melobot-2.5.8.tar.gz` & `tmp/melobot-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melobot-2.5.8.tar", last modified: Sun Mar 31 16:28:12 2024, max compression
+gzip compressed data, was "melobot-2.5.9.tar", last modified: Mon Apr  1 16:24:16 2024, max compression
```

## Comparing `melobot-2.5.8.tar` & `melobot-2.5.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    34503 2024-01-15 15:39:44.000000 melobot-2.5.8/LICENSE
--rw-r--r--   0        0        0     4338 2024-03-31 16:25:02.553199 melobot-2.5.8/README.md
--rw-r--r--   0        0        0     1752 2024-03-31 16:28:12.147549 melobot-2.5.8/pyproject.toml
--rw-r--r--   0        0        0      862 2024-03-30 08:38:36.033575 melobot-2.5.8/src/melobot/__init__.py
--rw-r--r--   0        0        0      345 2024-03-24 14:31:23.666726 melobot-2.5.8/src/melobot/base/__init__.py
--rw-r--r--   0        0        0    17292 2024-03-29 15:06:55.286596 melobot-2.5.8/src/melobot/base/abc.py
--rw-r--r--   0        0        0     3057 2024-03-24 15:02:59.473829 melobot-2.5.8/src/melobot/base/exceptions.py
--rw-r--r--   0        0        0    20554 2024-03-24 16:05:55.234406 melobot-2.5.8/src/melobot/base/tools.py
--rw-r--r--   0        0        0     3550 2024-03-31 12:34:47.915775 melobot-2.5.8/src/melobot/base/typing.py
--rw-r--r--   0        0        0      272 2024-03-22 11:40:21.563163 melobot-2.5.8/src/melobot/bot/__init__.py
--rw-r--r--   0        0        0     2271 2024-03-29 11:31:37.416494 melobot-2.5.8/src/melobot/bot/hook.py
--rw-r--r--   0        0        0    17096 2024-03-29 15:06:55.239721 melobot-2.5.8/src/melobot/bot/init.py
--rw-r--r--   0        0        0     1274 2024-03-31 06:44:58.283526 melobot-2.5.8/src/melobot/context/__init__.py
--rw-r--r--   0        0        0    45501 2024-03-31 13:59:28.878887 melobot-2.5.8/src/melobot/context/action.py
--rw-r--r--   0        0        0    21573 2024-03-31 06:44:58.266878 melobot-2.5.8/src/melobot/context/session.py
--rw-r--r--   0        0        0        0 2024-03-08 13:14:49.000000 melobot-2.5.8/src/melobot/controller/__init__.py
--rw-r--r--   0        0        0     4089 2024-03-29 11:33:02.553255 melobot-2.5.8/src/melobot/controller/dispatcher.py
--rw-r--r--   0        0        0     2868 2024-03-22 17:43:07.375990 melobot-2.5.8/src/melobot/controller/responder.py
--rw-r--r--   0        0        0      178 2024-03-29 13:09:27.562534 melobot-2.5.8/src/melobot/io/__init__.py
--rw-r--r--   0        0        0     6880 2024-03-29 17:25:35.066236 melobot-2.5.8/src/melobot/io/forward_ws.py
--rw-r--r--   0        0        0     8413 2024-03-29 17:26:29.606330 melobot-2.5.8/src/melobot/io/full_duplex_http.py
--rw-r--r--   0        0        0     8140 2024-03-29 17:27:23.530647 melobot-2.5.8/src/melobot/io/reverse_ws.py
--rw-r--r--   0        0        0     2138 2024-03-31 16:04:30.399591 melobot-2.5.8/src/melobot/meta.py
--rw-r--r--   0        0        0      610 2024-03-31 12:29:02.222202 melobot-2.5.8/src/melobot/models/__init__.py
--rw-r--r--   0        0        0    14758 2024-03-31 12:28:49.011197 melobot-2.5.8/src/melobot/models/cq.py
--rw-r--r--   0        0        0    29618 2024-03-31 10:37:41.437038 melobot-2.5.8/src/melobot/models/event.py
--rw-r--r--   0        0        0       57 2024-03-23 10:16:23.231515 melobot-2.5.8/src/melobot/plugin/__init__.py
--rw-r--r--   0        0        0    13479 2024-03-29 11:33:53.159440 melobot-2.5.8/src/melobot/plugin/handler.py
--rw-r--r--   0        0        0    47561 2024-03-24 14:32:04.789847 melobot-2.5.8/src/melobot/plugin/init.py
--rw-r--r--   0        0        0     6342 2024-03-29 11:34:09.731812 melobot-2.5.8/src/melobot/plugin/ipc.py
--rw-r--r--   0        0        0      831 2024-03-24 13:38:01.396871 melobot-2.5.8/src/melobot/utils/__init__.py
--rw-r--r--   0        0        0    12812 2024-03-24 13:41:52.092688 melobot-2.5.8/src/melobot/utils/checker.py
--rw-r--r--   0        0        0     7413 2024-03-24 13:43:51.387417 melobot-2.5.8/src/melobot/utils/formatter.py
--rw-r--r--   0        0        0     8373 2024-03-27 07:27:30.028945 melobot-2.5.8/src/melobot/utils/logger.py
--rw-r--r--   0        0        0     4442 2024-03-27 07:12:29.469637 melobot-2.5.8/src/melobot/utils/matcher.py
--rw-r--r--   0        0        0     7000 2024-03-24 13:42:40.253742 melobot-2.5.8/src/melobot/utils/parser.py
--rw-r--r--   0        0        0        0 2024-03-12 08:09:26.000000 melobot-2.5.8/tests/__init__.py
--rw-r--r--   0        0        0   292545 2024-03-04 13:21:47.000000 melobot-2.5.8/tests/private/2939fc304d7d88447f460b76aa9d7199.jpeg
--rw-r--r--   0        0        0      629 2024-03-31 14:20:46.827086 melobot-2.5.8/tests/private/TODO.txt
--rw-r--r--   0        0        0        0 2024-03-12 06:35:00.000000 melobot-2.5.8/tests/private/__init__.py
--rw-r--r--   0        0        0     1473 2024-03-11 05:30:20.000000 melobot-2.5.8/tests/private/__main__.py
--rw-r--r--   0        0        0      346 2024-03-31 13:29:23.457942 melobot-2.5.8/tests/private/app.py
--rw-r--r--   0        0        0     1017 2024-03-16 09:34:42.134229 melobot-2.5.8/tests/private/main.py
--rw-r--r--   0        0        0       83 2024-03-14 14:54:02.701829 melobot-2.5.8/tests/private/meta.py
--rw-r--r--   0        0        0    92007 2024-03-08 13:06:33.000000 melobot-2.5.8/tests/private/output.png
--rw-r--r--   0        0        0    16272 2024-03-08 13:06:56.000000 melobot-2.5.8/tests/private/output.svg
--rw-r--r--   0        0        0     1942 2024-01-15 15:39:47.000000 melobot-2.5.8/tests/private/procedure.txt
--rw-r--r--   0        0        0     4150 2024-02-27 06:31:28.000000 melobot-2.5.8/tests/private/qjson.json
--rw-r--r--   0        0        0     9254 2024-01-13 14:01:16.000000 melobot-2.5.8/tests/private/templates/draw.py
--rw-r--r--   0        0        0     8308 2024-03-05 15:50:37.000000 melobot-2.5.8/tests/private/templates/sdapi/api.py
--rw-r--r--   0        0        0     1898 2024-01-13 14:01:16.000000 melobot-2.5.8/tests/private/templates/sdapi/api_help.py
--rw-r--r--   0        0        0      350 2024-01-13 14:39:21.000000 melobot-2.5.8/tests/private/templates/sdapi/config.json
--rw-r--r--   0        0        0     1306 2024-01-13 14:48:03.000000 melobot-2.5.8/tests/private/templates/sdapi/sd_test.py
--rw-r--r--   0        0        0   389862 2024-01-13 14:48:27.000000 melobot-2.5.8/tests/private/templates/sdapi/test.png
--rw-r--r--   0        0        0      735 2024-03-31 09:31:14.301196 melobot-2.5.8/tests/private/test.py
--rw-r--r--   0        0        0        0 2024-03-17 12:12:19.817029 melobot-2.5.8/tests/private/test2/test2.py
--rw-r--r--   0        0        0     4848 1970-01-01 00:00:00.000000 melobot-2.5.8/PKG-INFO
+-rw-r--r--   0        0        0    34503 2024-01-15 15:39:44.000000 melobot-2.5.9/LICENSE
+-rw-r--r--   0        0        0     4338 2024-03-31 16:25:02.553199 melobot-2.5.9/README.md
+-rw-r--r--   0        0        0     1752 2024-04-01 16:24:16.306867 melobot-2.5.9/pyproject.toml
+-rw-r--r--   0        0        0      865 2024-04-01 09:45:08.891326 melobot-2.5.9/src/melobot/__init__.py
+-rw-r--r--   0        0        0      408 2024-04-01 09:52:40.319649 melobot-2.5.9/src/melobot/base/__init__.py
+-rw-r--r--   0        0        0    19147 2024-04-01 09:50:48.245464 melobot-2.5.9/src/melobot/base/abc.py
+-rw-r--r--   0        0        0     3057 2024-03-24 15:02:59.473829 melobot-2.5.9/src/melobot/base/exceptions.py
+-rw-r--r--   0        0        0    20554 2024-03-24 16:05:55.234406 melobot-2.5.9/src/melobot/base/tools.py
+-rw-r--r--   0        0        0     3701 2024-04-01 13:47:08.533874 melobot-2.5.9/src/melobot/base/typing.py
+-rw-r--r--   0        0        0      272 2024-03-22 11:40:21.563163 melobot-2.5.9/src/melobot/bot/__init__.py
+-rw-r--r--   0        0        0     2271 2024-03-29 11:31:37.416494 melobot-2.5.9/src/melobot/bot/hook.py
+-rw-r--r--   0        0        0    17096 2024-03-29 15:06:55.239721 melobot-2.5.9/src/melobot/bot/init.py
+-rw-r--r--   0        0        0     1274 2024-03-31 06:44:58.283526 melobot-2.5.9/src/melobot/context/__init__.py
+-rw-r--r--   0        0        0    52218 2024-04-01 13:47:08.299419 melobot-2.5.9/src/melobot/context/action.py
+-rw-r--r--   0        0        0    21558 2024-04-01 10:29:13.862731 melobot-2.5.9/src/melobot/context/session.py
+-rw-r--r--   0        0        0        0 2024-03-08 13:14:49.000000 melobot-2.5.9/src/melobot/controller/__init__.py
+-rw-r--r--   0        0        0     4088 2024-04-01 10:26:53.805900 melobot-2.5.9/src/melobot/controller/dispatcher.py
+-rw-r--r--   0        0        0     2868 2024-03-22 17:43:07.375990 melobot-2.5.9/src/melobot/controller/responder.py
+-rw-r--r--   0        0        0      178 2024-03-29 13:09:27.562534 melobot-2.5.9/src/melobot/io/__init__.py
+-rw-r--r--   0        0        0     6880 2024-03-29 17:25:35.066236 melobot-2.5.9/src/melobot/io/forward_ws.py
+-rw-r--r--   0        0        0     8407 2024-04-01 09:59:01.581195 melobot-2.5.9/src/melobot/io/full_duplex_http.py
+-rw-r--r--   0        0        0     8140 2024-03-29 17:27:23.530647 melobot-2.5.9/src/melobot/io/reverse_ws.py
+-rw-r--r--   0        0        0     2138 2024-04-01 16:20:25.582825 melobot-2.5.9/src/melobot/meta.py
+-rw-r--r--   0        0        0      632 2024-04-01 14:41:10.447540 melobot-2.5.9/src/melobot/models/__init__.py
+-rw-r--r--   0        0        0    29545 2024-04-01 14:14:06.936706 melobot-2.5.9/src/melobot/models/event.py
+-rw-r--r--   0        0        0    15492 2024-04-01 14:41:47.118818 melobot-2.5.9/src/melobot/models/msg.py
+-rw-r--r--   0        0        0       84 2024-04-01 09:16:35.320891 melobot-2.5.9/src/melobot/plugin/__init__.py
+-rw-r--r--   0        0        0    13475 2024-04-01 09:42:14.940667 melobot-2.5.9/src/melobot/plugin/handler.py
+-rw-r--r--   0        0        0    46097 2024-04-01 10:35:35.422279 melobot-2.5.9/src/melobot/plugin/init.py
+-rw-r--r--   0        0        0     6341 2024-04-01 10:31:40.886052 melobot-2.5.9/src/melobot/plugin/ipc.py
+-rw-r--r--   0        0        0      837 2024-04-01 09:45:09.215509 melobot-2.5.9/src/melobot/utils/__init__.py
+-rw-r--r--   0        0        0    12808 2024-04-01 13:56:11.714821 melobot-2.5.9/src/melobot/utils/checker.py
+-rw-r--r--   0        0        0     7416 2024-04-01 09:45:09.199967 melobot-2.5.9/src/melobot/utils/formatter.py
+-rw-r--r--   0        0        0     8356 2024-04-01 10:37:47.251674 melobot-2.5.9/src/melobot/utils/logger.py
+-rw-r--r--   0        0        0     4442 2024-03-27 07:12:29.469637 melobot-2.5.9/src/melobot/utils/matcher.py
+-rw-r--r--   0        0        0     7033 2024-04-01 09:55:20.362795 melobot-2.5.9/src/melobot/utils/parser.py
+-rw-r--r--   0        0        0        0 2024-03-12 08:09:26.000000 melobot-2.5.9/tests/__init__.py
+-rw-r--r--   0        0        0   292545 2024-03-04 13:21:47.000000 melobot-2.5.9/tests/private/2939fc304d7d88447f460b76aa9d7199.jpeg
+-rw-r--r--   0        0        0      631 2024-04-01 12:17:17.605631 melobot-2.5.9/tests/private/TODO.txt
+-rw-r--r--   0        0        0        0 2024-03-12 06:35:00.000000 melobot-2.5.9/tests/private/__init__.py
+-rw-r--r--   0        0        0     1473 2024-03-11 05:30:20.000000 melobot-2.5.9/tests/private/__main__.py
+-rw-r--r--   0        0        0      346 2024-03-31 13:29:23.457942 melobot-2.5.9/tests/private/app.py
+-rw-r--r--   0        0        0     1017 2024-03-16 09:34:42.134229 melobot-2.5.9/tests/private/main.py
+-rw-r--r--   0        0        0       83 2024-03-14 14:54:02.701829 melobot-2.5.9/tests/private/meta.py
+-rw-r--r--   0        0        0    92007 2024-03-08 13:06:33.000000 melobot-2.5.9/tests/private/output.png
+-rw-r--r--   0        0        0    16272 2024-03-08 13:06:56.000000 melobot-2.5.9/tests/private/output.svg
+-rw-r--r--   0        0        0     1942 2024-01-15 15:39:47.000000 melobot-2.5.9/tests/private/procedure.txt
+-rw-r--r--   0        0        0     4150 2024-02-27 06:31:28.000000 melobot-2.5.9/tests/private/qjson.json
+-rw-r--r--   0        0        0     9254 2024-01-13 14:01:16.000000 melobot-2.5.9/tests/private/templates/draw.py
+-rw-r--r--   0        0        0     8308 2024-03-05 15:50:37.000000 melobot-2.5.9/tests/private/templates/sdapi/api.py
+-rw-r--r--   0        0        0     1898 2024-01-13 14:01:16.000000 melobot-2.5.9/tests/private/templates/sdapi/api_help.py
+-rw-r--r--   0        0        0      350 2024-01-13 14:39:21.000000 melobot-2.5.9/tests/private/templates/sdapi/config.json
+-rw-r--r--   0        0        0     1306 2024-01-13 14:48:03.000000 melobot-2.5.9/tests/private/templates/sdapi/sd_test.py
+-rw-r--r--   0        0        0   389862 2024-01-13 14:48:27.000000 melobot-2.5.9/tests/private/templates/sdapi/test.png
+-rw-r--r--   0        0        0      735 2024-03-31 09:31:14.301196 melobot-2.5.9/tests/private/test.py
+-rw-r--r--   0        0        0        0 2024-03-17 12:12:19.817029 melobot-2.5.9/tests/private/test2/test2.py
+-rw-r--r--   0        0        0     4848 1970-01-01 00:00:00.000000 melobot-2.5.9/PKG-INFO
```

### Comparing `melobot-2.5.8/LICENSE` & `melobot-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/README.md` & `melobot-2.5.9/README.md`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/pyproject.toml` & `melobot-2.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "melobot"
-version = "2.5.8"
+version = "2.5.9"
 description = "A qq bot development framework with friendly APIs, session control and plugin-supported."
 authors = [
     { name = "aicorein", email = "melodyecho@glowmem.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "uvloop>=0.17.0; platform_system==\"Linux\"",
```

### Comparing `melobot-2.5.8/src/melobot/__init__.py` & `melobot-2.5.9/src/melobot/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     send_reply,
     send_wait,
 )
 from .io import ForwardWsConn, HttpConn, ReverseWsConn
 from .meta import MetaInfo
 from .plugin import BotPlugin
 from .utils import (
-    ArgFormatter,
     AtChecker,
+    CmdArgFormatter,
     CmdParser,
     CmdParserGen,
     GroupMsgLvlChecker,
     MsgCheckerGen,
     PrivateMsgLvlChecker,
 )
```

### Comparing `melobot-2.5.8/src/melobot/base/abc.py` & `melobot-2.5.9/src/melobot/base/abc.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,35 +24,36 @@
     ParseArgs,
     Type,
     Void,
     VoidType,
 )
 
 if TYPE_CHECKING:
+    import logging
+
     from ..bot.hook import BotHookBus
     from ..controller.dispatcher import BotDispatcher
     from ..controller.responder import BotResponder
     from ..models.event import BotEventBuilder
     from ..plugin.handler import EventHandler
-    from ..utils.logger import Logger
 
 
 class AbstractConnector(ABC):
     """抽象连接器类
 
     .. admonition:: 提示
        :class: tip
 
        一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
     """
 
     def __init__(self, cd_time: float) -> None:
         super().__init__()
         #: 连接器的日志器
-        self.logger: "Logger"
+        self.logger: "logging.Logger"
         #: 是否在 slack 状态
         self.slack: bool = False
         #: 连接器发送行为操作的冷却时间
         self.cd_time = cd_time
 
         self._ref_flag: bool = False
         self._ready_signal = asyncio.Event()
@@ -82,15 +83,15 @@
 
     def _bind(
         self,
         dispatcher: "BotDispatcher",
         responder: "BotResponder",
         event_builder: Type["BotEventBuilder"],
         bot_bus: "BotHookBus",
-        logger: "Logger",
+        logger: "logging.Logger",
     ) -> None:
         self._event_builder = event_builder
         self._bot_bus = bot_bus
         self.logger = logger
         self._common_dispatcher = dispatcher
         self._resp_dispatcher = responder
 
@@ -145,15 +146,15 @@
 
        一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
     """
 
     def __init__(self, rawEvent: dict) -> None:
         super().__init__()
         #: 从 onebot 实现项目获得的未格式化的事件
-        self.raw = rawEvent
+        self.raw: dict = rawEvent
         self._args_map: Optional[dict[Any, dict[str, ParseArgs] | None]] = None
 
     @abstractproperty
     def time(self) -> int:
         """事件发生的时间"""
         pass
 
@@ -184,19 +185,19 @@
 
     def _get_args(self, parser_id: Any) -> dict[str, ParseArgs] | VoidType | None:
         if self._args_map is None:
             return Void
         return self._args_map.get(parser_id, Void)
 
     def _store_args(
-        self, parser_id: Any, args_group: dict[str, ParseArgs] | None
+        self, parser_id: Any, args_dict: dict[str, ParseArgs] | None
     ) -> None:
         if self._args_map is None:
             self._args_map = {}
-        self._args_map[parser_id] = args_group
+        self._args_map[parser_id] = args_dict
 
 
 class ActionArgs(ABC):
     # 行为信息构造基类
 
     def __init__(self) -> None:
         super().__init__()
@@ -219,22 +220,21 @@
         self,
         action_args: ActionArgs,
         resp_id: Optional[str] = None,
         triggerEvent: Optional[BotEvent] = None,
         ready: bool = False,
     ) -> None:
         super().__init__()
-        #: 响应标识 id。只有选择等待响应时，才会生成 id
         self.resp_id = resp_id
         #: 行为类型。对应 onebot 标准中的 API 终结点名称
-        self.type = action_args.type
+        self.type: str = action_args.type
         #: 行为参数。对应 onebot 标准中向 API 传送的数据的 params 字段
-        self.params = action_args.params
+        self.params: dict = action_args.params
         #: 行为的触发事件，一般是行为生成时所在会话的事件
-        self.trigger = triggerEvent
+        self.trigger: Optional[BotEvent] = triggerEvent
 
         self._ready = ready
 
     def extract(self) -> dict:
         # 从对象提取标准 cq action dict
         obj = {
             "action": self.type,
@@ -522,27 +522,69 @@
             self.mode,
             self.m1.match(text),
             self.m2.match(text) if self.m2 is not None else None,
         )
 
 
 class BotParser(ABC):
-    # 解析器基类。解析器一般用作从消息文本中按规则提取指定字符串或字符串组合
+    """解析器基类
+
+    解析器一般用作从消息文本中按规则批量提取参数
+    """
 
     def __init__(self, id: Any) -> None:
+        """初始化一个解析器
+
+        :param id: 解析器解析规则的标识
+
+           id 相同，意味着解析规则相同。一组解析规则相同的解析器，只有第一个会实际运行解析。其他后续解析器会复用这个解析结果。
+
+           id 标识存在的意义是增强复用性。如果你不需要复用，id 值给定不同的随机值即可。
+        """
         super().__init__()
-        self.id = id
+        #: 解析器的 id，即解析规则的表示
+        self.id: Any = id
+        #: 是否需要格式化（此属性可在继承后进行修改，若为否，则不再进行格式化）
         self.need_format: bool = False
 
     @abstractmethod
     def parse(self, text: str) -> Optional[dict[str, ParseArgs]]:
+        """解析方法
+
+        任何解析器应该实现此抽象方法
+
+        :param text: 消息文本内容
+        :return: 解析结果
+
+           因为一次解析可能会得到多组结果，结果为字典或空值。字典键为一组解析结果的识别标志（例如命令解析中的命令名），值为解析参数对象（象征一组解析结果）
+        """
         pass
 
     @abstractmethod
     def test(
-        self, args_group: dict[str, ParseArgs] | None
+        self, args_dict: Optional[dict[str, ParseArgs]]
     ) -> tuple[bool, Optional[str], Optional[ParseArgs]]:
+        """解析测试方法
+
+        任何解析器应该实现此抽象方法
+
+        :param args_dict: 之前的解析结果
+        :return: 返回元组：(判断是否解析成功, 可为空的一组解析结果的识别标志, 可为空的解析参数对象)
+        """
         pass
 
     @abstractmethod
-    async def format(self, cmd_name: str, args: ParseArgs) -> bool:
+    async def format(self, group_id: str, args: ParseArgs) -> bool:
+        """格式化方法
+
+        任何解析器应该实现此抽象方法
+
+        格式化是否进行，会受解析器 `need_fotmat` 参数和 :meth:`~.BotParser.test` 的影响。
+        如果你确定你的解析器子类 100% 不需要格式化，那么继承这个方法再次标记为 pass 即可。
+
+        格式化过程最后只返回是否格式化成功，格式化的结果将会被直接保存，并可通过 :func:`.msg_args` 获得。
+
+        :param group_id: 一组解析结果的识别标志
+        :param args: 解析参数对象
+        :return: 格式化是否成功
+        """
         pass
```

### Comparing `melobot-2.5.8/src/melobot/base/exceptions.py` & `melobot-2.5.9/src/melobot/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/src/melobot/base/tools.py` & `melobot-2.5.9/src/melobot/base/tools.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/src/melobot/base/typing.py` & `melobot-2.5.9/src/melobot/base/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,49 +25,53 @@
 
 # 修复在 windows powershell 显示错误的 bug
 better_exceptions.encoding.ENCODING = sys.stdout.encoding
 better_exceptions.formatter.ENCODING = sys.stdout.encoding
 better_exceptions.hook()
 
 
-class CQMsgDict(TypedDict):
+class MsgSegment(TypedDict):
     """onebot 标准的消息段对象"""
 
     type: str
     data: dict[str, float | int | str]
 
 
 class CustomNodeData(TypedDict):
     """onebot 标准的自定义消息结点数据"""
 
     name: str
     uin: str
-    content: list[CQMsgDict]
-    seq: NotRequired[list[CQMsgDict]]
+    content: list[MsgSegment]
+    seq: NotRequired[list[MsgSegment]]
 
 
 class ReferNodeData(TypedDict):
     """onebot 标准的引用消息结点数据"""
 
     id: str
 
 
-class MsgNodeDict(TypedDict):
+class MsgNode(TypedDict):
     """onebot 标准的转发消息结点"""
 
     type: Literal["node"]
     data: CustomNodeData | ReferNodeData
 
 
 class ParseArgs:
-    # 命令参数类
+    """命令参数类"""
 
     def __init__(self, values: list[Any] | None) -> None:
-        self.vals = values
-        self.formatted = False
+        """实例化一组命令参数，对应一次解析的结果
+
+        :param values: 参数值
+        """
+        #: 保存的一组命令参数值
+        self.vals: Optional[list[Any]] = values
 
 
 class LogicMode(Enum):
     """逻辑模式枚举类型"""
 
     AND = 1
     OR = 2
@@ -111,15 +115,15 @@
     SU = 1000
     WHITE = 100
     USER = 10
     BLACK = -1
 
 
 class PriorLevel(int, Enum):
-    """事件处理器优先级枚举
+    """事件处理优先级枚举
 
     为方便进行优先级设置，有 MIN, MAX, MEAN 三个枚举值
     """
 
     MIN = 0
     MAX = 1000
     MEAN = (MAX + MIN) // 2
```

### Comparing `melobot-2.5.8/src/melobot/bot/hook.py` & `melobot-2.5.9/src/melobot/bot/hook.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/src/melobot/bot/init.py` & `melobot-2.5.9/src/melobot/bot/init.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/src/melobot/context/__init__.py` & `melobot-2.5.9/src/melobot/context/__init__.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/src/melobot/context/action.py` & `melobot-2.5.9/src/melobot/context/action.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import warnings
 
 from ..base.abc import ActionArgs, BotAction, BotEvent
 from ..base.exceptions import BotActionError, BotSessionError, DirectRetSignal
 from ..base.tools import get_id
-from ..base.typing import TYPE_CHECKING, CQMsgDict, Literal, MsgNodeDict, Optional
-from ..models.cq import _to_cq_str_action, reply_msg, text_msg
+from ..base.typing import TYPE_CHECKING, Literal, MsgNode, MsgSegment, Optional, Union
+from ..models.msg import _to_cq_str_action, reply_msg, text_msg
 from .session import SESSION_LOCAL
 from .session import BotSessionManager as CtxManager
 
 if TYPE_CHECKING:
     from ..models.event import ResponseEvent
 
 __all__ = (
@@ -53,15 +53,15 @@
 
 
 class MsgActionArgs(ActionArgs):
     """消息 action 信息构造类."""
 
     def __init__(
         self,
-        msgs: list[CQMsgDict],
+        msgs: list[MsgSegment],
         isPrivate: bool,
         userId: Optional[int] = None,
         groupId: Optional[int] = None,
     ) -> None:
         super().__init__()
         self.type = "send_msg"
         if isPrivate:
@@ -75,15 +75,15 @@
                 "message_type": "group",
                 "user_id": userId,
                 "group_id": groupId,
                 "message": msgs,
             }
 
 
-def _process_msg(content: str | CQMsgDict | list[CQMsgDict]) -> list[CQMsgDict]:
+def _process_msg(content: str | MsgSegment | list[MsgSegment]) -> list[MsgSegment]:
     """将多种可能的消息格式，统一转换为 cq 消息列表."""
     if isinstance(content, str):
         _ = text_msg(content)
         if not isinstance(_, list):
             msgs = [_]
     elif isinstance(content, dict):
         msgs = [content]
@@ -98,15 +98,15 @@
     else:
         raise BotActionError("content 参数类型不正确，无法封装")
     return msgs
 
 
 @CtxManager._activate
 async def send_custom_msg(
-    content: str | CQMsgDict | list[CQMsgDict],
+    content: str | MsgSegment | list[MsgSegment],
     isPrivate: bool,
     userId: Optional[int] = None,
     groupId: Optional[int] = None,
     cq_str: bool = False,
     wait: bool = False,
     auto: bool = True,
 ) -> BotAction:
@@ -117,22 +117,25 @@
 
        当启用了 `cq_str` 选项，且 `content` 参数为字符串时，
        `content` 字符串将不会被处理为消息段对象，此时字符串中的 cq 码将会直接生效，而不是被转义。
 
     .. admonition:: 警告
        :class: attention
 
-       这个小技巧可以让你发送有效的 cq 码字符串。但是存在潜在的安全问题：
-       如果将用户输入作为 cq 码字符串的一部分发送出去，这将会造成“注入攻击”！
-       用户可以构造包含恶意图片、语音的 cq 码，让 bot 发送。
+       这个小技巧可以让你直接发送 CQ 码字符串。但是存在潜在的安全问题：
+       如果将用户输入作为 CQ 码字符串的一部分发送出去，这将会造成“注入攻击”！
+       用户可以构造包含恶意图片、语音的 CQ 码，让 bot 发送。
 
        任何时候启用 `cq_str` 选项，如需用到用户输入，务必校验。
 
     此接口合并了 onebot 标准中的私聊消息发送、群聊消息发送接口。
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-2 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-2>`_
+
     :param content: 发送内容
     :param isPrivate: 是否是私聊
     :param userId: 如果是私聊，传入目标 qq 号；群聊置空即可
     :param groupId: 如果是群聊，传入群号；私聊置空即可
     :param cq_str: 是否以 cq 字符串发送（默认格式是消息段对象)
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
@@ -155,15 +158,15 @@
     if cq_str:
         action = _to_cq_str_action(action)
     return action
 
 
 @CtxManager._activate
 async def send(
-    content: str | CQMsgDict | list[CQMsgDict],
+    content: str | MsgSegment | list[MsgSegment],
     cq_str: bool = False,
     wait: bool = False,
     auto: bool = True,
 ) -> BotAction:
     """发送消息（在当前会话下自动定位发送目标）
 
     .. admonition:: 小技巧
@@ -171,20 +174,23 @@
 
        当启用了 `cq_str` 选项，且 `content` 参数为字符串时，
        `content` 字符串将不会被处理为消息段对象，此时字符串中的 cq 码将会直接生效，而不是被转义。
 
     .. admonition:: 警告
        :class: attention
 
-       这个小技巧可以让你发送有效的 cq 码字符串。但是存在潜在的安全问题：
-       如果将用户输入作为 cq 码字符串的一部分发送出去，这将会造成“注入攻击”！
-       用户可以构造包含恶意图片、语音的 cq 码，让 bot 发送。
+       这个小技巧可以让你直接发送 CQ 码字符串。但是存在潜在的安全问题：
+       如果将用户输入作为 CQ 码字符串的一部分发送出去，这将会造成“注入攻击”！
+       用户可以构造包含恶意图片、语音的 CQ 码，让 bot 发送。
 
        任何时候启用 `cq_str` 选项，如需用到用户输入，务必校验。
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-2 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-2>`_
+
     :param content: 发送内容（可以是文本、消息段对象、消息段对象列表）
     :param cq_str: 是否以 cq 字符串发送（默认格式是消息段对象)
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
@@ -212,15 +218,15 @@
 
 
 class ForwardMsgActionArgs(ActionArgs):
     """转发消息 action 信息构造类."""
 
     def __init__(
         self,
-        msgs: list[MsgNodeDict],
+        msgs: list[MsgNode],
         isPrivate: bool,
         userId: Optional[int] = None,
         groupId: Optional[int] = None,
     ) -> None:
         super().__init__()
         if isPrivate:
             self.type = "send_private_forward_msg"
@@ -228,15 +234,15 @@
         else:
             self.type = "send_group_forward_msg"
             self.params = {"group_id": groupId, "messages": msgs, "auto_escape": True}
 
 
 @CtxManager._activate
 async def send_custom_forward(
-    msgNodes: list[MsgNodeDict],
+    msgNodes: list[MsgNode],
     isPrivate: bool,
     userId: Optional[int] = None,
     groupId: Optional[int] = None,
     cq_str: bool = False,
     wait: bool = False,
     auto: bool = True,
 ) -> BotAction:
@@ -247,20 +253,29 @@
 
        当启用了 `cq_str` 选项，且 `content` 参数为字符串时，
        `content` 字符串将不会被处理为消息段对象，此时字符串中的 cq 码将会直接生效，而不是被转义。
 
     .. admonition:: 警告
        :class: attention
 
-       这个小技巧可以让你发送有效的 cq 码字符串。但是存在潜在的安全问题：
-       如果将用户输入作为 cq 码字符串的一部分发送出去，这将会造成“注入攻击”！
-       用户可以构造包含恶意图片、语音的 cq 码，让 bot 发送。
+       这个小技巧可以让你直接发送 CQ 码字符串。但是存在潜在的安全问题：
+       如果将用户输入作为 CQ 码字符串的一部分发送出去，这将会造成“注入攻击”！
+       用户可以构造包含恶意图片、语音的 CQ 码，让 bot 发送。
 
        任何时候启用 `cq_str` 选项，如需用到用户输入，务必校验。
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+
+    .. code:: python
+
+       {
+           "message_id": xxx,  # int
+           "forward_id": xxx   # str
+       }
+
     :param msgNodes: 消息结点列表
     :param isPrivate: 是否是私聊
     :param userId: 如果是私聊，传入目标 qq 号；群聊置空即可
     :param groupId: 如果是群聊，传入群号；私聊置空即可
     :param cq_str: 是否以 cq 字符串发送（默认格式是消息段对象)
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
@@ -279,15 +294,15 @@
     if cq_str:
         action = _to_cq_str_action(action)
     return action
 
 
 @CtxManager._activate
 async def send_forward(
-    msgNodes: list[MsgNodeDict],
+    msgNodes: list[MsgNode],
     cq_str: bool = False,
     wait: bool = False,
     auto: bool = True,
 ) -> BotAction:
     """发送转发消息（在当前会话下自动定位发送目标）
 
     .. admonition:: 小技巧
@@ -295,20 +310,29 @@
 
        当启用了 `cq_str` 选项，且 `content` 参数为字符串时，
        `content` 字符串将不会被处理为消息段对象，此时字符串中的 cq 码将会直接生效，而不是被转义。
 
     .. admonition:: 警告
        :class: attention
 
-       这个小技巧可以让你发送有效的 cq 码字符串。但是存在潜在的安全问题：
-       如果将用户输入作为 cq 码字符串的一部分发送出去，这将会造成“注入攻击”！
-       用户可以构造包含恶意图片、语音的 cq 码，让 bot 发送。
+       这个小技巧可以让你直接发送 CQ 码字符串。但是存在潜在的安全问题：
+       如果将用户输入作为 CQ 码字符串的一部分发送出去，这将会造成“注入攻击”！
+       用户可以构造包含恶意图片、语音的 CQ 码，让 bot 发送。
 
        任何时候启用 `cq_str` 选项，如需用到用户输入，务必校验。
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+
+    .. code:: python
+
+       {
+           "message_id": xxx,  # int
+           "forward_id": xxx   # str
+       }
+
     :param msgNodes: 消息结点列表
     :param cq_str: 是否以 cq 字符串发送（默认格式是消息段对象)
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
@@ -346,14 +370,17 @@
         }
 
 
 @CtxManager._activate
 async def msg_recall(msgId: int, wait: bool = False, auto: bool = True) -> BotAction:
     """撤回消息
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-3 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-3>`_
+
     :param msgId: 消息 id
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
        `auto=True, wait=True` -> :class:`.ResponseEvent` 对象
@@ -374,14 +401,17 @@
         self.params = {"message_id": msgId}
 
 
 @CtxManager._activate
 async def get_msg(msgId: int, wait: bool = True, auto: bool = True) -> BotAction:
     """获取消息详细信息
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-4 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-4>`_
+
     :param msgId: 消息 id
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
        `auto=True, wait=True` -> :class:`.ResponseEvent` 对象
@@ -395,23 +425,26 @@
 
 class getForwardActionArgs(ActionArgs):
     """转发消息获取 action 信息构造类."""
 
     def __init__(self, forwardId: str) -> None:
         super().__init__()
         self.type = "get_forward_msg"
-        self.params = {"message_id": forwardId}
+        self.params = {"id": forwardId}
 
 
 @CtxManager._activate
 async def get_forward_msg(
     forwardId: str, wait: bool = True, auto: bool = True
 ) -> BotAction:
     """获取转发消息的详细信息
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-5 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-5>`_
+
     :param forwardId: 转发 id
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
        `auto=True, wait=True` -> :class:`.ResponseEvent` 对象
@@ -432,14 +465,17 @@
         self.params = {"file": fileName}
 
 
 @CtxManager._activate
 async def get_image(fileName: str, wait: bool = True, auto: bool = True) -> BotAction:
     """获取图片信息
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-31 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-31>`_
+
     :param fileName: 图片文件名
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
        `auto=True, wait=True` -> :class:`.ResponseEvent` 对象
@@ -462,14 +498,17 @@
 
 @CtxManager._activate
 async def send_like(
     userId: int, times: int = 1, wait: bool = False, auto: bool = True
 ) -> BotAction:
     """发送好友赞
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-6 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-6>`_
+
     :param userId: qq 号
     :param times: 赞的数量，默认为 1，每天最多 10
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
@@ -503,14 +542,17 @@
     userId: int,
     laterReject: bool = False,
     wait: bool = False,
     auto: bool = True,
 ) -> BotAction:
     """群组踢人
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-7 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-7>`_
+
     :param groupId: 群号
     :param userId: 被踢的 qq 号
     :param laterReject: 是否拒绝此人再次加群
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
@@ -541,14 +583,17 @@
 
 @CtxManager._activate
 async def group_ban(
     groupId: int, userId: int, duration: int, wait: bool = False, auto: bool = True
 ) -> BotAction:
     """群组禁言
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-8 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-8>`_
+
     :param groupId: 群号
     :param userId: 禁言的 qq 号
     :param duration: 禁言时长，为 0 则表示取消禁言
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
@@ -575,14 +620,17 @@
 
 @CtxManager._activate
 async def group_whole_ban(
     groupId: int, enable: bool, wait: bool = False, auto: bool = True
 ) -> BotAction:
     """群组全员禁言
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-10 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-10>`_
+
     :param groupId: 群号
     :param enable: 是则禁言，否则取消禁言
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
@@ -608,14 +656,17 @@
 
 @CtxManager._activate
 async def set_group_admin(
     groupId: int, userId: int, enable: bool, wait: bool = False, auto: bool = True
 ) -> BotAction:
     """设置群管理员
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-11 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-11>`_
+
     :param groupId: 群号
     :param userId: 设置的 qq 号
     :param enable: 是则设置，否则取消
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
@@ -642,14 +693,17 @@
 
 @CtxManager._activate
 async def set_group_card(
     groupId: int, userId: int, card: str, wait: bool = False, auto: bool = True
 ) -> BotAction:
     """设置群名片
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-13 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-13>`_
+
     :param groupId: 群号
     :param userId: 设置的 qq 号
     :param card: 新名片内容
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
@@ -676,14 +730,17 @@
 
 @CtxManager._activate
 async def set_group_name(
     groupId: int, name: str, wait: bool = False, auto: bool = True
 ) -> BotAction:
     """设置群名
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-14 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-14>`_
+
     :param groupId: 群号
     :param name: 新群名
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
@@ -709,14 +766,17 @@
 
 @CtxManager._activate
 async def group_leave(
     groupId: int, isDismiss: bool, wait: bool = False, auto: bool = True
 ) -> BotAction:
     """退出群
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-15 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-15>`_
+
     :param groupId: 群号
     :param isDismiss: 是否解散群（仅在 bot 为群主时可用）
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
@@ -758,14 +818,17 @@
     title: str,
     duration: int = -1,
     wait: bool = False,
     auto: bool = True,
 ) -> BotAction:
     """设置群特殊头衔
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-16 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-16>`_
+
     :param groupId: 群号
     :param userId: 设置的 qq 号
     :param title: 头衔名
     :param duration: 生效时间，为 -1 则为无限期
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
@@ -792,14 +855,17 @@
 
 @CtxManager._activate
 async def set_friend_add(
     addFlag: str, approve: bool, remark: str, wait: bool = False, auto: bool = True
 ) -> BotAction:
     """处理加好友请求
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-17 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-17>`_
+
     :param addFlag: 好友添加 flag，对应 :attr:`~.RequestEvent.req_flag` 属性
     :param approve: 是否通过
     :param remark: 添加后的好友备注（仅用于通过请求后）
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
@@ -843,14 +909,17 @@
     approve: bool,
     rejectReason: Optional[str] = None,
     wait: bool = False,
     auto: bool = True,
 ) -> BotAction:
     """处理加群请求（只有 bot 是群管理时有用）
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-18 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-18>`_
+
     :param addFlag: 加群 flag，对应 :attr:`~.RequestEvent.req_flag` 属性
     :param addType: 加群类型，对应 :attr:`~.RequestEvent.group_req_type` 属性
     :param approve: 是否通过
     :param rejectReason: 如果不通过的原因回复
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
@@ -876,14 +945,17 @@
         self.params = {}
 
 
 @CtxManager._activate
 async def get_login_info(wait: bool = True, auto: bool = True) -> BotAction:
     """获得 bot 登录号信息
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-19 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-19>`_
+
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
        `auto=True, wait=True` -> :class:`.ResponseEvent` 对象
 
@@ -905,14 +977,17 @@
 
 @CtxManager._activate
 async def get_stranger_info(
     userId: int, noCache: bool, wait: bool = True, auto: bool = True
 ) -> BotAction:
     """获取陌生人信息，也可以对好友使用
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-20 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-20>`_
+
     :param userId: qq 号
     :param noCache: 是否不使用缓存
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
@@ -936,14 +1011,17 @@
         self.params = {}
 
 
 @CtxManager._activate
 async def get_friend_list(wait: bool = True, auto: bool = True) -> BotAction:
     """获取好友列表
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-21 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-21>`_
+
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
        `auto=True, wait=True` -> :class:`.ResponseEvent` 对象
 
@@ -965,14 +1043,17 @@
 
 @CtxManager._activate
 async def get_group_info(
     groupId: int, noCache: bool, wait: bool = True, auto: bool = True
 ) -> BotAction:
     """获取群信息，可以是未加入的群聊
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-22 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-22>`_
+
     :param groupId: 群号
     :param noCache: 是否不使用缓存
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
@@ -996,15 +1077,18 @@
         self.params = {}
 
 
 @CtxManager._activate
 async def get_group_list(wait: bool = True, auto: bool = True) -> BotAction:
     """获取群列表。
 
-    可能返回的建群时间都是 0，这是不准确的。准确的时间可以通过 :meth:`get_group_info` 获得.
+    可能返回的建群时间都是 0，这是不准确的。准确的时间可以通过 :meth:`get_group_info` 获得
+
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-23 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-23>`_
 
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
        `auto=True, wait=True` -> :class:`.ResponseEvent` 对象
@@ -1027,14 +1111,17 @@
 
 @CtxManager._activate
 async def get_group_member_info(
     groupId: int, userId: int, noCache: bool, wait: bool = True, auto: bool = True
 ) -> BotAction:
     """获取群成员信息
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-24 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-24>`_
+
     :param groupId: 群号
     :param userId: qq 号
     :param noCache: 是否不使用缓存
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
@@ -1061,14 +1148,17 @@
 
 @CtxManager._activate
 async def get_group_member_list(
     groupId: int, noCache: bool, wait: bool = True, auto: bool = True
 ) -> BotAction:
     """获取群成员列表
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-25 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-25>`_
+
     :param groupId: 群号
     :param noCache: 是否不使用缓存
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
@@ -1108,14 +1198,17 @@
     auto: bool = True,
 ) -> BotAction:
     """获取群荣誉信息
 
     详细说明参考：
     `获取群荣誉信息 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#get_group_honor_info-获取群荣誉信息>`_
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-26 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-26>`_
+
     :param groupId: 群号
     :param type: 荣誉类型
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
@@ -1139,14 +1232,17 @@
         self.params = {}
 
 
 @CtxManager._activate
 async def check_send_image(wait: bool = True, auto: bool = True) -> BotAction:
     """检查是否可以发送图片
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-32 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-32>`_
+
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
        `auto=True, wait=True` -> :class:`.ResponseEvent` 对象
 
@@ -1166,14 +1262,17 @@
         self.params = {}
 
 
 @CtxManager._activate
 async def check_send_record(wait: bool = True, auto: bool = True) -> BotAction:
     """检查是否可以发送语音
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-33 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-33>`_
+
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
        `auto=True, wait=True` -> :class:`.ResponseEvent` 对象
 
@@ -1193,14 +1292,17 @@
         self.params = {}
 
 
 @CtxManager._activate
 async def get_onebot_version(wait: bool = True, auto: bool = True) -> BotAction:
     """获取 onebot 实现项目的版本
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-35 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-35>`_
+
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
        `auto=True, wait=True` -> :class:`.ResponseEvent` 对象
 
@@ -1220,14 +1322,17 @@
         self.params = {}
 
 
 @CtxManager._activate
 async def get_onebot_status(wait: bool = True, auto: bool = True) -> BotAction:
     """获取 onebot 实现项目的状态
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-34 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-34>`_
+
     :param wait: 是否等待这个行为的响应
     :param auto: 是否自动发送
     :return:
        `auto=False` -> :class:`.BotAction` 对象
 
        `auto=True, wait=True` -> :class:`.ResponseEvent` 对象
 
@@ -1267,15 +1372,15 @@
     """
     args = ActionArgs()
     args.type, args.params = type, params
     return BotAction(args, get_id() if need_resp else None, trigger, ready=False)
 
 
 async def send_wait(
-    content: str | CQMsgDict | list[CQMsgDict],
+    content: str | MsgSegment | list[MsgSegment],
     cq_str: bool = False,
     overtime: Optional[int] = None,
 ) -> None:
     """发送一条消息然后暂停当前会话（在当前会话下自动定位发送目标）
 
     会话应该是可暂停的，这意味着该会话应该拥有会话规则。
 
@@ -1284,17 +1389,17 @@
 
        当启用了 `cq_str` 选项，且 `content` 参数为字符串时，
        `content` 字符串将不会被处理为消息段对象，此时字符串中的 cq 码将会直接生效，而不是被转义。
 
     .. admonition:: 警告
        :class: attention
 
-       这个小技巧可以让你发送有效的 cq 码字符串。但是存在潜在的安全问题：
-       如果将用户输入作为 cq 码字符串的一部分发送出去，这将会造成“注入攻击”！
-       用户可以构造包含恶意图片、语音的 cq 码，让 bot 发送。
+       这个小技巧可以让你直接发送 CQ 码字符串。但是存在潜在的安全问题：
+       如果将用户输入作为 CQ 码字符串的一部分发送出去，这将会造成“注入攻击”！
+       用户可以构造包含恶意图片、语音的 CQ 码，让 bot 发送。
 
        任何时候启用 `cq_str` 选项，如需用到用户输入，务必校验。
 
     :param content: 发送内容
     :param cq_str: 是否以 cq 字符串发送（默认格式是消息段对象)
     :param overtime: 会话暂停的超时时间，超时将抛出 :class:`.SessionHupTimeout` 异常
     """
@@ -1302,59 +1407,66 @@
     try:
         await SESSION_LOCAL.hup(overtime)
     except LookupError:
         raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
 
 
 async def send_reply(
-    content: str | CQMsgDict | list[CQMsgDict],
+    content: str | MsgSegment | list[MsgSegment],
     cq_str: bool = False,
     wait: bool = False,
-) -> Optional["ResponseEvent"]:
+    auto: bool = True,
+) -> Union[BotAction, "ResponseEvent", None]:
     """发送一条回复消息（在当前会话下自动定位发送目标）
 
     .. admonition:: 小技巧
        :class: note
 
        当启用了 `cq_str` 选项，且 `content` 参数为字符串时，
        `content` 字符串将不会被处理为消息段对象，此时字符串中的 cq 码将会直接生效，而不是被转义。
 
     .. admonition:: 警告
        :class: attention
 
-       这个小技巧可以让你发送有效的 cq 码字符串。但是存在潜在的安全问题：
-       如果将用户输入作为 cq 码字符串的一部分发送出去，这将会造成“注入攻击”！
-       用户可以构造包含恶意图片、语音的 cq 码，让 bot 发送。
+       这个小技巧可以让你直接发送 CQ 码字符串。但是存在潜在的安全问题：
+       如果将用户输入作为 CQ 码字符串的一部分发送出去，这将会造成“注入攻击”！
+       用户可以构造包含恶意图片、语音的 CQ 码，让 bot 发送。
 
        任何时候启用 `cq_str` 选项，如需用到用户输入，务必校验。
 
+    响应数据将会在响应的 :attr:`~.ResponseEvent.data` 属性，数据结构参考：
+    `响应数据-2 <https://github.com/botuniverse/onebot-11/blob/master/api/public.md#响应数据-2>`_
+
     :param content: 发送内容
     :param cq_str: 是否以 cq 字符串发送（默认格式是消息段对象)
     :param wait: 是否等待发送后的响应
+    :param auto: 是否自动发送
     :return:
-       若指定等待 -> :class:`.ResponseEvent` 对象
+       `auto=False` -> :class:`.BotAction` 对象
+
+       `auto=True, wait=True` -> :class:`.ResponseEvent` 对象
 
-       若未指定等待 -> :obj:`None`
+       `auto=True, wait=False` -> :obj:`None`
     """
     try:
         content_arr = [reply_msg(SESSION_LOCAL.event.id)]
     except LookupError:
         raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
 
     if isinstance(content, str):
         content_arr.append(text_msg(content))
     elif isinstance(content, dict):
         content_arr.append(content)
     else:
         content_arr.extend(content)
-    return await send(content_arr, cq_str, wait)  # type: ignore
+    return await send(content_arr, cq_str, wait, auto)
 
 
 async def finish(
-    content: str | CQMsgDict | list[CQMsgDict],
+    content: str | MsgSegment | list[MsgSegment],
     cq_str: bool = False,
 ) -> None:
     """发送一条消息，然后直接结束当前事件处理方法（在当前会话下自动定位发送目标）
 
     只可在事件处理方法中使用。
 
     .. admonition:: 小技巧
@@ -1362,17 +1474,17 @@
 
        当启用了 `cq_str` 选项，且 `content` 参数为字符串时，
        `content` 字符串将不会被处理为消息段对象，此时字符串中的 cq 码将会直接生效，而不是被转义。
 
     .. admonition:: 警告
        :class: attention
 
-       这个小技巧可以让你发送有效的 cq 码字符串。但是存在潜在的安全问题：
-       如果将用户输入作为 cq 码字符串的一部分发送出去，这将会造成“注入攻击”！
-       用户可以构造包含恶意图片、语音的 cq 码，让 bot 发送。
+       这个小技巧可以让你直接发送 CQ 码字符串。但是存在潜在的安全问题：
+       如果将用户输入作为 CQ 码字符串的一部分发送出去，这将会造成“注入攻击”！
+       用户可以构造包含恶意图片、语音的 CQ 码，让 bot 发送。
 
        任何时候启用 `cq_str` 选项，如需用到用户输入，务必校验。
 
     :param content: 发送内容
     :param cq_str: 是否以 cq 字符串发送（默认格式是消息段对象)
     """
     await send(content, cq_str)
@@ -1380,33 +1492,33 @@
         SESSION_LOCAL.destory()
     except LookupError:
         raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
     raise DirectRetSignal("事件处理方法被安全地递归 return，请无视这个异常")
 
 
 async def reply_finish(
-    content: str | CQMsgDict | list[CQMsgDict],
+    content: str | MsgSegment | list[MsgSegment],
     cq_str: bool = False,
-) -> Optional["ResponseEvent"]:
+) -> None:
     """发送一条回复消息，然后直接结束当前事件处理方法（在当前会话下自动定位发送目标）
 
     只可在事件处理方法中使用。
 
     .. admonition:: 小技巧
        :class: note
 
        当启用了 `cq_str` 选项，且 `content` 参数为字符串时，
        `content` 字符串将不会被处理为消息段对象，此时字符串中的 cq 码将会直接生效，而不是被转义。
 
     .. admonition:: 警告
        :class: attention
 
-       这个小技巧可以让你发送有效的 cq 码字符串。但是存在潜在的安全问题：
-       如果将用户输入作为 cq 码字符串的一部分发送出去，这将会造成“注入攻击”！
-       用户可以构造包含恶意图片、语音的 cq 码，让 bot 发送。
+       这个小技巧可以让你直接发送 CQ 码字符串。但是存在潜在的安全问题：
+       如果将用户输入作为 CQ 码字符串的一部分发送出去，这将会造成“注入攻击”！
+       用户可以构造包含恶意图片、语音的 CQ 码，让 bot 发送。
 
        任何时候启用 `cq_str` 选项，如需用到用户输入，务必校验。
 
     :param content: 发送内容
     :param cq_str: 是否以 cq 字符串发送（默认格式是消息段对象)
     """
     try:
```

### Comparing `melobot-2.5.8/src/melobot/context/session.py` & `melobot-2.5.9/src/melobot/context/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,19 +64,19 @@
     @property
     def args(self):
         if (
             self._handler is not None
             and hasattr(self._handler, "parser")
             and self.event._args_map is not None
         ):
-            args_group = self.event._args_map.get(self._handler.parser.id)
-            if args_group is None:
+            args_dict = self.event._args_map.get(self._handler.parser.id)
+            if args_dict is None:
                 return None
-            for cmd_name in self._handler.parser.target:
-                args = args_group.get(cmd_name)
+            for group_id in self._handler.parser.target:
+                args = args_dict.get(group_id)
                 if args is not None:
                     return deepcopy(args.vals)
             raise BotSessionError("尝试获取的命令解析参数不存在")
         return None
 
     async def hup(self, overtime: Optional[int] = None) -> None:
         """当前 session 挂起（也就是所在方法的挂起）。直到满足同一 session_rule 的事件重新进入， session
@@ -469,20 +469,20 @@
 
     :return: 具体的事件
     """
     return any_event()  # type: ignore
 
 
 def msg_text() -> str:
-    """获取当前会话下的消息事件的，所有纯文本消息的合并字符串。
+    """获取当前会话下的，消息事件的纯文本内容的合并字符串。
     等价于手动读取消息事件的 :attr:`~.MessageEvent.text` 属性
 
     只能在确定当前会话下必为消息事件时使用
 
-    :return: 所有纯文本消息的合并字符串
+    :return: 纯文本内容的合并字符串
     """
     event: "MessageEvent" = any_event()  # type: ignore
     return event.text
 
 
 def msg_args() -> list[Any] | None:
     """获取当前会话下的消息事件的所有解析参数值。
@@ -531,14 +531,14 @@
 def dispose() -> None:
     """销毁当前会话
 
     将会清理会话的存储空间，并将会话标记为过期态。
     此时调用该方法的函数依然可以运行，但是此会话状态下无法再进行行为操作。
 
     一般来说，会话将会自动销毁。
-    只有在注册事件处理函数时使用 `session_hold=True`，才会需要使用此函数。
+    只有在绑定事件处理函数时使用 `session_hold=True`，才会需要使用此函数。
 
     """
     try:
         SESSION_LOCAL.destory()
     except LookupError:
         raise BotSessionError("当前 session 上下文不存在，因此无法使用本方法")
```

### Comparing `melobot-2.5.8/src/melobot/controller/dispatcher.py` & `melobot-2.5.9/src/melobot/controller/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         for tuple in self._channel_map.values():
             for channel in tuple:
                 if channel not in self.handlers.keys():
                     self.handlers[channel] = []
 
     def add_handlers(self, handlers: list["EventHandler"]) -> None:
-        """绑定事件处理器列表."""
+        """绑定事件处理器列表"""
         for handler in handlers:
             self.handlers[handler.__class__].append(handler)
         for k in self.handlers.keys():
             self.handlers[k] = sorted(
                 self.handlers[k], key=lambda x: x.priority, reverse=True
             )
```

### Comparing `melobot-2.5.8/src/melobot/controller/responder.py` & `melobot-2.5.9/src/melobot/controller/responder.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/src/melobot/io/forward_ws.py` & `melobot-2.5.9/src/melobot/io/forward_ws.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/src/melobot/io/full_duplex_http.py` & `melobot-2.5.9/src/melobot/io/full_duplex_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self.onebot_url = f"http://{onebot_host}:{onebot_port}"
         #: 本连接器服务端的 host
         self.host: str = listen_host
         #: 本连接器服务端的 port
         self.port: int = listen_port
         #: 本连接器服务端的站点对象
         self.serve_site: aiohttp.web.TCPSite
-        #: 本连接器客户端的 HTTP 会话
+        #: 本连接器客户端的会话
         self.client_session: aiohttp.ClientSession
 
         self._send_queue: asyncio.Queue["BotAction"] = asyncio.Queue()
         self._pre_send_time = time.time()
         self._closed = asyncio.Event()
         self._close_lock = asyncio.Lock()
         self._onebot_onlined = asyncio.Event()
```

### Comparing `melobot-2.5.8/src/melobot/io/reverse_ws.py` & `melobot-2.5.9/src/melobot/io/reverse_ws.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/src/melobot/meta.py` & `melobot-2.5.9/src/melobot/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
        :class: tip
 
        一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
     """
 
     def __init__(self) -> None:
         #: melobot 版本
-        self.VER: str = "2.5.8"
+        self.VER: str = "2.5.9"
         #: melobot 项目名称
         self.PROJ_NAME: str = "melobot"
         #: melobot 项目描述
         self.PROJ_DESC: str = (
             "A qq bot development framework with friendly APIs, session control and plugin-supported."
         )
         #: melobot 项目地址
```

### Comparing `melobot-2.5.8/src/melobot/models/__init__.py` & `melobot-2.5.9/src/melobot/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .cq import *
 from .event import MessageEvent, MetaEvent, NoticeEvent, RequestEvent, ResponseEvent
+from .msg import *
 
 __all__ = (
     "MessageEvent",
     "MetaEvent",
     "NoticeEvent",
     "RequestEvent",
     "ResponseEvent",
@@ -22,9 +22,10 @@
     "custom_msg_node",
     "refer_msg_node",
     "cq_filter_text",
     "cq_escape",
     "cq_anti_escape",
     "to_cq_arr",
     "to_cq_str",
-    "custom_type_msg"
+    "custom_type_msg",
+    "forward_msg",
 )
```

### Comparing `melobot-2.5.8/src/melobot/models/cq.py` & `melobot-2.5.9/src/melobot/models/msg.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from copy import deepcopy
 from itertools import chain, zip_longest
 
 from ..base.exceptions import BotActionError
 from ..base.typing import (
     TYPE_CHECKING,
     Any,
-    CQMsgDict,
+    Callable,
     Literal,
-    MsgNodeDict,
+    MsgNode,
+    MsgSegment,
     Optional,
-    Type,
 )
 
 if TYPE_CHECKING:
     from ..base.abc import BotAction
 
 
 __all__ = (
@@ -33,34 +33,35 @@
     "refer_msg_node",
     "reply_msg",
     "share_msg",
     "text_msg",
     "to_cq_arr",
     "to_cq_str",
     "xml_msg",
-    "custom_type_msg"
+    "custom_type_msg",
+    "forward_msg",
 )
 
 
 def text_msg(
     text: str,
-) -> CQMsgDict:
+) -> MsgSegment:
     """生成普通文本消息
 
     参数详细说明参考 onebot 标准：`纯文本 <https://github.com/botuniverse/onebot-11/blob/master/message/segment.md#纯文本>`_
 
-    :param text: 消息内容
+    :param text: 文本内容
     :return: onebot 标准中的消息段对象
     """
     return {"type": "text", "data": {"text": text}}
 
 
 def face_msg(
     id: int,
-) -> CQMsgDict:
+) -> MsgSegment:
     """生成 qq 表情消息
 
     参数详细说明参考 onebot 标准：`QQ 表情 <https://github.com/botuniverse/onebot-11/blob/master/message/segment.md#qq-表情>`_
 
     :param id: qq 表情的 ID
     :return: onebot 标准中的消息段对象
     """
@@ -69,74 +70,74 @@
 
 def record_msg(
     file: str,
     magic: Literal[0, 1] = 0,
     cache: Literal[0, 1] = 1,
     proxy: Literal[0, 1] = 1,
     timeout: Optional[int] = None,
-) -> CQMsgDict:
+) -> MsgSegment:
     """生成语音消息
 
     参数详细说明参考 onebot 标准：`语音 <https://github.com/botuniverse/onebot-11/blob/master/message/segment.md#语音>`_
 
     :param file: 语音文件名
     :param magic: 是否使用变声
     :param cache: 是否使用已缓存文件
     :param proxy: 是否通过代理下载文件
     :param timeout: 超时时间，默认不启用
     :return: onebot 标准中的消息段对象
     """
-    base: CQMsgDict = {
+    base: MsgSegment = {
         "type": "record",
         "data": {
             "file": file,
             "magic": str(magic),
             "cache": str(cache),
             "proxy": str(proxy),
         },
     }
     if timeout:
         base["data"]["timeout"] = str(timeout)
     return base
 
 
-def at_msg(qq: int | Literal["all"]) -> CQMsgDict:
+def at_msg(qq: int | Literal["all"]) -> MsgSegment:
     """生成艾特消息
 
     参数详细说明参考 onebot 标准：`某人 <https://github.com/botuniverse/onebot-11/blob/master/message/segment.md#某人>`_
 
     :param qq: 艾特的 qq 号，"all" 表示艾特全体成员
     :return: onebot 标准中的消息段对象
     """
-    base: CQMsgDict = {
+    base: MsgSegment = {
         "type": "at",
         "data": {
             "qq": str(qq),
         },
     }
     return base
 
 
 def share_msg(
     url: str,
     title: str,
     content: Optional[str] = None,
     image: Optional[str] = None,
-) -> CQMsgDict:
+) -> MsgSegment:
     """生成链接分享消息
 
     参数详细说明参考 onebot 标准：`链接分享 <https://github.com/botuniverse/onebot-11/blob/master/message/segment.md#链接分享>`_
 
     :param url: 链接的 url
     :param title: 消息的标题
     :param content: 消息的内容描述（可选）
     :param image: 消息的封面图 url（可选）
     :return: onebot 标准中的消息段对象
     """
-    base: CQMsgDict = {
+    base: MsgSegment = {
         "type": "share",
         "data": {
             "url": url,
             "title": title,
         },
     }
     if content:
@@ -145,15 +146,15 @@
         base["data"]["image"] = image
     return base
 
 
 def music_msg(
     type: Literal["qq", "163", "xm"],
     id: str,
-) -> CQMsgDict:
+) -> MsgSegment:
     """生成音乐分享消息
 
     参数详细说明参考 onebot 标准：`音乐分享 <https://github.com/botuniverse/onebot-11/blob/master/message/segment.md#音乐分享->`_
 
     :param type: 音乐平台的类型（q 音、网易云、虾米）
     :param id: 歌曲 id
     :return: onebot 标准中的消息段对象
@@ -163,27 +164,27 @@
 
 def custom_music_msg(
     url: str,
     audio: str,
     title: str,
     content: Optional[str] = None,
     image: Optional[str] = None,
-) -> CQMsgDict:
+) -> MsgSegment:
     """生成音乐自定义分享 url
 
     参数详细说明参考 onebot 标准：`音乐自定义分享 <https://github.com/botuniverse/onebot-11/blob/master/message/segment.md#音乐自定义分享->`_
 
     :param url: 点击后跳转目标 url
     :param audio: 音乐 url
     :param title: 标题
     :param content: 内容描述（可选）
     :param image: 封面图 url（可选）
     :return: onebot 标准中的消息段对象
     """
-    base: CQMsgDict = {
+    base: MsgSegment = {
         "type": "music",
         "data": {
             "type": "custom",
             "url": url,
             "audio": audio,
             "title": title,
         },
@@ -197,27 +198,27 @@
 
 def image_msg(
     file: str,
     type: Optional[Literal["flash"]] = None,
     cache: Literal[0, 1] = 1,
     proxy: Literal[0, 1] = 1,
     timeout: Optional[int] = None,
-) -> CQMsgDict:
+) -> MsgSegment:
     """生成图片消息
 
     参数详细说明参考 onebot 标准：`图片 <https://github.com/botuniverse/onebot-11/blob/master/message/segment.md#图片>`_
 
     :param file: 图片文件名或图片 base64 内容
     :param type: 图片类型
     :param cache: 是否使用已缓存的文件
     :param proxy: 是否通过代理下载文件
     :param timeout: 超时时间，默认不超时
     :return: onebot 标准中的消息段对象
     """
-    base: CQMsgDict = {
+    base: MsgSegment = {
         "type": "image",
         "data": {
             "file": file,
             "cache": str(cache),
             "proxy": str(proxy),
         },
     }
@@ -226,15 +227,15 @@
     if timeout:
         base["data"]["timeout"] = str(timeout)
     return base
 
 
 def reply_msg(
     id: int,
-) -> CQMsgDict:
+) -> MsgSegment:
     """生成回复消息
 
     参数详细说明参考 onebot 标准：`回复 <https://github.com/botuniverse/onebot-11/blob/master/message/segment.md#回复>`_
 
     :param id: 消息 id
     :return: onebot 标准中的消息段对象
     """
@@ -244,15 +245,15 @@
             "id": str(id),
         },
     }
 
 
 def poke_msg(
     qq: int,
-) -> CQMsgDict:
+) -> MsgSegment:
     """生成戳一戳消息
 
     .. admonition:: 提示
        :class: tip
 
        鉴于目前大多数实现 cq 协议的项目都采用了此参数规范，因此在 melobot 中，也采用此规范。虽然这种规范实际上不符合 onebot 标准
 
@@ -263,43 +264,60 @@
         "type": "poke",
         "data": {
             "qq": str(qq),
         },
     }
 
 
-def xml_msg(data: str) -> CQMsgDict:
+def xml_msg(data: str) -> MsgSegment:
     """生成 xml 消息
 
     参数详细说明参考 onebot 标准：`xml 消息 <https://github.com/botuniverse/onebot-11/blob/master/message/segment.md#xml-消息>`_
 
     :param data: xml 内容
     :return: onebot 标准中的消息段对象
     """
     return {"type": "xml", "data": {"data": data}}
 
 
-def json_msg(data: str) -> CQMsgDict:
+def json_msg(data: str) -> MsgSegment:
     """生成 json 消息
 
     参数详细说明参考 onebot 标准：`json 消息 <https://github.com/botuniverse/onebot-11/blob/master/message/segment.md#json-消息>`_
 
     :param data: json 内容
     :return: onebot 标准中的消息段对象
     """
     return {"type": "json", "data": {"data": data}}
 
 
+def forward_msg(forwardId: str) -> MsgSegment:
+    """生成一条完整的转发消息，以消息段的形式
+
+    .. admonition:: 注意
+       :class: caution
+
+       这与通过结点来构造转发消息是不同的，这里直接构造一个消息段对象，就可以代表整条转发消息。
+       因为这里使用的是转发 id。
+
+    参数详细说明参考 onebot 标准：`forward 消息段 <https://github.com/botuniverse/onebot-11/blob/master/message/segment.md#合并转发->`_
+
+    :param forwardId: 转发 id
+    :return: onebot 标准中的消息段对象
+    """
+    return {"type": "forward", "data": {"id": str(forwardId)}}
+
+
 def custom_msg_node(
-    content: str | CQMsgDict | list[CQMsgDict],
+    content: str | MsgSegment | list[MsgSegment],
     sendName: str,
     sendId: int,
-    seq: Optional[list[CQMsgDict]] = None,
+    seq: Optional[list[MsgSegment]] = None,
     useStd: bool = False,
-) -> MsgNodeDict:
+) -> MsgNode:
     """生成一个自定义合并消息转发结点
 
     .. admonition:: 提示
        :class: tip
 
        鉴于此方法涉及的消息构造，存在两种规范：
        `onebot 规范 <https://github.com/botuniverse/onebot-11/blob/master/message/segment.md#合并转发自定义节点>`_、
@@ -324,45 +342,45 @@
         for _ in content:
             if isinstance(_, list):
                 temp.extend(_)
             else:
                 temp.append(_)
         msgs = temp
     if not useStd:
-        ret: MsgNodeDict = {
+        ret: MsgNode = {
             "type": "node",
             "data": {"name": sendName, "uin": str(sendId), "content": msgs},
         }
     else:
-        ret: MsgNodeDict = {  # type: ignore
+        ret: MsgNode = {  # type: ignore
             "type": "node",
             "data": {"user_id": sendId, "nickname": sendName, "content": msgs},
         }
     if seq:
         ret["data"]["seq"] = seq  # type: ignore
     return ret
 
 
-def refer_msg_node(id: int) -> MsgNodeDict:
+def refer_msg_node(id: int) -> MsgNode:
     """生成一个引用合并消息转发结点
 
     :param id: 消息 id
     :return: onebot 标准中的消息段对象
     """
     return {"type": "node", "data": {"id": str(id)}}
 
 
-def custom_type_msg(type: str, params: dict[str, str]) -> CQMsgDict:
+def custom_type_msg(type: str, params: dict[str, str]) -> MsgSegment:
     """生成一个自定义消息段对象
 
     :param type: 消息段对象的类型标识
     :param params: 消息段的参数
     :return: 符合 onebot 格式，但不在 onebot 标准中的消息段对象
     """
-    ret: CQMsgDict = {"type": type, "data": {}}
+    ret: MsgSegment = {"type": type, "data": {}}
     for k, v in params.items():
         ret["data"][k] = str(v)
     return ret
 
 
 def cq_filter_text(s: str) -> str:
     """cq 文本过滤函数
@@ -404,15 +422,15 @@
         text.replace("&#44;", ",")
         .replace("&#93;", "]")
         .replace("&#91;", "[")
         .replace("&amp;", "&")
     )
 
 
-def to_cq_arr(s: str) -> list[CQMsgDict]:
+def to_cq_arr(s: str) -> list[MsgSegment]:
     """将 cq 字符串转换为消息段对象列表
 
     :param s: cq 字符串
     :return: 消息段对象列表
     """
 
     def replace_func(m) -> str:
@@ -448,15 +466,15 @@
                 data[name] = float(val)
             except Exception:
                 data[name] = val
         content.append({"type": cq_type, "data": data})
     return content
 
 
-def to_cq_str(content: list[CQMsgDict]) -> str:
+def to_cq_str(content: list[MsgSegment]) -> str:
     """将消息段对象列表转换为 cq 字符串
 
     :param content: 消息段对象列表
     :return: cq 字符串
     """
     if isinstance(content, str):
         return content
@@ -489,20 +507,23 @@
     elif _action.type in ("send_private_forward_msg", "send_group_forward_msg"):
         _format_forward_action(_action)
     else:
         raise BotActionError("传入的 action 因类型不匹配，不可被 cq 序列化")
     return _action
 
 
-def _get_cq(content: list[CQMsgDict], cq_type: str) -> list[CQMsgDict]:
+def _get_cq(content: list[MsgSegment], cq_type: str) -> list[MsgSegment]:
     return [item for item in content if item["type"] == cq_type]
 
 
 def _get_cq_params(
-    content: list[CQMsgDict], cq_type: str, param: str, type: Optional[Type[Any]] = None
+    content: list[MsgSegment],
+    cq_type: str,
+    param: str,
+    type: Optional[Callable[[Any], Any]] = None,
 ) -> list[Any]:
     res: list[Any] = []
     for item in content:
         if item["type"] == cq_type:
             val = item["data"].get(param)
             res.append(val)
     if type is not None:
```

### Comparing `melobot-2.5.8/src/melobot/models/event.py` & `melobot-2.5.9/src/melobot/models/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import re
 import time
 
 from ..base.abc import BotEvent
-from ..base.typing import Any, CQMsgDict, Literal, Optional, Type
-from .cq import _get_cq, _get_cq_params, to_cq_arr, to_cq_str
+from ..base.typing import Any, Callable, Literal, MsgSegment, Optional
+from .msg import _get_cq, _get_cq_params, to_cq_arr, to_cq_str
 
 
 class BotEventBuilder:
     @staticmethod
     def build(rawEvent: dict | str) -> BotEvent:
         if isinstance(rawEvent, str):
             raw: dict[str, str | float | int] = json.loads(rawEvent)
@@ -46,15 +46,15 @@
         #: 消息事件的发送者数据结构
         self.sender: MessageEvent.Sender
         #: 消息事件的来源群号，私聊时此属性也存在并为 :obj:`None`
         self.group_id: Optional[int]
         #: 使用 CQ 字符串表示的，本事件的所有消息内容
         self.raw_content: str
         #: 使用消息段对象列表表示的，本事件的所有消息内容
-        self.content: list[CQMsgDict]
+        self.content: list[MsgSegment]
         #: 本事件的所有消息内容中，纯文本消息的合并字符串
         self.text: str
         #: 消息字体
         self.font: int
         #: 临时消息的来源标记，不是临时消息时为 :obj:`None`
         self.temp_src: Optional[
             Literal[
@@ -110,15 +110,15 @@
     def _format_to_str(self, content: list | str) -> str:
         """对外部零信任，强制转换为 cq 字符串格式."""
         if not isinstance(content, str):
             return to_cq_str(content)
         else:
             return content
 
-    def _format_to_array(self, content: list | str) -> list[CQMsgDict]:
+    def _format_to_array(self, content: list | str) -> list[MsgSegment]:
         """对外部零信任，强制转换为消息段格式."""
         if not isinstance(content, str):
             for item in content:
                 if item["type"] == "text":
                     continue
                 for k, v in item["data"].items():
                     if not isinstance(v, str):
@@ -130,54 +130,54 @@
                         item["data"][k] = float(v)
                     except Exception:
                         pass
             return content
         else:
             return to_cq_arr(content)
 
-    def _get_text(self, content: list[CQMsgDict]) -> str:
+    def _get_text(self, content: list[MsgSegment]) -> str:
         """获取消息中所有文本消息，返回合并字符串."""
         text_list: list[str] = []
         for item in content:
             if item["type"] == "text":
                 text_list.append(item["data"]["text"])  # type: ignore
         return "".join(text_list)
 
-    def get_cq(self, cq_type: str) -> list[CQMsgDict]:
-        """提取指定类型的消息组成消息段对象列表
+    def get_segments(self, type: str) -> list[MsgSegment]:
+        """提取指定类型的，消息段对象组成的消息段对象列表
 
-        :param cq_type: 消息段对象类型
+        :param type: 消息段类型（对应 OneBot 标准中每种消息段对象的 type）
         :return: 消息段对象列表
         """
-        return _get_cq(self.content, cq_type)
+        return _get_cq(self.content, type)
 
-    def get_cq_params(
-        self, cq_type: str, param: str, type: Optional[Type[Any]] = None
+    def get_datas(
+        self, type: str, data: str, convert: Optional[Callable[[Any], Any]] = None
     ) -> list[Any]:
-        """提取指定类型的消息中的指定参数
+        """提取指定类型的消息段对象中的指定数据
 
-        当没有任何对应类型的消息时，为空列表。如果有对应类型的消息，但是指定的参数不存在，
+        当没有任何对应类型的消息段时，为空列表。如果有对应类型的消息段，但是指定的数据键名不存在，
         则在列表中产生 :obj:`None` 值.
 
-        可以指定 type 来强制转换类型，不填则使用智能解析出的类型
+        可以指定 `convert` 来强制转换类型，不填则不使用类型转换
 
         使用示例如下：
 
         .. code:: python
 
            # 假设 event 是 MessageEvent 对象，即象征一个消息事件
-           params = event.get_cq_params('at', 'qq')
-           # params 将是此事件中，所有 at 类型消息的 "qq" 参数所组成的列表
+           datas = event.get_datas('at', 'qq')
+           # datas 将是此事件中，所有 at 消息段的 "qq" 数据值所组成的列表
 
-        :param cq_type: 消息类型
-        :param param: 该类消息中的参数名
-        :param type: 类型转换使用的类
-        :return: 参数值列表
+        :param type: 消息段类型（对应 OneBot 标准中每种消息段对象的 type）
+        :param data: 消息段对象 `data` 中的键名
+        :param convert: 类型转换使用的函数
+        :return: 值列表
         """
-        return _get_cq_params(self.content, cq_type, param, type)
+        return _get_cq_params(self.content, type, data, convert)
 
     def is_private(self) -> bool:
         """是否为私聊消息（注意群临时会话属于该类别）"""
         return self.raw["message_type"] == "private"
 
     def is_friend(self) -> bool:
         """是否为好友消息"""
@@ -412,19 +412,19 @@
        :class: tip
 
        一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
 
     .. admonition:: 注意
        :class: caution
 
-       受 onebot 协议实现项目的影响，以及对通知事件本身复杂性的考虑，通知事件的所有实例属性，
-       都只会在特定类别的通知事件中存在。想要使用这些属性，最好先经过实际验证。
+       受 onebot 协议实现项目的影响，及对通知事件本身复杂性的考虑，通知事件大多数实例属性，
+       只会在特定类别的通知事件中存在。各个属性的含义与存在的时机，已在下方的注释说明。
 
-       例如你想要处理一个群禁言通知事件，建议先绑定“群禁言通知事件”的事件处理器，
-       然后调试查看事件都有哪些属性。这样就可以确定对“群禁言”这一类别的通知事件哪些属性可用。
+       如果你仍不确定某个属性在何时出现，建议直接调试查看存在的属性。例如通过
+       `print(event.__dict__)` 或调试器查看。
     """
 
     def __init__(self, rawEvent: dict) -> None:
         super().__init__(rawEvent)
         #: 收到事件的机器人 qq 号
         self.bot_id: int = rawEvent.get("self_id")  # type: ignore
         # 修复某些 onebot 协议实现，user_id 缺失的问题
@@ -714,16 +714,14 @@
        :class: tip
 
        onebot 标准中未定义“响应”为一种事件类型。但在 melobot 中，“响应”仍然被封装为一种事件类型。
     """
 
     def __init__(self, rawEvent: dict) -> None:
         super().__init__(rawEvent)
-
-        #: 响应标识符。当响应是对 resp_id 属性不为空的 :class:`.BotAction` 的回应时，此属性才不为 :obj:`None`
         self.id: Optional[str] = None
         #: 响应的状态码
         self.status: int
         #: 响应的数据
         self.data: Optional[dict] = None
 
         self._init()
```

### Comparing `melobot-2.5.8/src/melobot/plugin/handler.py` & `melobot-2.5.9/src/melobot/plugin/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,47 +246,47 @@
     ) -> bool | tuple[bool, str | None, ParseArgs | None]:
         """检查是否匹配."""
         if self.matcher:
             return self.matcher.match(event.text)
         if self.parser:
             _ = event._get_args(self.parser.id)
             if _ is Void:
-                args_group = self.parser.parse(event.text)
-                event._store_args(self.parser.id, args_group)
+                args_dict = self.parser.parse(event.text)
+                event._store_args(self.parser.id, args_dict)
             else:
-                args_group = _
-            res, cmd_name, args = self.parser.test(args_group)
-            return res, cmd_name, args
+                args_dict = _
+            res, group_id, args = self.parser.test(args_dict)
+            return res, group_id, args
         return True
 
-    async def _format(self, cmd_name: str, args: ParseArgs) -> bool:
+    async def _format(self, group_id: str, args: ParseArgs) -> bool:
         """格式化。只有 parser 存在时需要."""
         self.parser = cast(BotParser, self.parser)
         if not self.parser.need_format:
             return True
-        status = await self.parser.format(cmd_name, args)
+        status = await self.parser.format(group_id, args)
         return status
 
     async def _pre_process(self, event: "MessageEvent") -> bool:  # type: ignore
         session = BotSessionManager.make_temp(event)
         # 先进行 match，match 不支持回调，因此可以直接同步运行，而且无需异步加锁
         match_res = self._match(event)
         if isinstance(match_res, bool):
             if not match_res:
                 return False
         else:
-            res, cmd_name, args = match_res
+            res, group_id, args = match_res
             if not res:
                 return False
 
         async def wrapped_func() -> bool:
             if not (await self._verify()):
                 return False
             if self.parser:
-                if not (await self._format(cmd_name, args)):  # type: ignore
+                if not (await self._format(group_id, args)):  # type: ignore
                     return False
             return True
 
         status = await self._run_on_ctx(wrapped_func(), session)
         return status
```

### Comparing `melobot-2.5.8/src/melobot/plugin/init.py` & `melobot-2.5.9/src/melobot/plugin/init.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,37 +50,54 @@
     from ..base.abc import SessionRule, WrappedChecker
     from ..utils.checker import BotChecker
     from ..utils.matcher import BotMatcher
     from ..utils.parser import BotParser
 
 
 class PluginProxy:
-    """Bot 插件代理类。供外部使用."""
+    """Bot 插件代理类
+
+    通过 bot 实例获取插件时，将获取此对象的列表
+
+    .. admonition:: 提示
+       :class: tip
+
+       一般无需手动实例化该类，多数情况会直接使用本类对象，或将本类用作类型注解。
+    """
 
     def __init__(
         self,
         id: str,
         ver: str,
         desc: str,
         doc: str,
         keywords: list[str],
         url: str,
         share_objs: list[tuple[str, str]],
         share_cbs: list[tuple[str, str]],
         signal_methods: list[tuple[str, str]],
     ) -> None:
-        self.id = id
-        self.version = ver
-        self.desc = desc
-        self.doc = doc
-        self.keywords = keywords
-        self.url = url
-        self.shares = share_objs
-        self.share_cbs = share_cbs
-        self.signal_methods = signal_methods
+        #: 插件的 id
+        self.id: str = id
+        #: 插件的版本
+        self.version: str = ver
+        #: 插件的简短描述
+        self.desc: str = desc
+        #: 插件的长篇描述
+        self.doc: str = doc
+        #: 插件的关键词
+        self.keywords: list[str] = keywords
+        #: 插件的项目地址
+        self.url: str = url
+        #: 插件的共享对象标识：[(命名空间，id), ...]
+        self.shares: list[tuple[str, str]] = share_objs
+        #: 插件的共享对象回调标识：[(命名空间，id), ...]
+        self.share_cbs: list[tuple[str, str]] = share_cbs
+        #: 插件的信号处理方法标识：[(命名空间, 信号名), ...]
+        self.signal_methods: list[tuple[str, str]] = signal_methods
 
 
 class PluginLoader:
     """插件加载器."""
 
     @staticmethod
     def load_from_dir(plugin_path: str) -> "BotPlugin":
@@ -116,18 +133,15 @@
         else:
             plugin = target
         plugin._self_build()
         return plugin
 
 
 class BotPlugin:
-    """插件类，使用该类实例化一个插件
-
-    同时该类会提供各种接口用于注册事件处理器、共享对象、共享对象回调方法和信号处理方法。
-    """
+    """插件类，使用该类实例化一个插件"""
 
     def __init__(
         self,
         id: str,
         version: str,
         desc: str = "",
         doc: str = "",
@@ -173,30 +187,30 @@
         check_pass = all(
             False
             for pair in self.__proxy__.share_cbs
             if pair not in self.__proxy__.shares
         )
         if not check_pass:
             raise PluginInitError(
-                f"插件 {self.__id__} 不能为不属于自己的共享对象注册回调"
+                f"插件 {self.__id__} 不能为不属于自己的共享对象绑定回调"
             )
 
     def on_event(
         self,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
         block: bool = False,
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = False,
         conflict_wait: bool = False,
         conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
     ):
-        """注册一个任意事件处理器
+        """绑定一个任意事件处理方法
 
         :param checker: 使用的检查器，为空则默认通过检查
         :param priority: 优先级
         :param block: 是否进行优先级阻断
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
@@ -239,15 +253,15 @@
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = False,
         conflict_wait: bool = False,
         conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
     ):
-        """注册一个消息事件处理器
+        """绑定一个消息事件处理方法
 
         :param matcher: 使用的匹配器（和解析器二选一）
         :param parser: 使用的解析器（和匹配器二选一）
         :param checker: 使用的检查器，为空则默认通过检查
         :param priority: 优先级
         :param block: 是否进行优先级阻断
         :param temp: 是否是一次性的
@@ -280,65 +294,14 @@
                     ],
                 )
             )
             return executor
 
         return make_args
 
-    def on_every_message(
-        self,
-        checker: Optional["BotChecker"] = None,
-        priority: PriorLevel = PriorLevel.MEAN,
-        block: bool = False,
-        temp: bool = False,
-        session_rule: Optional["SessionRule"] = None,
-        session_hold: bool = False,
-        direct_rouse: bool = False,
-        conflict_wait: bool = False,
-        conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
-    ):
-        """注册一个任意消息事件处理器
-
-        :param checker: 使用的检查器，为空则默认通过检查
-        :param priority: 优先级
-        :param block: 是否进行优先级阻断
-        :param temp: 是否是一次性的
-        :param session_rule: 会话规则，为空则不使用会话规则
-        :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
-        :param direct_rouse: 会话暂停时，是否允许不检查就唤醒会话（有会话规则才可启用）
-        :param conflict_wait: 会话冲突时，是否需要事件等待处理（有会话规则才可启用）
-        :param conflict_cb: 会话冲突时，运行的回调（有会话规则才可启用，`conflict_wait=True`，此参数无效）
-        """
-
-        def make_args(
-            executor: Callable[[], Coroutine[Any, Any, None]]
-        ) -> Callable[[], Coroutine[Any, Any, None]]:
-            self.__handler_args__.append(
-                EventHandlerArgs(
-                    executor=executor,
-                    type=MsgEventHandler,
-                    params=[
-                        None,
-                        None,
-                        checker,
-                        priority,
-                        block,
-                        temp,
-                        session_rule,
-                        session_hold,
-                        direct_rouse,
-                        conflict_wait,
-                        conflict_cb,
-                    ],
-                )
-            )
-            return executor
-
-        return make_args
-
     def on_at_qq(
         self,
         qid: Optional[int] = None,
         matcher: Optional["BotMatcher"] = None,
         parser: Optional["BotParser"] = None,
         checker: Optional["BotChecker"] = None,
         priority: PriorLevel = PriorLevel.MEAN,
@@ -346,15 +309,15 @@
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = False,
         conflict_wait: bool = False,
         conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
     ):
-        """注册一个艾特消息事件处理器
+        """绑定一个艾特消息事件处理方法
 
         消息必须是艾特消息，且匹配成功才能被进一步处理。
 
         :param qid: 被艾特的 qq 号。为空则接受所有艾特消息;不为空则只接受指定 qid 被艾特的艾特消息
         :param matcher: 使用的匹配器（和解析器二选一）
         :param parser: 使用的解析器（和匹配器二选一）
         :param checker: 使用的检查器，为空则默认通过检查
@@ -410,15 +373,15 @@
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = False,
         conflict_wait: bool = False,
         conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
     ):
-        """注册一个字符串起始匹配的消息事件处理器
+        """绑定一个字符串起始匹配的消息事件处理方法
 
         `target` 为字符串时，只进行一次起始匹配，即判断是否匹配成功。
         `target` 为字符串列表时，所有字符串都进行起始匹配，再将所有结果使用给定
         `logic_mode` 计算是否匹配成功。
 
         消息必须匹配成功才能被进一步处理。
 
@@ -472,15 +435,15 @@
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = False,
         conflict_wait: bool = False,
         conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
     ):
-        """注册一个字符串包含匹配的消息事件处理器
+        """绑定一个字符串包含匹配的消息事件处理方法
 
         `target` 为字符串时，只进行一次包含匹配，即判断是否匹配成功。
         `target` 为字符串列表时，所有字符串都进行包含匹配，再将所有结果使用给定
         `logic_mode` 计算是否匹配成功。
 
         消息必须匹配成功才能被进一步处理。
 
@@ -534,15 +497,15 @@
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = False,
         conflict_wait: bool = False,
         conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
     ):
-        """注册一个字符串全匹配的消息事件处理器
+        """绑定一个字符串全匹配的消息事件处理方法
 
         `target` 为字符串时，只进行一次全匹配，即判断是否匹配成功。
         `target` 为字符串列表时，所有字符串都进行全匹配，再将所有结果使用给定
         `logic_mode` 计算是否匹配成功。
 
         消息必须匹配成功才能被进一步处理。
 
@@ -596,15 +559,15 @@
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = False,
         conflict_wait: bool = False,
         conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
     ):
-        """注册一个字符串结尾匹配的消息事件处理器
+        """绑定一个字符串结尾匹配的消息事件处理方法
 
         `target` 为字符串时，只进行一次结尾匹配，即判断是否匹配成功。
         `target` 为字符串列表时，所有字符串都进行结尾匹配，再将所有结果使用给定
         `logic_mode` 计算是否匹配成功。
 
         消息必须匹配成功才能被进一步处理。
 
@@ -657,15 +620,15 @@
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = False,
         conflict_wait: bool = False,
         conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
     ):
-        """注册一个字符串正则匹配的消息事件处理器
+        """绑定一个字符串正则匹配的消息事件处理方法
 
         消息必须匹配成功才能被进一步处理。
 
         :param target: 匹配目标的正则表达式，在匹配时，它应该可以使 :meth:`re.findall` 不返回空列表
         :param checker: 使用的检查器，为空则默认通过检查
         :param priority: 优先级
         :param block: 是否进行优先级阻断
@@ -712,15 +675,15 @@
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = False,
         conflict_wait: bool = False,
         conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
     ):
-        """注册一个请求事件处理器
+        """绑定一个请求事件处理方法
 
         :param checker: 使用的检查器，为空则默认通过检查
         :param priority: 优先级
         :param block: 是否进行优先级阻断
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
@@ -761,15 +724,15 @@
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = False,
         conflict_wait: bool = False,
         conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
     ):
-        """注册一个好友请求事件处理器
+        """绑定一个好友请求事件处理方法
 
         :param checker: 使用的检查器，为空则默认通过检查
         :param priority: 优先级
         :param block: 是否进行优先级阻断
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
@@ -816,15 +779,15 @@
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = False,
         conflict_wait: bool = False,
         conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
     ):
-        """注册一个加群请求事件处理器
+        """绑定一个加群请求事件处理方法
 
         :param checker: 使用的检查器，为空则默认通过检查
         :param priority: 优先级
         :param block: 是否进行优先级阻断
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
@@ -891,15 +854,15 @@
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = False,
         conflict_wait: bool = False,
         conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
     ):
-        """注册一个通知事件处理器
+        """绑定一个通知事件处理方法
 
         :param type: 通知的类型，为 "ALL" 时接受所有通知
         :param checker: 使用的检查器，为空则默认通过检查
         :param priority: 优先级
         :param block: 是否进行优先级阻断
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
@@ -947,15 +910,15 @@
         temp: bool = False,
         session_rule: Optional["SessionRule"] = None,
         session_hold: bool = False,
         direct_rouse: bool = False,
         conflict_wait: bool = False,
         conflict_cb: Optional[Callable[[], Coroutine[Any, Any, None]]] = None,
     ):
-        """注册一个元事件处理器
+        """绑定一个元事件处理方法
 
         :param checker: 使用的检查器，为空则默认通过检查
         :param priority: 优先级
         :param block: 是否进行优先级阻断
         :param temp: 是否是一次性的
         :param session_rule: 会话规则，为空则不使用会话规则
         :param session_hold: 处理方法结束后是否保留会话（有会话规则才可启用）
@@ -985,17 +948,17 @@
                 )
             )
             return executor
 
         return make_args
 
     def on_signal(self, namespace: str, signal: str):
-        """注册一个信号处理方法
+        """绑定一个信号处理方法
 
-        本方法作为异步函数的装饰器使用，此时可注册一个函数为信号处理方法。
+        本方法作为异步函数的装饰器使用，此时可绑定一个函数为信号处理方法。
 
         .. code:: python
 
            # 假设存在一个名为 plugin 的变量，是 BotPlugin 实例
            # 为在命名空间 BaseUtils 中，名为 txt2img 的信号绑定处理方法：
            @plugin.on_signal("BaseUtils", "txt2img")
            async def get_img_of_txt(text: str, format: Any) -> bytes:
@@ -1003,15 +966,15 @@
                # 接下来是具体逻辑
                ...
            # 在这个示例中，具体的功能是为其他插件提供转换大段文本为图片的能力，因为大段文本不便于发送
 
         .. admonition:: 注意
            :class: caution
 
-           在一个 bot 实例的范围内，同命名空间同名称的信号，只能注册一个处理方法。
+           在一个 bot 实例的范围内，同命名空间同名称的信号，只能绑定一个处理方法。
 
         :param namespace: 信号的命名空间
         :param signal: 信号的名称
         """
 
         def make_args(
             func: Callable[P, Coroutine[Any, Any, Any]]
@@ -1050,32 +1013,32 @@
         .. admonition:: 注意
            :class: caution
 
            在一个 bot 实例的范围内，同命名空间同名称的共享对象，只能注册一个。
 
         :param namespace: 共享对象的命名空间
         :param id: 共享对象的 id 标识
-        :param reflector: 为空时，本方法当作异步函数的装饰器使用；否则应该直接使用，此处提供共享对象值获取的反射函数
+        :param reflector: 本方法当作异步函数的装饰器使用时，本参数为空；直接使用本方法时，参数为共享对象值获取的同步函数
         """
         if reflector is not None:
             self.__share_args__.append(ShareObjArgs(namespace, id, to_async(reflector)))
             return
 
         def make_args(
             func: Callable[[], Coroutine[Any, Any, Any]]
         ) -> Callable[[], Coroutine[Any, Any, Any]]:
             self.__share_args__.append(ShareObjArgs(namespace, id, func))
             return func
 
         return make_args
 
     def on_share_affected(self, namespace: str, id: str):
-        """为一个共享对象注册回调方法
+        """为一个共享对象绑定回调方法
 
-        本方法作为异步函数的装饰器使用，此时可为一个共享对象注册回调方法。
+        本方法作为异步函数的装饰器使用，此时可为一个共享对象绑定回调方法。
 
         .. code:: python
 
            # 假设存在一个名为 plugin 的变量，是 BotPlugin 实例
            # 为在命名空间 HelpUtils 中，名为 all_helps 的共享对象绑定回调方法：
            @plugin.on_share_affected("HelpUtils", "all_helps")
            async def add_a_help(text: str) -> bool:
@@ -1084,33 +1047,33 @@
                ...
            # 此回调用于被其他插件触发，为它们提供“影响”共享对象的能力，
            # 在这个示例中，具体的功能是让其他插件可以添加一条自己的帮助信息，但是有所校验
 
         .. admonition:: 注意
            :class: caution
 
-           在一个 bot 实例的范围内，同命名空间同名称的共享对象，只能注册一个回调方法。
-           而且这个共享对象必须在本插件通过 :meth:`on_share` 注册（共享对象注册、共享对象回调注册先后顺序不重要）
+           在一个 bot 实例的范围内，同命名空间同名称的共享对象，只能绑定一个回调方法。
+           而且这个共享对象必须在本插件通过 :meth:`on_share` 注册（共享对象注册、共享对象回调绑定先后顺序不重要）
 
         :param namespace: 共享对象的命名空间
         :param id: 共享对象的 id 标识
         """
 
         def make_args(
             func: Callable[P, Coroutine[Any, Any, Any]]
         ) -> Callable[P, Coroutine[Any, Any, Any]]:
             self.__share_cb_args__.append(ShareObjCbArgs(namespace, id, func))
             return func
 
         return make_args
 
     def on_bot_life(self, type: BotLife):
-        """注册 bot 在某个生命周期的 hook 方法
+        """绑定 bot 在某个生命周期的 hook 方法
 
-        本方法作为异步函数的装饰器使用，此时可注册一个函数为 bot 生命周期 hook 方法。
+        本方法作为异步函数的装饰器使用，此时可绑定一个函数为 bot 生命周期 hook 方法。
 
         .. code:: python
 
            # 假设存在一个名为 plugin 的变量，是 BotPlugin 实例
            # 我们希望这个插件，在 bot 连接器建立连接后给某人发一条消息
            @plugin.on_bot_life(BotLife.CONNECTED)
            async def say_hi() -> None:
@@ -1127,52 +1090,52 @@
             self.__hook_args__.append(BotHookRunnerArgs(func, type))
             return func
 
         return make_args
 
     @property
     def on_plugins_loaded(self):
-        """注册 bot 在 :attr:`.BotLife.LOADED` 生命周期的 hook 方法
+        """绑定 bot 在 :attr:`.BotLife.LOADED` 生命周期的 hook 方法
 
         本方法作为异步函数的装饰器使用。用法与 :class:`on_bot_life` 类似。
         """
         return self.on_bot_life(BotLife.LOADED)
 
     @property
     def on_connected(self):
-        """注册 bot 在 :attr:`.BotLife.CONNECTED` 生命周期的 hook 方法
+        """绑定 bot 在 :attr:`.BotLife.CONNECTED` 生命周期的 hook 方法
 
         本方法作为异步函数的装饰器使用。用法与 :class:`on_bot_life` 类似。
         """
         return self.on_bot_life(BotLife.CONNECTED)
 
     @property
     def on_before_close(self):
-        """注册 bot 在 :attr:`.BotLife.BEFORE_CLOSE` 生命周期的 hook 方法
+        """绑定 bot 在 :attr:`.BotLife.BEFORE_CLOSE` 生命周期的 hook 方法
 
         本方法作为异步函数的装饰器使用。用法与 :class:`on_bot_life` 类似。
         """
         return self.on_bot_life(BotLife.BEFORE_CLOSE)
 
     @property
     def on_before_stop(self):
-        """注册 bot 在 :attr:`.BotLife.BEFORE_STOP` 生命周期的 hook 方法
+        """绑定 bot 在 :attr:`.BotLife.BEFORE_STOP` 生命周期的 hook 方法
 
         本方法作为异步函数的装饰器使用。用法与 :class:`on_bot_life` 类似。
         """
         return self.on_bot_life(BotLife.BEFORE_STOP)
 
     @property
     def on_event_built(self):
-        """注册 bot 在 :attr:`.BotLife.EVENT_BUILT` 生命周期的 hook 方法
+        """绑定 bot 在 :attr:`.BotLife.EVENT_BUILT` 生命周期的 hook 方法
 
         本方法作为异步函数的装饰器使用。用法与 :class:`on_bot_life` 类似。
         """
         return self.on_bot_life(BotLife.EVENT_BUILT)
 
     @property
     def on_action_presend(self):
-        """注册 bot 在 :attr:`.BotLife.ACTION_PRESEND` 生命周期的 hook 方法
+        """绑定 bot 在 :attr:`.BotLife.ACTION_PRESEND` 生命周期的 hook 方法
 
         本方法作为异步函数的装饰器使用。用法与 :class:`on_bot_life` 类似。
         """
         return self.on_bot_life(BotLife.ACTION_PRESEND)
```

### Comparing `melobot-2.5.8/src/melobot/plugin/ipc.py` & `melobot-2.5.9/src/melobot/plugin/ipc.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             raise ShareObjError(f"共享对象回调指定的命名空间 {namespace} 不存在")
         if id not in self.store[namespace].keys():
             raise ShareObjError(
                 f"共享对象回调指定的命名空间中，不存在标记为 {id} 的共享对象"
             )
         if self.store[namespace][id].__cb_set.is_set():
             raise ShareObjError(
-                f"{namespace} 中标记为 {id} 的共享对象已被注册过回调，拒绝再次注册"
+                f"{namespace} 中标记为 {id} 的共享对象已被绑定过回调，拒绝再次绑定"
             )
         self.store[namespace][id]._fill_cb(cb)
 
     def get(self, namespace: str, id: str) -> ShareObject:
         """获取共享对象."""
         if namespace not in self.store.keys():
             raise ShareObjError(
@@ -85,15 +85,15 @@
             )
         if id not in self.store[namespace].keys():
             raise ShareObjError(f"无法获取不存在的共享对象：标识 {id} 不存在")
         return self.store[namespace][id]
 
 
 class PluginSignalHandler:
-    """插件信号处理器."""
+    """插件信号处理器"""
 
     def __init__(
         self, namespace: str, signal: str, func: Callable[..., Coroutine[Any, Any, Any]]
     ) -> None:
         self.cb = func
         self.namespace = namespace
         self.signal = signal
@@ -108,15 +108,15 @@
 
     def _bind(self, logger: "Logger") -> None:
         self.logger = logger
 
     def register(
         self, namespace: str, signal: str, func: Callable[..., Coroutine[Any, Any, Any]]
     ) -> None:
-        """注册一个插件信号处理方法。由 plugin build 过程调用."""
+        """绑定一个插件信号处理方法。由 plugin build 过程调用."""
         if namespace not in self.store.keys():
             self.store[namespace] = {}
         if signal in self.store[namespace].keys():
             raise PluginSignalError("同一命名空间的同一信号只能绑定一个处理函数")
         self.store[namespace][signal] = PluginSignalHandler(namespace, signal, func)
 
     async def _run_on_ctx(
```

### Comparing `melobot-2.5.8/src/melobot/utils/__init__.py` & `melobot-2.5.9/src/melobot/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,29 +4,29 @@
     GroupMsgLvlChecker,
     GroupReqChecker,
     MsgCheckerGen,
     MsgLvlChecker,
     NoticeTypeChecker,
     PrivateMsgLvlChecker,
 )
-from .formatter import ArgFormatter, FormatInfo
+from .formatter import CmdArgFormatter, FormatInfo
 from .logger import BotLogger
 from .matcher import ContainMatcher, EndMatcher, FullMatcher, RegexMatcher, StartMatcher
 from .parser import CmdParser, CmdParserGen
 
 __all__ = (
     "AtChecker",
     "FriendReqChecker",
     "GroupMsgLvlChecker",
     "GroupReqChecker",
     "MsgCheckerGen",
     "MsgLvlChecker",
     "NoticeTypeChecker",
     "PrivateMsgLvlChecker",
-    "ArgFormatter",
+    "CmdArgFormatter",
     "FormatInfo",
     "BotLogger",
     "ContainMatcher",
     "EndMatcher",
     "FullMatcher",
     "RegexMatcher",
     "StartMatcher",
```

### Comparing `melobot-2.5.8/src/melobot/utils/checker.py` & `melobot-2.5.9/src/melobot/utils/checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
         """
         super().__init__(None, None)
         self.qid = qid if qid is not None else None
 
     async def check(self, event: "MessageEvent") -> bool:  # type: ignore
         if not event.is_msg_event():
             return False
-        id_list = event.get_cq_params("at", "qq")
+        id_list = event.get_datas("at", "qq")
         if self.qid is None:
             status = len(id_list) > 0
         else:
             for id in id_list:
                 if id == self.qid:
                     status = True
                     break
```

### Comparing `melobot-2.5.8/src/melobot/utils/formatter.py` & `melobot-2.5.9/src/melobot/utils/formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,33 +29,33 @@
         self,
         src: str | VoidType,
         src_desc: Optional[str],
         src_expect: Optional[str],
         idx: int,
         exc_type: Exception,
         exc_tb: ModuleType,
-        cmd_name: str,
+        group_id: str,
     ) -> None:
         #: 命令参数格式化前的原值
         self.src = src
         #: 命令参数值的功能描述
         self.src_desc = src_desc
         #: 命令参数值的值期待描述
         self.src_expect = src_expect
         #: 命令参数值的顺序（从 0 开始索引）
         self.idx = idx
         #: 命令参数格式化异常时的异常对象
         self.exc_type = exc_type
         #: 命令参数格式化异常时的调用栈信息
         self.exc_tb = exc_tb
         #: 命令参数所属命令的命令名
-        self.cmd_name = cmd_name
+        self.group_id = group_id
 
 
-class ArgFormatter:
+class CmdArgFormatter:
     """命令参数格式化器
 
     用于格式化命令解析器解析出的命令参数。
     """
 
     def __init__(
         self,
@@ -108,15 +108,15 @@
             args.vals = [self.default]
         elif len(args.vals) < idx + 1:
             args.vals.append(self.default)
         return args.vals[idx]
 
     async def format(
         self,
-        cmd_name: str,
+        group_id: str,
         args: ParseArgs,
         idx: int,
     ) -> bool:
         # 格式化参数为对应类型的变量
         try:
             src = self._get_val(args, idx)
             if (
@@ -132,33 +132,33 @@
                 pass
             else:
                 raise ArgVerifyFailed
             args.vals[idx] = res  # type: ignore
             return True
         except ArgVerifyFailed as e:
             info = FormatInfo(
-                src, self.src_desc, self.src_expect, idx, e, traceback, cmd_name
+                src, self.src_desc, self.src_expect, idx, e, traceback, group_id
             )
             if self.verify_fail:
                 await self.verify_fail(info)
             else:
                 await self._verify_fail_default(info)
             return False
         except ArgLackError as e:
             info = FormatInfo(
-                Void, self.src_desc, self.src_expect, idx, e, traceback, cmd_name
+                Void, self.src_desc, self.src_expect, idx, e, traceback, group_id
             )
             if self.arg_lack:
                 await self.arg_lack(info)
             else:
                 await self._arglack_default(info)
             return False
         except Exception as e:
             info = FormatInfo(
-                src, self.src_desc, self.src_expect, idx, e, traceback, cmd_name
+                src, self.src_desc, self.src_expect, idx, e, traceback, group_id
             )
             if self.convert_fail:
                 await self.convert_fail(info)
             else:
                 await self._convert_fail_default(info)
             return False
 
@@ -169,28 +169,28 @@
         tip += (
             f"（{info.src_desc}）无法处理，给定的值为：{src}。"
             if info.src_desc
             else f"给定的值 {src} 无法处理。"
         )
         tip += f"参数要求：{info.src_expect}。" if info.src_expect else ""
         tip += f"\n详细错误描述：[{e_class}] {info.exc_type}"
-        tip = f"命令 {info.cmd_name} 参数格式化失败：\n" + tip
+        tip = f"命令 {info.group_id} 参数格式化失败：\n" + tip
         await send(tip)
 
     async def _verify_fail_default(self, info: FormatInfo) -> None:
         src = info.src.__repr__() if isinstance(info.src, str) else info.src
         tip = f"第 {info.idx+1} 个参数"
         tip += (
             f"（{info.src_desc}）不符合要求，给定的值为：{src}。"
             if info.src_desc
             else f"给定的值 {src} 不符合要求。"
         )
         tip += f"参数要求：{info.src_expect}。" if info.src_expect else ""
-        tip = f"命令 {info.cmd_name} 参数格式化失败：\n" + tip
+        tip = f"命令 {info.group_id} 参数格式化失败：\n" + tip
         await send(tip)
 
     async def _arglack_default(self, info: FormatInfo) -> None:
         tip = f"第 {info.idx+1} 个参数"
         tip += f"（{info.src_desc}）缺失。" if info.src_desc else "缺失。"
         tip += f"参数要求：{info.src_expect}。" if info.src_expect else ""
-        tip = f"命令 {info.cmd_name} 参数格式化失败：\n" + tip
+        tip = f"命令 {info.group_id} 参数格式化失败：\n" + tip
         await send(tip)
```

### Comparing `melobot-2.5.8/src/melobot/utils/logger.py` & `melobot-2.5.9/src/melobot/utils/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,24 +145,24 @@
         handler = self._file_handler(
             self._file_fmt(self.name, self._no_tag), log_dir, self.name
         )
         self.addHandler(handler)
         self._handler_arr.append(handler)
 
     def setLevel(self, level: Literal["DEBUG", "ERROR", "INFO", "WARNING", "CRITICAL"]) -> None:  # type: ignore
+        """设置日志等级
+
+        日志等级自动应用于包含的所有 handler
+
+        :param level: 日志等级字面量
+        """
         super().setLevel(level)
         for handler in self._handler_arr:
             handler.setLevel(level)
 
-    # def to_console(self) -> None:
-    #     self._add_console_handler()
-
-    # def to_dir(self, log_dir: str) -> None:
-    #     self._add_file_handler(log_dir)
-
 
 _SysExcInfoType: TypeAlias = (
     tuple[Type[BaseException], BaseException, Optional[TracebackType]]
     | tuple[None, None, None]
 )
 _ExcInfoType: TypeAlias = None | bool | _SysExcInfoType | BaseException
```

### Comparing `melobot-2.5.8/src/melobot/utils/matcher.py` & `melobot-2.5.9/src/melobot/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/src/melobot/utils/parser.py` & `melobot-2.5.9/src/melobot/utils/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import re
 
 from ..base.abc import BotParser
 from ..base.exceptions import ArgParseError
 from ..base.typing import TYPE_CHECKING, Optional, ParseArgs
 
 if TYPE_CHECKING:
-    from .formatter import ArgFormatter
+    from .formatter import CmdArgFormatter
 
 
 class CmdParser(BotParser):
     """命令解析器
 
     通过解析命令名和命令参数的形式，解析字符串。
     """
 
     def __init__(
         self,
         cmd_start: str | list[str],
         cmd_sep: str | list[str],
         target: str | list[str],
-        formatters: Optional[list[Optional["ArgFormatter"]]] = None,
+        formatters: Optional[list[Optional["CmdArgFormatter"]]] = None,
     ) -> None:
         """初始化一个命令解析器
 
         .. admonition:: 注意
            :class: caution
 
            - 命令起始符和命令间隔符不允许包含：引号，各种括号，反斜杠，数字，英文，控制字符及各类空白字符。
@@ -100,37 +100,37 @@
                 s[0]: ParseArgs(s[1:]) if len(s) > 1 else ParseArgs(None)
                 for s in str_list
             }
         else:
             return None
 
     def test(
-        self, args_group: dict[str, ParseArgs] | None
+        self, args_dict: dict[str, ParseArgs] | None
     ) -> tuple[bool, Optional[str], Optional[ParseArgs]]:
         # 测试是否匹配。返回三元组：（是否匹配成功，匹配成功的命令名，匹配成功的命令参数）。
         # 最后两个返回值若不存在，则返回 None。
-        if args_group is None:
+        if args_dict is None:
             return (False, None, None)
-        for cmd_name in args_group.keys():
-            if cmd_name in self.target:
-                return (True, cmd_name, args_group[cmd_name])
+        for group_id in args_dict.keys():
+            if group_id in self.target:
+                return (True, group_id, args_dict[group_id])
         return (False, None, None)
 
-    async def format(self, cmd_name: str, args: ParseArgs) -> bool:
+    async def format(self, group_id: str, args: ParseArgs) -> bool:
         # 格式化命令解析参数
-        if args.formatted:
+        if hasattr(args, "formatted"):
             return True
         for idx, formatter in enumerate(self.formatters):
             if formatter is None:
                 continue
-            status = await formatter.format(cmd_name, args, idx)
+            status = await formatter.format(group_id, args, idx)
             if not status:
                 return False
         args.vals = args.vals[: len(self.formatters)]  # type: ignore
-        args.formatted = True
+        args.formatted = True  # type: ignore
         return True
 
 
 class CmdParserGen:
     """命令解析器的生成器
 
     预先存储命令起始符和命令间隔符，指定匹配的命令名后返回一个命令解析器。
@@ -150,15 +150,15 @@
         """
         self.cmd_start = cmd_start
         self.cmd_sep = cmd_sep
 
     def gen(
         self,
         target: str | list[str],
-        formatters: Optional[list[Optional["ArgFormatter"]]] = None,
+        formatters: Optional[list[Optional["CmdArgFormatter"]]] = None,
     ) -> CmdParser:
         """生成匹配指定命令名的命令解析器
 
         :param target: 匹配的命令名
         :param formatters: 格式化器列表（列表可以包含空值，即此位置的参数无格式化选项）
         """
         return CmdParser(self.cmd_start, self.cmd_sep, target, formatters)
```

### Comparing `melobot-2.5.8/tests/private/2939fc304d7d88447f460b76aa9d7199.jpeg` & `melobot-2.5.9/tests/private/2939fc304d7d88447f460b76aa9d7199.jpeg`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/tests/private/TODO.txt` & `melobot-2.5.9/tests/private/TODO.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 
 会话（会话是什么？会话普遍存在，会话的生命周期，自定义会话，会话规则及定义，自定义会话的使用）
 
 跨插件通信之信号（跨插件通信的准则，信号的目的，原理与使用方法）
 
 跨插件通信之共享对象（共享对象的目的，原理与使用方法）
 
-多 bot 协同工作
+多 bot 协同工作
```

### Comparing `melobot-2.5.8/tests/private/__main__.py` & `melobot-2.5.9/tests/private/__main__.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/tests/private/main.py` & `melobot-2.5.9/tests/private/main.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/tests/private/output.png` & `melobot-2.5.9/tests/private/output.png`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/tests/private/output.svg` & `melobot-2.5.9/tests/private/output.svg`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/tests/private/procedure.txt` & `melobot-2.5.9/tests/private/procedure.txt`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/tests/private/qjson.json` & `melobot-2.5.9/tests/private/qjson.json`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/tests/private/templates/draw.py` & `melobot-2.5.9/tests/private/templates/draw.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/tests/private/templates/sdapi/api.py` & `melobot-2.5.9/tests/private/templates/sdapi/api.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/tests/private/templates/sdapi/api_help.py` & `melobot-2.5.9/tests/private/templates/sdapi/api_help.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/tests/private/templates/sdapi/sd_test.py` & `melobot-2.5.9/tests/private/templates/sdapi/sd_test.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/tests/private/templates/sdapi/test.png` & `melobot-2.5.9/tests/private/templates/sdapi/test.png`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/tests/private/test.py` & `melobot-2.5.9/tests/private/test.py`

 * *Files identical despite different names*

### Comparing `melobot-2.5.8/PKG-INFO` & `melobot-2.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melobot
-Version: 2.5.8
+Version: 2.5.9
 Summary: A qq bot development framework with friendly APIs, session control and plugin-supported.
 Author-Email: aicorein <melodyecho@glowmem.com>
 License: AGPL3
 Project-URL: Homepage, https://github.com/aicorein/melobot
 Requires-Python: >=3.10
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: uvloop>=0.17.0; platform_system == "Linux"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: melobot Version: 2.5.8 Summary: A qq bot
+Metadata-Version: 2.1 Name: melobot Version: 2.5.9 Summary: A qq bot
 development framework with friendly APIs, session control and plugin-supported.
 Author-Email: aicorein
 glowmem.com> License: AGPL3 Project-URL: Homepage, https://github.com/aicorein/
 melobot Requires-Python: >=3.10 Requires-Dist: coloredlogs>=15.0.1 Requires-
 Dist: uvloop>=0.17.0; platform_system == "Linux" Requires-Dist:
 websockets>=10.4 Requires-Dist: better-exceptions==0.3.3 Requires-Dist:
 rich>=13.7.1 Requires-Dist: typing-extensions>=4.10.0 Requires-Dist:
```


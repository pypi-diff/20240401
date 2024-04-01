# Comparing `tmp/uvlog-0.1.0-py3-none-any.whl.zip` & `tmp/uvlog-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 13006 bytes, number of entries: 7
--rw-r--r--  2.0 unx      363 b- defN 24-Apr-01 07:48 uvlog/__init__.py
--rw-r--r--  2.0 unx    31374 b- defN 24-Apr-01 07:22 uvlog/uvlog.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-01 07:52 uvlog-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     7421 b- defN 24-Apr-01 07:52 uvlog-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 07:52 uvlog-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-01 07:52 uvlog-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      520 b- defN 24-Apr-01 07:52 uvlog-0.1.0.dist-info/RECORD
-7 files, 40845 bytes uncompressed, 12092 bytes compressed:  70.4%
+Zip file size: 13851 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      363 b- defN 24-Apr-01 20:38 uvlog/__init__.py
+-rw-r--r--  2.0 unx    34859 b- defN 24-Apr-01 20:37 uvlog/uvlog.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-01 20:38 uvlog-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7840 b- defN 24-Apr-01 20:38 uvlog-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 20:38 uvlog-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-01 20:38 uvlog-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      520 b- defN 24-Apr-01 20:38 uvlog-0.1.1.dist-info/RECORD
+7 files, 44749 bytes uncompressed, 12937 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: uvlog/__init__.py
 Comment: 
 
 Filename: uvlog/uvlog.py
 Comment: 
 
-Filename: uvlog-0.1.0.dist-info/LICENSE
+Filename: uvlog-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: uvlog-0.1.0.dist-info/METADATA
+Filename: uvlog-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: uvlog-0.1.0.dist-info/WHEEL
+Filename: uvlog-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: uvlog-0.1.0.dist-info/top_level.txt
+Filename: uvlog-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: uvlog-0.1.0.dist-info/RECORD
+Filename: uvlog-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## uvlog/__init__.py

```diff
@@ -3,15 +3,15 @@
 import atexit
 
 from uvlog.uvlog import *
 
 __python_version__ = "3.8"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "MIT"
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 add_formatter_type(TextFormatter)
 add_formatter_type(JSONFormatter)
 add_handler_type(StreamHandler)
 add_handler_type(QueueHandler)
 configure(BASIC_CONFIG)
 atexit.register(clear)
```

## uvlog/uvlog.py

```diff
@@ -4,30 +4,30 @@
 import logging
 import os
 import queue
 import sys
 import traceback
 from abc import abstractmethod
 from collections import ChainMap
-from contextvars import ContextVar
-from copy import deepcopy
+from contextvars import ContextVar  # noqa: pycharm bug?
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
 from json import dumps
+from random import random
+from pathlib import Path
 from threading import Thread
 from typing import (
     Any,
     BinaryIO,
     Callable,
     ClassVar,
     Collection,
     Literal,
     Mapping,
-    NamedTuple,
     Optional,
     Protocol,
     TypedDict,
     cast,
     no_type_check,
     Type,
     Dict,
@@ -52,92 +52,93 @@
     "set_logger_type",
     "add_handler",
     "add_formatter",
     "remove_handler",
     "get_logger",
     "configure",
     "clear",
+    "DEBUG",
+    "INFO",
+    "WARNING",
+    "ERROR",
+    "CRITICAL",
 ]
 
 LOG_CONTEXT: ContextVar[Optional[Dict[str, Any]]] = ContextVar(
     "LOG_CONTEXT", default=None
 )  #: default log context
 
 
 class Stream(Enum):
-    """Default log streams."""
+    """List of default log streams."""
 
     stdout = sys.stdout.buffer
     stderr = sys.stderr.buffer
 
 
-_LevelName = Literal["NOTSET", "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
-_default_timespec = "seconds"
-_default_format = "{asctime} | {levelname} | {name} | {message} | {extra} | {ctx}"
+DEBUG = "DEBUG"
+INFO = "INFO"
+WARNING = "WARNING"
+ERROR = "ERROR"
+CRITICAL = "CRITICAL"
+
 _root_logger_name = ""
+_default_timespec = "seconds"
+_default_format = "{asctime} | {level} | {name} | {message} | {extra} | {ctx}"
 _formatter_types: Dict[str, Type["Formatter"]] = {}
-_handler_types: Dict[str, Type["Handler"]] = {}
-_handlers: Dict[str, "Handler"] = {}
-_formatters: Dict[str, "Formatter"] = {}
-_loggers_persistent: Dict[str, "Logger"] = {}
-_loggers_temp: WeakValueDictionary = WeakValueDictionary()
-_loggers: ChainMap = ChainMap(_loggers_persistent, _loggers_temp)
-_name_to_level: Dict[_LevelName, int] = {
-    "NOTSET": logging.NOTSET,
-    "DEBUG": logging.DEBUG,
-    "INFO": logging.INFO,
-    "WARNING": logging.WARNING,
-    "ERROR": logging.ERROR,
-    "CRITICAL": logging.CRITICAL,
-}
 
 
 class _DictConfig(TypedDict, total=False):
     loggers: Dict[str, dict]
     handlers: Dict[str, dict]
     formatters: Dict[str, dict]
 
 
 BASIC_CONFIG: _DictConfig = {
-    "loggers": {_root_logger_name: {"levelname": "INFO", "handlers": ["stderr"]}},
+    "loggers": {_root_logger_name: {}},
     "handlers": {
-        Stream.stderr.name: {
-            "type": "StreamHandler",
-            "dest": Stream.stderr.name,
-            "levelname": "DEBUG",
-            "formatter": "text",
-        },
-        Stream.stdout.name: {
-            "type": "StreamHandler",
-            "dest": Stream.stdout.name,
-            "levelname": "DEBUG",
-            "formatter": "text",
-        },
+        Stream.stderr.name: {},
+        Stream.stdout.name: {},
     },
     "formatters": {
-        "text": {
-            "type": "TextFormatter",
-            "timespec": _default_timespec,
-            "format_str": _default_format,
-        },
-        "json": {"type": "JSONFormatter"},
+        "text": {"class": "TextFormatter"},
+        "json": {"class": "JSONFormatter"},
     },
 }  #: default log configuration
 
+_LevelName = Literal["NOTSET", "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
+_handler_types: Dict[str, Type["Handler"]] = {}
+_handlers: Dict[str, "Handler"] = {}
+_formatters: Dict[str, "Formatter"] = {}
+_loggers_persistent: Dict[str, "Logger"] = {}
+_loggers_temp: WeakValueDictionary = WeakValueDictionary()
+_loggers: ChainMap = ChainMap(_loggers_persistent, _loggers_temp)
+_name_to_level: Dict[_LevelName, int] = {
+    "NOTSET": logging.NOTSET,
+    "DEBUG": logging.DEBUG,
+    "INFO": logging.INFO,
+    "WARNING": logging.WARNING,
+    "ERROR": logging.ERROR,
+    "CRITICAL": logging.CRITICAL,
+}
+
 
-class LogRecord(NamedTuple):
+@dataclass
+class LogRecord:
     """Log record object.
 
     A log record object is created when a log method of a logger is called.
     """
 
+    __slots__ = ('name', 'level', 'levelno', 'asctime', 'filename', 'lineno', 'func', 'message', 'exc_info', 'extra', 'ctx')
+
     name: str
     """Logger name"""
 
-    levelname: _LevelName
+    level: _LevelName
     """Log record level name"""
 
     levelno: int
     """Log record level number"""
 
     asctime: datetime
     """Timestamp of record creation"""
@@ -159,51 +160,71 @@
 
     func: Optional[str]
     """Function name of the caller"""
 
     lineno: Optional[int]
     """Source code line number of the caller"""
 
+    def __getitem__(self, item: str, /):
+        return getattr(self, item)
+
 
 class Formatter(Protocol):
-    """Log formatter interface."""
+    """Log formatter interface.
+
+    It's a protocol class, i.e. one doesn't need to inherit from it to create a valid formatter.
+    """
 
     @abstractmethod
-    def format(self, record: LogRecord, /) -> bytes:
-        """Format a log record for output."""
+    def format_record(self, record: LogRecord, /) -> bytes: ...
 
 
 class Handler(Protocol):
-    """Log handler interface."""
+    """Log handler interface.
+
+    It's a protocol class, i.e. one doesn't need to inherit from it to create a valid handler.
+    """
 
     @abstractmethod
-    def handle(self, record: LogRecord, /) -> None:
-        """Handle a log record."""
+    def handle(self, record: LogRecord, /) -> None: ...
 
     @abstractmethod
-    def set_level(self, level: _LevelName, /) -> None:
-        """Set log level for this handler."""
+    def set_level(self, level: _LevelName, /) -> None: ...
 
     @abstractmethod
-    def set_formatter(self, fmt: Formatter, /) -> None:
-        """Set log formatter for this handler."""
+    def set_formatter(self, fmt: Formatter, /) -> None: ...
 
     @abstractmethod
     def set_destination(self, dest: str, /) -> None:
-        """Set handler destination
+        """Set a handler destination.
+
+        Since only one destination allowed for a single handler, this method must call :py:func:`~uvlog.add_handler`
+        to ensure that a handler for this destination doesn't exist. It also should call
+        :py:func:`~uvlog.remove_handler` for its previous destination before adding a new one.
+
+        Example:
+
+        .. code-block:: python
+
+            def set_destination(self, dest: str, /) -> None:
+                remove_handler(self._dest)
+                self._dest = dest
+                ...
+                add_handler(dest)
 
-        This method must call `add_handler` to ensure that a handler for this destination doesn't exist. It also
-        should call `remove_handler` for his previous destination before setting a new one.
         """
         # remove_handler(self.dest)
         # add_handler(dest, self)
 
     @abstractmethod
     def close(self) -> None:
-        """Close handler and the associated stream."""
+        """Close the handler including all connections to its destination.
+
+        This method is called automatically at exit for each added handler by the :py:func:`~uvlog.clear` function.
+        """
 
 
 def add_formatter_type(typ: Type[Formatter], /) -> None:
     _formatter_types[typ.__name__] = typ
 
 
 def add_handler_type(typ: Type[Handler], /) -> None:
@@ -211,84 +232,107 @@
 
 
 def add_formatter(name: str, formatter: Formatter, /) -> None:
     _formatters[name] = formatter
 
 
 def add_handler(destination: str, handler: Handler, /) -> None:
-    """Add a handler for a specific destination.
-
-    :param destination: handler destination (depends on a handler type), can be an url, a file name, etc
-    :param handler: handler to add
-
-    Generally it's a good idea to use URL format for destinations, i.e. https:// or file:/// etc.
-    """
     if destination in _handlers:
         raise ValueError(
             f"handler already exists for this destination: {destination}\n\n"
             f"Fix: ensure you don't have two handlers with the same destination, or use "
             f"`uvlog.remove_handler(<dest>)` method to remove a conflicting handler"
         )
     _handlers[destination] = handler
 
 
 def remove_handler(destination: str, /) -> None:
-    """Remove a handler for a specific destination."""
     handler = _handlers.pop(destination, None)
     if handler is not None:
         handler.close()
 
 
 @dataclass
 class Logger:
-    """Logger object."""
+    """Logger object.
+
+    It can be used almost like a standard Python logger, except that it allows passing keyword arguments
+    directly to `extra`:
+
+    .. code-block:: python
+
+        main_logger = uvlog.get_logger('app')
+        logger = main_logger.get_child('my_service')
+
+        logger.debug('debug message', debug_value=42)
+        logger.error('error happened', exc_info=Exception())
+
+    """
 
     name: str
     """Logger name"""
 
-    levelname: _LevelName = "INFO"
-    """Current logging level"""
+    level: _LevelName = "INFO"
+    """Logging level"""
 
     handlers: List[Handler] = field(default_factory=list)
     """List of attached log handlers"""
 
+    sample_rate: float = 1.0
+    """Log records sample rate which determines a probability at which a record should be sampled.
+    
+    Sample rate is not considered for levels above 'INFO'. Values >= 1 disable the sampling mechanism.
+    """
+
+    sample_propagate: bool = True
+    """By default the sampling mechanism is contextual meaning that if there's a non-empty log context,
+    the log chain is marked 'sampled' as it sampled by the first logger in a chain. Once a record is 'sampled' the
+    log chain cannot be *unsampled*, i.e. all subsequent loggers will be forced to sample it as well.
+    It allows to preserve an entire request log chain in the logs and not just some random not connected logs.
+    """
+
     context: ContextVar[Optional[Dict[str, Any]]] = LOG_CONTEXT
-    """Log context variable - useful for contextual data"""
+    """Log context variable - useful for contextual data,
+    see `contextvars <https://docs.python.org/3/library/contextvars.html>`_
+    """
 
     capture_trace: bool = False
-    """Capture traceback for each call (and not just errors) - affects performance"""
+    """Capture traceback for each call such as line numbers, file names etc. — may affect performance"""
 
     _levelno: int = field(init=False, default=0)
     _parent: Optional["Logger"] = field(init=False, default=None)
 
     def __post_init__(self) -> None:
-        self._levelno = _name_to_level[self.levelname]
+        self._levelno = _name_to_level[self.level]
+        self.sample_rate = min(max(0.0, self.sample_rate), 1.0)
 
     def set_level(self, level: _LevelName, /) -> None:
         self._levelno = _name_to_level[level]
-        self.levelname = level
+        self.level = level
 
     def get_child(self, name: str, /, *, persistent: bool = False) -> "Logger":
-        """Get or create a child logger.
+        """Get or create a child logger inheriting all the logger settings.
 
-        :param name: child logger name added to the parent logger name
-        :param persistent: create a persistent logger and store it forever (by default a temp logger is created)
+        .. attention::
+
+            Note that by default a new logger is not *persistent*, i.e. it will be eventually garbage collected if
+            there are no live references to it.
         """
         if "." in name:
             raise ValueError(
                 '"." symbol is not allowed in logger names when calling `get_child` directly\n\n'
                 "Fix: if you want to create a chain of loggers "
                 "use `uvlog.get_logger()` function instead"
             )
         if name in _loggers:
             return _loggers[name]
         child_name = name if self.name == _root_logger_name else f"{self.name}.{name}"
         child_logger = _logger_type(
             name=child_name,
-            levelname=self.levelname,
+            level=self.level,
             context=self.context,
             handlers=[*self.handlers],
             capture_trace=self.capture_trace,
         )  # noqa
         child_logger._parent = self
         if persistent:
             _loggers_persistent[name] = child_logger
@@ -303,28 +347,31 @@
         exc_info: Optional[Exception] = None,
         stack_info=None,
         stacklevel=1,
         **kws,
     ) -> None:
         if self._levelno > logging.CRITICAL:
             return
+        ctx = self.context.get()
+        if ctx and self.sample_rate < 1:
+            ctx["_sample"] = True
         fn, lno, func, _ = (
             _find_caller(stack_info, stacklevel)
             if self.capture_trace
             else (None, None, None, None)
         )
         record = LogRecord(
             self.name,
             "CRITICAL",
             logging.CRITICAL,
             datetime.now(),
-            msg,
+            msg.format_map(kws),
             exc_info,
             kws if kws else None,
-            self.context.get(),
+            ctx,
             fn,
             func,
             lno,
         )
         for handler in self.handlers:
             handler.handle(record)
 
@@ -335,28 +382,31 @@
         exc_info: Optional[Exception] = None,
         stack_info=None,
         stacklevel=1,
         **kws,
     ) -> None:
         if self._levelno > logging.ERROR:
             return
+        ctx = self.context.get()
+        if ctx and self.sample_rate < 1:
+            ctx["_sample"] = True
         fn, lno, func, _ = (
             _find_caller(stack_info, stacklevel)
             if self.capture_trace
             else (None, None, None, None)
         )
         record = LogRecord(
             self.name,
             "ERROR",
             logging.ERROR,
             datetime.now(),
-            msg,
+            msg.format_map(kws),
             exc_info,
             kws if kws else None,
-            self.context.get(),
+            ctx,
             fn,
             func,
             lno,
         )
         for handler in self.handlers:
             handler.handle(record)
 
@@ -367,28 +417,31 @@
         exc_info: Optional[Exception] = None,
         stack_info=None,
         stacklevel=1,
         **kws,
     ) -> None:
         if self._levelno > logging.WARNING:
             return
+        ctx = self.context.get()
+        if ctx and self.sample_rate < 1:
+            ctx["_sample"] = True
         fn, lno, func, _ = (
             _find_caller(stack_info, stacklevel)
             if self.capture_trace
             else (None, None, None, None)
         )
         record = LogRecord(
             self.name,
             "WARNING",
             logging.WARNING,
             datetime.now(),
-            msg,
+            msg.format_map(kws),
             exc_info,
             kws if kws else None,
-            self.context.get(),
+            ctx,
             fn,
             func,
             lno,
         )
         for handler in self.handlers:
             handler.handle(record)
 
@@ -399,28 +452,37 @@
         exc_info: Optional[Exception] = None,
         stack_info=None,
         stacklevel=1,
         **kws,
     ) -> None:
         if self._levelno > logging.INFO:
             return
+        ctx = self.context.get()
+        if ctx and self.sample_rate < 1:
+            _sample = ctx.get("_sample")
+            if _sample is None:
+                _sample = random() < self.sample_rate
+                if self.sample_propagate:
+                    ctx["_sample"] = _sample
+            if not _sample:
+                return
         fn, lno, func, _ = (
             _find_caller(stack_info, stacklevel)
             if self.capture_trace
             else (None, None, None, None)
         )
         record = LogRecord(
             self.name,
             "INFO",
             logging.INFO,
             datetime.now(),
-            msg,
+            msg.format_map(kws),
             exc_info,
             kws if kws else None,
-            self.context.get(),
+            ctx,
             fn,
             func,
             lno,
         )
         for handler in self.handlers:
             handler.handle(record)
 
@@ -431,28 +493,37 @@
         exc_info: Optional[Exception] = None,
         stack_info=None,
         stacklevel=1,
         **kws,
     ) -> None:
         if self._levelno > logging.DEBUG:
             return
+        ctx = self.context.get()
+        if ctx and self.sample_rate < 1:
+            _sample = ctx.get("_sample")
+            if _sample is None:
+                _sample = random() < self.sample_rate
+                if self.sample_propagate:
+                    ctx["_sample"] = _sample
+            if not _sample:
+                return
         fn, lno, func, _ = (
             _find_caller(stack_info, stacklevel)
             if self.capture_trace
             else (None, None, None, None)
         )
         record = LogRecord(
             self.name,
             "DEBUG",
             logging.DEBUG,
             datetime.now(),
-            msg,
+            msg.format_map(kws),
             exc_info,
             kws if kws else None,
-            self.context.get(),
+            ctx,
             fn,
             func,
             lno,
         )
         for handler in self.handlers:
             handler.handle(record)
 
@@ -531,39 +602,52 @@
 
 
 @dataclass
 class TextFormatter:
     """Text log formatter.
 
     Creates human-readable log output.
+
+    Formatter settings can be set directly.
+
+    .. code-block:: python
+
+        _formatter = TextFormatter()
+        _formatter.timestamp_separator = ' '
+
     """
 
     timespec: str = field(init=False, default=_default_timespec)
-    """Timestamp precision for ISO timestamps"""
+    """Precision for ISO timestamps,
+    see `datetime.isoformat() <https://docs.python.org/3/library/datetime.html#datetime.datetime.isoformat>`_"""
 
     timestamp_separator: str = field(init=False, default="T")
-    """Timestamp separator for ISO timestamps"""
+    """Timestamp separator for ISO timestamps,
+    see `datetime.isoformat() <https://docs.python.org/3/library/datetime.html#datetime.datetime.isoformat>`_"""
 
-    format_string: str = field(init=False, default=_default_format)
-    """Log record format"""
+    format: str = field(init=False, default=_default_format)
+    """Log record format, a python f-string,
+    the available keys can be seen in :py:class:`~uvlog.LogRecord` type
+    """
 
-    def format(self, record: LogRecord, /) -> bytes:
-        t = record.asctime.isoformat(
-            timespec=self.timespec, sep=self.timestamp_separator
-        )
-        message = self.format_string.format(
-            asctime=t,
-            levelname=record.levelname,
-            name=record.name,
-            message=record.message,
-            extra=record.extra,
-            ctx=record.ctx,
-            filename=record.filename,
-            lineno=record.lineno,
-            func=record.func,
+    def format_record(self, record: LogRecord, /) -> bytes:
+        message = self.format.format_map(
+            {
+                "asctime": record.asctime.isoformat(
+                    timespec=self.timespec, sep=self.timestamp_separator
+                ),
+                "level": record.level,
+                "name": record.name,
+                "message": record.message,
+                "filename": record.filename,
+                "func": record.func,
+                "lineno": record.lineno,
+                "extra": record.extra,
+                "ctx": record.ctx,
+            }
         )
         if record.exc_info is not None:
             exc_info = record.exc_info
             message += "\n" + self._format_exc(
                 type(exc_info), exc_info, exc_info.__traceback__
             )
         return message.encode("utf-8")
@@ -580,46 +664,66 @@
 
     def __str__(self):
         return f"<{self.__class__.__name__}>"
 
 
 @dataclass
 class JSONFormatter:
+    """JSON log formatter.
+
+    To change the default `dumps` function assign it to the class attribute:
+
+    .. code-block:: python
+
+        import orjson
+
+        JSONFormatter.serializer = orjson.dumps
+
+    Formatter settings can be set directly.
+
+    .. code-block:: python
+
+        _formatter = JSONFormatter()
+        _formatter.exc_pass_locals = True
+
+    """
+
     serializer: ClassVar[Callable[[Any], bytes]] = field(
         init=False, default=_dumps_bytes
     )
     """Serializer function - a class attribute"""
 
     keys: Collection[str] = field(
         init=False,
         default=(
             "name",
-            "levelname",
+            "level",
             "asctime",
             "message",
             "exc_info",
             "extra",
             "ctx",
             "filename",
             "lineno",
             "func",
         ),
     )
-    """List of serialized log record keys"""
+    """List of serialized log record keys,
+    the available keys can be seen in :py:class:`~uvlog.LogRecord` type"""
 
     exc_pass_locals: bool = field(init=False, default=False)
-    """Pass locals in exception traceback"""
+    """Pass locals dict in exception traceback (don't use it unless you're sure your logs are secure)"""
 
     exc_pass_globals: bool = field(init=False, default=False)
-    """Pass globals in exception traceback"""
+    """Pass globals dict in exception traceback (don't use it unless you're sure your logs are secure)"""
 
     def __post_init__(self):
         self.keys = set(self.keys)
 
-    def format(self, record: LogRecord, /) -> bytes:
+    def format_record(self, record: LogRecord, /) -> bytes:
         data = {
             k: getattr(record, k) for k in self.keys if getattr(record, k) is not None
         }
         exc_info = cast(Exception, data.pop("exc_info", None))
         if exc_info and "exc_info" in self.keys:
             error_cls, exc, _ = type(exc_info), exc_info, exc_info.__traceback__
             if hasattr(exc, "serialize"):
@@ -655,79 +759,86 @@
     However, in server applications you may want to use `uvlog.QueueStreamLogger`
     to ensure your code is not blocking due to intensive logging.
     """
 
     terminator: ClassVar[bytes] = b"\n"
     """Delimiter between log records"""
 
-    _levelname: _LevelName = field(init=False, default="DEBUG")
+    _level: _LevelName = field(init=False, default="DEBUG")
     _dest: str = field(init=False, default=Stream.stderr.name)
     _formatter: Formatter = field(default_factory=TextFormatter)
     _levelno: int = field(init=False, default=0)
     _stream: Optional[BinaryIO] = field(init=False, default=None)
 
     def __post_init__(self):
-        self._levelno = _name_to_level[self._levelname]
+        self._levelno = _name_to_level[self._level]
         self._stream = None
 
     def handle(self, record: LogRecord, /) -> None:
         """Immediately write a log record to the write buffer."""
         if record.levelno < self._levelno:
             return
         if self._stream is None:
             self._stream = self._open_stream()
-        record_bytes = self._formatter.format(record)
+        record_bytes = self._formatter.format_record(record)
         try:
             self._stream.write(record_bytes + self.terminator)
         except Exception:  # noqa: acceptable
-            self._handle_error(record)
+            self._handle_error(record_bytes)
 
-    def set_level(self, levelname: _LevelName, /) -> None:
-        self._levelname = levelname
-        self._levelno = _name_to_level[levelname]
+    def set_level(self, level: _LevelName, /) -> None:
+        self._level = level
+        self._levelno = _name_to_level[level]
 
     def set_formatter(self, formatter: Formatter, /) -> None:
         self._formatter = formatter
 
     def set_destination(self, dest: str, /) -> None:
         """Set log destination (file stream).
 
-        Pre-configured destinations are present in `Stream` enum: 'stdout' and 'stderr'. Both plain and URL formats
-        for paths are acceptable:
+        Pre-configured destinations are: 'stdout' and 'stderr'.
+
+        Both plain and URL file formats are acceptable and normalized into a path string:
 
-        - 'logs.txt' - OK, relative path
-        - '/logs.txt' - OK, absolute path
-        - 'file:///logs.txt' - OK, absolute path in file URL format
+        - logs.txt - relative path
+        - /logs.txt - absolute path
+        - file:///logs.txt - absolute path in file URL format
         """
+        if dest not in (Stream.stdout.name, Stream.stderr.name):
+            _path = Path(urlparse(dest).path)
+            _path.parent.mkdir(parents=True, exist_ok=True)
+            _path.touch(exist_ok=True)
         remove_handler(dest)
         add_handler(dest, self)
         self._dest = dest
         self._stream = None
 
     def close(self) -> None:
-        """Close the opened file stream."""
+        """Close the handler including all connections to its destination.
+
+        This method is called automatically at exit for each added handler by the :py:func:`~uvlog.clear` function.
+        """
         if self._stream and not self._stream.closed:
             self._stream.flush()
             if self._stream not in (sys.stderr.buffer, sys.stdout.buffer):
                 self._stream.close()
         self._stream = None
 
     def _open_stream(self) -> BinaryIO:
         """Open a file stream."""
         if self._dest == Stream.stderr.name:
             return Stream.stderr.value
         elif self._dest == Stream.stdout.name:
             return Stream.stdout.value
         else:
-            filepath = urlparse(self._dest).path
-            return open(filepath, "ab")
+            return open(self._dest, "ab")
 
     @staticmethod
     @no_type_check
-    def _handle_error(record: LogRecord, /) -> None:
+    def _handle_error(message: bytes, /) -> None:
         """Handle an error which occurs during an emit() call.
 
         This method is a loose ripoff of the standard python logging error handling mechanism.
         """
         _, exc, tb = sys.exc_info()
         try:
             sys.stderr.write("--- Logging error ---\n")
@@ -736,22 +847,16 @@
             )
             sys.stderr.write("Call stack:\n")
             frame = exc.__traceback__.tb_frame
             while frame:
                 frame = frame.f_back
             if frame:
                 traceback.print_stack(frame, file=sys.stderr)
-            else:
-                sys.stderr.write(
-                    f"Logged from file {record.filename}, line {record.lineno}\n"
-                )
             try:
-                sys.stderr.write(
-                    f"Message: {record.message}\n Arguments: {record._asdict()}\n"
-                )
+                sys.stderr.write(f"Message: {message}\n")
             except RecursionError:
                 raise
             except Exception:  # noqa: acceptable
                 sys.stderr.write(
                     "Unable to print the message and arguments"
                     " - possible formatting error.\nUse the"
                     " traceback above to help find the error.\n"
@@ -766,151 +871,158 @@
 
 
 @dataclass
 class QueueHandler(StreamHandler):
     """Logging handler with an internal queue.
 
     This handler uses a queue and a separate thread providing at least some concurrency during intensive logging
-    workload. It has a worse overall performance than `uvlog.StreamHandler` but may be beneficial when you have
+    workload. It has a worse overall performance than :py:class:`~uvlog.StreamHandler` but may be beneficial if you have
     concurrent code such as a server application.
 
-    You may want to set `queue_size` to a reasonable value considering your application workload.
+    You may want to set :py:attr:`~uvlog.QueueHandler.queue_size`
+    to some reasonable value considering your application workload.
 
-    Note that this handler doesn't use any internal locks because it's expected by design that each handler has its own
-    destination which is unique.
+    The handler uses a separate thread to write logs to the buffer via the :py:meth:`~uvlog.QueueHandler.write_loop`
+    method. Note that this handler doesn't use any internal locks,
+    because it's expected by design that each handler has its own destination.
     """
 
     _sentinel = None
 
     queue_size: int = -1
-    """Log queue size, by default it's infinite"""
+    """Log queue size, infinite by default"""
 
     batch_size: int = 50
-    """Maximum amount of log records to write at once"""
+    """Maximum number of log records to concatenate and write at once,
+    consider setting it so an average batch would be ~ tens of KBs"""
 
     _write_queue: queue.Queue = field(default_factory=queue.Queue)
     _thread: Optional[Thread] = field(default=None)
 
     def __post_init__(self):
-        self._levelno = _name_to_level[self._levelname]
+        self._levelno = _name_to_level[self._level]
         self._write_queue.maxsize = self.queue_size
         self._stream = None
         self._thread = None
 
     def handle(self, record: LogRecord, /) -> None:
         """Put a log record to the write queue."""
         if record.levelno < self._levelno:
             return
         if self._thread is None:
             self._thread = self._open_thread()
         self._write_queue.put(record)
 
     def _open_thread(self) -> Thread:
         self._write_queue.maxsize = self.queue_size
-        thread = Thread(target=self._write, name=f"{self} _write", args=(), daemon=True)
+        thread = Thread(
+            target=self.write_loop, name=f"{self} _write", args=(), daemon=True
+        )
         thread.start()
         return thread
 
     def close(self) -> None:
+        """Close the handler including all connections to its destination.
+
+        This method is called automatically at exit for each added handler by the :py:func:`~uvlog.clear` function.
+        """
         self._write_queue.put(self._sentinel)
         if self._thread is not None:
             self._thread.join()
             self._thread = None
         # just in case the stream is not closed, however it should be closed when existing the `_write` method
         StreamHandler.close(self)
 
-    def _write(self) -> None:
-        """Write logs from the queue to the stream."""
+    def write_loop(self) -> None:
+        """Write logs from the queue to the stream.
+
+        This method is executed in a separate thread.
+        """
         _queue = self._write_queue
+        _queue.maxsize = self.queue_size
         _sentinel = self._sentinel
         _formatter = self._formatter
-        _terminator = self.terminator
         _batch_size = self.batch_size
         self._stream = _stream = self._open_stream()
-        data: List[bytes] = []
+        formatted_records: List[bytes] = []
         while 1:
             if _queue.qsize():
                 records = [_queue.get(block=True)]
             else:
                 records = [
                     _queue.get_nowait() for _ in range(min(_batch_size, _queue.qsize()))
                 ]
             for record in records:
                 if record is _sentinel:
-                    # ugly duplicate but better performance
-                    try:
-                        if data:
-                            _stream.write(_terminator.join(data) + _terminator)
-                    except Exception:  # noqa: acceptable
-                        self._handle_error(records[0])
+                    self.write(_stream, _queue, formatted_records)
                     StreamHandler.close(self)
                     return
 
-                data.append(_formatter.format(record))
-            if not data:
-                continue
-            try:
-                _stream.write(_terminator.join(data) + _terminator)
-            except Exception:  # noqa: acdceptable
-                self._handle_error(records[0])  # TODO: other records?
-            finally:
-                # if you don't finalize even failed logs then you may end up with your actual code
-                # stuck when the queue gets full
-                for _ in range(len(data)):
-                    _queue.task_done()
-                data.clear()
+                formatted_records.append(_formatter.format_record(record))
+
+            self.write(_stream, _queue, formatted_records)
+            formatted_records.clear()
+
+    def write(
+        self, _stream: BinaryIO, _queue: queue.Queue, formatted_records: List[bytes], /
+    ) -> None:
+        if not formatted_records:
+            return
+        try:
+            formatted_records.append(b"")
+            _stream.write(self.terminator.join(formatted_records))
+        except Exception:  # noqa: acdceptable
+            self._handle_error(formatted_records[0])
+        finally:
+            for _ in range(len(formatted_records) - 1):
+                _queue.task_done()
+
+
+def _merge_dicts(from_dict: dict, to_dict: dict) -> dict:
+    _new_dict = {**from_dict}
+    for key, value in to_dict.items():
+        if key in _new_dict and type(value) is dict:
+            _new_dict[key] = _merge_dicts(_new_dict[key], value)
+        else:
+            _new_dict[key] = value
+    return _new_dict
 
 
 def _configure_formatter(name: str, params: dict, /) -> None:
-    if name in _formatters:
-        _formatter = _formatters[name]
-    else:
-        cls = _formatter_types[params.pop("class", TextFormatter.__name__)]
-        _formatter = cls()
+    cls = _formatter_types[params.pop("class", TextFormatter.__name__)]
+    _formatter = cls()
     for key, value in params.items():
         if not key.startswith("_"):
             setattr(_formatter, key, value)
-    add_formatter(name, _formatter)
+    _formatters[name] = _formatter
 
 
 def _configure_handler(dest: str, params: dict, /) -> None:
-    if dest in _handlers:
-        _handler = _handlers[dest]
-    else:
-        cls_name = params.pop("class", StreamHandler.__name__)
-        _handler = _handler_types[cls_name]()
-        _handler.set_destination(dest)
-        for key, value in params.items():
-            setattr(_handler, key, value)
-    formatter_name: Optional[str] = params.pop("formatter", None)
-    if formatter_name:
-        _handler.set_formatter(_formatters[formatter_name])
-    levelname: Optional[_LevelName] = params.pop("levelname", None)
-    if levelname:
-        _handler.set_level(levelname)
+    cls_name = params.pop("class", StreamHandler.__name__)
+    _handler = _handler_types[cls_name]()
+    _handler.set_destination(dest)
+    formatter_name = params.pop("formatter", "text")
+    _handler.set_formatter(_formatters[formatter_name])
+    level: _LevelName = cast(_LevelName, params.pop("level", "DEBUG"))
+    _handler.set_level(level)
     for key, value in params.items():
         if not key.startswith("_"):
             setattr(_handler, key, value)
 
 
 def _configure_logger(name: str, params: dict, context_var: ContextVar, /) -> None:
-    if name in _loggers:
-        _logger = _loggers[name]
-    else:
-        _logger = get_logger(name, persistent=True)
+    _logger = get_logger(name, persistent=True)
     handler_names = params.pop("handlers", [Stream.stderr.name])
-    if handler_names:
-        _logger.handlers = [_handlers[handler_name] for handler_name in handler_names]
-    levelname: Optional[_LevelName] = params.pop("levelname", None)
-    if levelname:
-        _logger.set_level(levelname)
+    _logger.handlers = [_handlers[handler_name] for handler_name in handler_names]
+    level: _LevelName = cast(_LevelName, params.pop("level", "INFO"))
+    _logger.set_level(level)
+    _logger.context = context_var
     for key, value in params.items():
         if not key.startswith("_"):
             setattr(_logger, key, value)
-    _logger.context = context_var
 
 
 def configure(
     config_dict: _DictConfig, /, context_var: ContextVar = LOG_CONTEXT
 ) -> Logger:
     """Configure loggers for a configuration dict.
 
@@ -922,67 +1034,63 @@
     different.
 
     .. code-block:: python
 
         {
             "loggers": {
                 "app": {
-                    "levelname": "ERROR",
+                    "level": "ERROR",
                     "handlers": ["my_file.txt"],
                     "capture_trace": True
                 }
             },
             "handlers": {
                 "my_file.txt": {
                     "class": "StreamHandler",
-                    "levelname": "DEBUG",
+                    "level": "DEBUG",
                     "formatter": "my_format"
                 }
             },
             "formatters": {
                 "my_format": {
                     "class": "TextFormatter",
-                    "format_string": "{name}: {message}"
+                    "format": "{name}: {message}"
                 }
             }
         }
 
     The main differences are:
 
     - 'class' names for handlers and formatters must be registered beforehand using 'add_formatter_type()' and
         'add_handler_type()' respectively to allow classes not inherited from `Handler` / 'Formatter`
-    - 'level' changed to 'levelname' to emphasize that you need to pass a string there
     - handler names are their destinations, since by design you're not allowed to bind multiple handlers to a single
         destination
-    - 'format_string' for the text formatter should be in Python f-string format
+    - 'format' for the text formatter should be in Python f-string format
 
     .. attention::
 
         The function is designed in such way you can extend or modify existing loggers, handlers or formatters
         by passing a config. If you want to configure logging from zero you should call `clear()` method beforehand.
         Please note that you need to provide all the handlers, formatters, loggers in the config after doing that,
         including the root logger (empty string).
 
     """
-    config_dict = deepcopy(config_dict)
-    for name, params in config_dict.get("formatters", {}).items():
+    clear()
+    config_dict = cast(
+        _DictConfig, _merge_dicts(cast(dict, BASIC_CONFIG), cast(dict, config_dict))
+    )
+    for name, params in config_dict["formatters"].items():
         _configure_formatter(name, params)
-    for dest, params in config_dict.get("handlers", {}).items():
+    for dest, params in config_dict["handlers"].items():
         _configure_handler(dest, params)
     # sorting loggers to init parents before children
-    loggers_params = list(config_dict.get("loggers", {}).items())
+    loggers_params = list(config_dict["loggers"].items())
     loggers_params.sort(key=lambda x: x[0])
     for name, params in loggers_params:
         _configure_logger(name, params, context_var)
-    if _root_logger_name not in _loggers:
-        raise ValueError(
-            "root logger is not configured\n\n"
-            f'Fix: ensure that you did not delete the root logger "{_root_logger_name}", '
-            f"if you used `uvlog.clear()` method you must provide a root logger configuration yourself"
-        )
     return _loggers[_root_logger_name]
 
 
 def clear() -> None:
     """Clear all existing loggers, handlers and formatters.
 
     This function also closes all existing handlers.
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `uvlog-0.1.0.dist-info/LICENSE` & `uvlog-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `uvlog-0.1.0.dist-info/METADATA` & `uvlog-0.1.1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: uvlog
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pythonic logger with better performance and contextvars + JSON support out of the box
 Home-page: 
-Author: attr: uvlog.__author__
-License: attr: __license__
+Author: violetblackdev@gmail.com
+License: MIT
 Keywords: logging,logs
 Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -31,25 +35,24 @@
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: python-docs-theme ; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest ==8.1.1 ; extra == 'test'
 Requires-Dist: orjson ==3.9.15 ; extra == 'test'
 
-
 [![PyPi Version](https://img.shields.io/pypi/v/uvlog.svg)](https://pypi.python.org/pypi/uvlog/)
 [![Docs](https://readthedocs.org/projects/uvlog/badge/?version=latest&style=flat)](https://uvlog.readthedocs.io)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-[![3.8](https://github.com/violet-black/uvlog/actions/workflows/py38.yaml/badge.svg)
-[![3.9](https://github.com/violet-black/uvlog/actions/workflows/py39.yaml/badge.svg)
-[![3.10](https://github.com/violet-black/uvlog/actions/workflows/py310.yaml/badge.svg)
-[![3.11](https://github.com/violet-black/uvlog/actions/workflows/py311.yaml/badge.svg)
-[![3.12](https://github.com/violet-black/uvlog/actions/workflows/py312.yaml/badge.svg)
+[![3.8](https://github.com/violet-black/uvlog/actions/workflows/py38.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/py38.yaml)
+[![3.9](https://github.com/violet-black/uvlog/actions/workflows/py39.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/py39.yaml)
+[![3.10](https://github.com/violet-black/uvlog/actions/workflows/py310.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/py310.yaml)
+[![3.11](https://github.com/violet-black/uvlog/actions/workflows/py311.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/py311.yaml)
+[![3.12](https://github.com/violet-black/uvlog/actions/workflows/py312.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/py312.yaml)
 
 **uvlog** is yet another logging library built with an idea of a simple logger what 'just works' without
 need for extension and customization. 
 
 - Single file, no external dependencies
 - JSON and [contextvars](https://docs.python.org/3/library/contextvars.html) out of the box
 - Less abstraction, better [performance](#Performance)
@@ -90,15 +93,15 @@
 
 ```python
 from uvlog import configure
 
 logger = configure({
     'loggers': {
         '': {
-            'levelname': 'DEBUG',
+            'level': 'DEBUG',
             'handlers': ['stderr', '/etc/log.txt']
         }
     },
     'handlers': {
         'stderr': {
             'class': 'StreamHandler',
             'formatter': 'json'
@@ -107,15 +110,15 @@
             'class': 'QueueHandler',
             'formatter': 'text'
         }
     },
     'formatters': {
         'text': {
             'class': 'TextFormatter',
-            'format_string': '{asctime} : {name} : {message}',
+            'format': '{asctime} : {name} : {message}',
             'timestamp_separator': ' '
         },
         'json': {
             'class': 'JSONFormatter',
             'keys': ['asctime', 'name', 'message']
         }
     }
@@ -196,18 +199,18 @@
 Benchmark results are provided for the M1 Pro Mac (16GB). The results are for the `StreamHandler`
 writing same log records into a file. The `QueueHandler` provides similar performance, but has been excluded
 from the test since Python threading model prevents results from being consistent between runs. However,
 I'd still recommend using the `QueueHandler` for server applications.
 
 | name          | total (s) | logs/s | %   |
 |---------------|-----------|--------|-----|
-| python logger | 0.11      | 92568  | 100 |
-| uvlog text    | 0.031     | 325034 | 351 |
-| uvlog json    | 0.02      | 500878 | 541 |
+| python logger | 0.085     | 117357 | 100 |
+| uvlog text    | 0.022     | 455333 | 388 |
+| uvlog json    | 0.015     | 665942 | 567 |
 
 # Ideas / goals
 
 - Rotating file handlers
 - Asynchronous queue logging to HTTP / TCP / UDP
-- Referencing `extra` and `ctx` keys in log message format strings
 - Better customization for `Logger` / `LogRecord` objects
+- Better coverage
 - Cython?
```


# Comparing `tmp/python_injection-0.8.0.tar.gz` & `tmp/python_injection-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_injection-0.8.0.tar", max compression
+gzip compressed data, was "python_injection-0.8.1.tar", max compression
```

## Comparing `python_injection-0.8.0.tar` & `python_injection-0.8.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     2809 2024-03-30 11:28:14.624004 python_injection-0.8.0/documentation/basic-usage.md
--rw-r--r--   0        0        0       20 2024-03-30 11:28:14.624004 python_injection-0.8.0/injection/__init__.py
--rw-r--r--   0        0        0      647 2024-03-30 11:28:14.624004 python_injection-0.8.0/injection/_pkg.py
--rw-r--r--   0        0        0     5171 2024-03-30 11:28:14.624004 python_injection-0.8.0/injection/_pkg.pyi
--rw-r--r--   0        0        0        0 2024-03-30 11:28:14.624004 python_injection-0.8.0/injection/common/__init__.py
--rw-r--r--   0        0        0     1392 2024-03-30 11:28:14.624004 python_injection-0.8.0/injection/common/event.py
--rw-r--r--   0        0        0     1436 2024-03-30 11:28:14.624004 python_injection-0.8.0/injection/common/lazy.py
--rw-r--r--   0        0        0     1566 2024-03-30 11:28:14.624004 python_injection-0.8.0/injection/common/queue.py
--rw-r--r--   0        0        0        0 2024-03-30 11:28:14.624004 python_injection-0.8.0/injection/common/tools/__init__.py
--rw-r--r--   0        0        0      688 2024-03-30 11:28:14.624004 python_injection-0.8.0/injection/common/tools/threading.py
--rw-r--r--   0        0        0     1276 2024-03-30 11:28:14.624004 python_injection-0.8.0/injection/common/tools/type.py
--rw-r--r--   0        0        0       22 2024-03-30 11:28:14.624004 python_injection-0.8.0/injection/core/__init__.py
--rw-r--r--   0        0        0    18989 2024-03-30 11:28:14.624004 python_injection-0.8.0/injection/core/module.py
--rw-r--r--   0        0        0      653 2024-03-30 11:28:14.628003 python_injection-0.8.0/injection/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-30 11:28:14.628003 python_injection-0.8.0/injection/integrations/__init__.py
--rw-r--r--   0        0        0      723 2024-03-30 11:28:14.628003 python_injection-0.8.0/injection/integrations/blacksheep.py
--rw-r--r--   0        0        0      676 2024-03-30 11:28:14.628003 python_injection-0.8.0/injection/utils.py
--rw-r--r--   0        0        0     1173 2024-03-30 11:28:29.420059 python_injection-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 python_injection-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2809 2024-04-01 11:37:27.304823 python_injection-0.8.1/documentation/basic-usage.md
+-rw-r--r--   0        0        0       20 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/__init__.py
+-rw-r--r--   0        0        0      647 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/_pkg.py
+-rw-r--r--   0        0        0     5327 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/_pkg.pyi
+-rw-r--r--   0        0        0        0 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/common/__init__.py
+-rw-r--r--   0        0        0     1316 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/common/event.py
+-rw-r--r--   0        0        0      558 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/common/invertible.py
+-rw-r--r--   0        0        0     1401 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/common/lazy.py
+-rw-r--r--   0        0        0     1443 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/common/queue.py
+-rw-r--r--   0        0        0        0 2024-04-01 11:37:27.304823 python_injection-0.8.1/injection/common/tools/__init__.py
+-rw-r--r--   0        0        0      271 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/common/tools/threading.py
+-rw-r--r--   0        0        0     1276 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/common/tools/type.py
+-rw-r--r--   0        0        0       22 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/core/__init__.py
+-rw-r--r--   0        0        0    19284 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/core/module.py
+-rw-r--r--   0        0        0      653 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/integrations/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/integrations/blacksheep.py
+-rw-r--r--   0        0        0      676 2024-04-01 11:37:27.308823 python_injection-0.8.1/injection/utils.py
+-rw-r--r--   0        0        0     1173 2024-04-01 11:37:42.176814 python_injection-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 python_injection-0.8.1/PKG-INFO
```

### Comparing `python_injection-0.8.0/documentation/basic-usage.md` & `python_injection-0.8.1/documentation/basic-usage.md`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.0/injection/_pkg.py` & `python_injection-0.8.1/injection/_pkg.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.0/injection/_pkg.pyi` & `python_injection-0.8.1/injection/_pkg.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Final,
     Protocol,
     TypeVar,
     final,
     runtime_checkable,
 )
 
-from injection.common.lazy import Lazy
+from injection.common.invertible import Invertible
 
 _T = TypeVar("_T")
 
 default_module: Final[Module] = ...
 
 get_instance = default_module.get_instance
 get_lazy_instance = default_module.get_lazy_instance
@@ -100,19 +100,24 @@
     def get_instance(self, cls: type[_T], none: bool = ...) -> _T | None:
         """
         Function used to retrieve an instance associated with the type passed in
         parameter or return `None` but if `none` parameter is `False` an exception
         will be raised.
         """
 
-    def get_lazy_instance(self, cls: type[_T]) -> Lazy[_T | None]:
+    def get_lazy_instance(
+        self,
+        cls: type[_T],
+        cache: bool = ...,
+    ) -> Invertible[_T | None]:
         """
         Function used to retrieve an instance associated with the type passed in
-        parameter or `None`. Return a `Lazy` object. To access the instance contained
-        in a lazy object, simply use a wavy line (~).
+        parameter or `None`. Return a `Invertible` object. To access the instance
+        contained in an invertible object, simply use a wavy line (~).
+        With `cache=True`, the instance retrieved will always be the same.
 
         Example: instance = ~lazy_instance
         """
 
     def use(self, module: Module, priority: ModulePriority = ...):
         """
         Function for using another module. Using another module replaces the module's
```

### Comparing `python_injection-0.8.0/injection/common/event.py` & `python_injection-0.8.1/injection/common/event.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from abc import ABC, abstractmethod
 from contextlib import ContextDecorator, ExitStack, contextmanager, suppress
 from dataclasses import dataclass, field
 from typing import ContextManager
 from weakref import WeakSet
 
-from injection.common.tools.threading import frozen_collection
-
 __all__ = ("Event", "EventChannel", "EventListener")
 
 
 class Event(ABC):
     __slots__ = ()
 
 
@@ -24,15 +22,15 @@
 @dataclass(repr=False, eq=False, frozen=True, slots=True)
 class EventChannel:
     __listeners: WeakSet[EventListener] = field(default_factory=WeakSet, init=False)
 
     @contextmanager
     def dispatch(self, event: Event) -> ContextManager | ContextDecorator:
         with ExitStack() as stack:
-            for listener in frozen_collection(self.__listeners):
+            for listener in tuple(self.__listeners):
                 context_manager = listener.on_event(event)
 
                 if context_manager is None:
                     continue
 
                 stack.enter_context(context_manager)
```

### Comparing `python_injection-0.8.0/injection/common/lazy.py` & `python_injection-0.8.1/injection/common/lazy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 from collections.abc import Callable, Iterator, Mapping
 from types import MappingProxyType
-from typing import Generic, TypeVar
+from typing import TypeVar
 
-from injection.common.tools.threading import thread_lock
+from injection.common.invertible import Invertible
 
 __all__ = ("Lazy", "LazyMapping")
 
 _T = TypeVar("_T")
 _K = TypeVar("_K")
 _V = TypeVar("_V")
 
 
-class Lazy(Generic[_T]):
+class Lazy(Invertible[_T]):
     __slots__ = ("__cache", "__is_set")
 
     def __init__(self, factory: Callable[[], _T]):
         self.__setup_cache(factory)
 
     def __invert__(self) -> _T:
         return next(self.__cache)
 
     @property
     def is_set(self) -> bool:
         return self.__is_set
 
     def __setup_cache(self, factory: Callable[[], _T]):
-        def new_cache() -> Iterator[_T]:
-            with thread_lock:
-                self.__is_set = True
-
+        def cache_generator() -> Iterator[_T]:
             nonlocal factory
             cached = factory()
+            self.__is_set = True
             del factory
 
             while True:
                 yield cached
 
-        self.__cache = new_cache()
+        self.__cache = cache_generator()
         self.__is_set = False
 
 
 class LazyMapping(Mapping[_K, _V]):
     __slots__ = ("__lazy",)
 
     def __init__(self, iterator: Iterator[tuple[_K, _V]]):
```

### Comparing `python_injection-0.8.0/injection/common/queue.py` & `python_injection-0.8.1/injection/common/queue.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from abc import abstractmethod
 from collections import deque
 from collections.abc import Iterator
 from dataclasses import dataclass, field
 from typing import NoReturn, Protocol, TypeVar
 
-from injection.common.tools.threading import thread_lock
-
 __all__ = ("LimitedQueue",)
 
 _T = TypeVar("_T")
 
 
 class Queue(Iterator[_T], Protocol):
     __slots__ = ()
@@ -30,39 +28,36 @@
             raise StopIteration from exc
 
     def add(self, item: _T):
         self.__items.append(item)
         return self
 
 
-class NoQueue(Queue[_T]):
+class DeadQueue(Queue[_T]):
     __slots__ = ()
 
     def __bool__(self) -> bool:
         return False
 
     def __next__(self) -> NoReturn:
         raise StopIteration
 
     def add(self, item: _T) -> NoReturn:
-        raise TypeError("Queue doesn't exist.")
+        raise TypeError("Queue is dead.")
 
 
 @dataclass(repr=False, slots=True)
 class LimitedQueue(Queue[_T]):
-    __queue: Queue[_T] = field(default_factory=SimpleQueue)
+    __state: Queue[_T] = field(default_factory=SimpleQueue)
 
     def __next__(self) -> _T:
-        if not self.__queue:
-            raise StopIteration
-
         try:
-            return next(self.__queue)
+            return next(self.__state)
         except StopIteration as exc:
-            with thread_lock:
-                self.__queue = NoQueue()
+            if self.__state:
+                self.__state = DeadQueue()
 
             raise exc
 
     def add(self, item: _T):
-        self.__queue.add(item)
+        self.__state.add(item)
         return self
```

### Comparing `python_injection-0.8.0/injection/common/tools/type.py` & `python_injection-0.8.1/injection/common/tools/type.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.0/injection/core/module.py` & `python_injection-0.8.1/injection/core/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,21 +33,18 @@
     Protocol,
     TypeVar,
     cast,
     runtime_checkable,
 )
 
 from injection.common.event import Event, EventChannel, EventListener
+from injection.common.invertible import Invertible, SimpleInvertible
 from injection.common.lazy import Lazy, LazyMapping
 from injection.common.queue import LimitedQueue
-from injection.common.tools.threading import (
-    frozen_collection,
-    synchronized,
-    thread_lock,
-)
+from injection.common.tools.threading import synchronized
 from injection.common.tools.type import find_types, format_type, get_origins
 from injection.exceptions import (
     InjectionError,
     ModuleError,
     ModuleLockError,
     ModuleNotUsedError,
     NoInjectable,
@@ -157,14 +154,21 @@
         pass
 
     @abstractmethod
     def get_instance(self) -> _T:
         raise NotImplementedError
 
 
+class FallbackInjectable(Injectable[_T], ABC):
+    __slots__ = ()
+
+    def __bool__(self) -> bool:
+        return False
+
+
 @dataclass(repr=False, frozen=True, slots=True)
 class BaseInjectable(Injectable[_T], ABC):
     factory: Callable[[], _T]
 
 
 class NewInjectable(BaseInjectable[_T]):
     __slots__ = ()
@@ -189,28 +193,25 @@
     def unlock(self):
         self.cache.clear()
 
     def get_instance(self) -> _T:
         with suppress(KeyError):
             return self.cache[self.__INSTANCE_KEY]
 
-        with thread_lock:
+        with synchronized():
             instance = self.factory()
             self.cache[self.__INSTANCE_KEY] = instance
 
         return instance
 
 
 @dataclass(repr=False, frozen=True, slots=True)
-class ShouldBeInjectable(Injectable[_T]):
+class ShouldBeInjectable(FallbackInjectable[_T]):
     cls: type[_T]
 
-    def __bool__(self) -> bool:
-        return False
-
     def get_instance(self) -> NoReturn:
         raise InjectionError(f"`{format_type(self.cls)}` should be an injectable.")
 
 
 """
 Broker
 """
@@ -260,44 +261,46 @@
 
     @property
     def is_locked(self) -> bool:
         return any(injectable.is_locked for injectable in self.__injectables)
 
     @property
     def __classes(self) -> frozenset[type]:
-        return frozenset(self.__data.keys())
+        return frozenset(self.__data)
 
     @property
     def __injectables(self) -> frozenset[Injectable]:
         return frozenset(self.__data.values())
 
+    @synchronized()
     def update(self, classes: Iterable[type], injectable: Injectable, override: bool):
         classes = frozenset(get_origins(*classes))
 
-        with thread_lock:
-            if not injectable:
-                classes -= self.__classes
-                override = True
+        if not injectable:
+            classes -= self.__classes
+            override = True
 
-            if classes:
-                event = ContainerDependenciesUpdated(self, classes, override)
+        if classes:
+            event = ContainerDependenciesUpdated(self, classes, override)
 
-                with self.notify(event):
-                    if not override:
-                        self.__check_if_exists(classes)
+            with self.notify(event):
+                if not override:
+                    self.__check_if_exists(classes)
 
-                    self.__data.update((cls, injectable) for cls in classes)
+                self.__data.update((cls, injectable) for cls in classes)
 
         return self
 
-    @synchronized
+    @synchronized()
     def unlock(self):
         for injectable in self.__injectables:
             injectable.unlock()
 
+        return self
+
     def add_listener(self, listener: EventListener):
         self.__channel.add_listener(listener)
         return self
 
     def notify(self, event: Event) -> ContextManager | ContextDecorator:
         return self.__channel.dispatch(event)
 
@@ -356,15 +359,15 @@
 
     @property
     def is_locked(self) -> bool:
         return any(broker.is_locked for broker in self.__brokers)
 
     @property
     def __brokers(self) -> Iterator[Broker]:
-        yield from frozen_collection(self.__modules)
+        yield from tuple(self.__modules)
         yield self.__container
 
     def injectable(
         self,
         wrapped: Callable[..., Any] = None,
         /,
         *,
@@ -417,15 +420,15 @@
         def decorator(wp):
             if not return_factory and isclass(wp):
                 wp.__init__ = self.inject(wp.__init__)
                 return wp
 
             function = InjectedFunction(wp)
 
-            @function.setup
+            @function.on_setup
             def listen():
                 function.update(self)
                 self.add_listener(function)
 
             return function
 
         return decorator(wrapped) if wrapped else decorator
@@ -438,16 +441,25 @@
                 return None
 
             raise exc
 
         instance = injectable.get_instance()
         return cast(cls, instance)
 
-    def get_lazy_instance(self, cls: type[_T]) -> Lazy[_T | None]:
-        return Lazy(lambda: self.get_instance(cls))
+    def get_lazy_instance(
+        self,
+        cls: type[_T],
+        cache: bool = False,
+    ) -> Invertible[_T | None]:
+        if cache:
+            return Lazy(lambda: self.get_instance(cls))
+
+        function = self.inject(lambda instance=None: instance)
+        function.set_owner(cls)
+        return SimpleInvertible(function)
 
     def update(
         self,
         classes: Iterable[type],
         injectable: Injectable,
         override: bool = False,
     ):
@@ -498,19 +510,21 @@
         event = ModulePriorityUpdated(self, module, priority)
 
         with self.notify(event):
             self.__move_module(module, priority)
 
         return self
 
-    @synchronized
+    @synchronized()
     def unlock(self):
         for broker in self.__brokers:
             broker.unlock()
 
+        return self
+
     def add_listener(self, listener: EventListener):
         self.__channel.add_listener(listener)
         return self
 
     def remove_listener(self, listener: EventListener):
         self.__channel.remove_listener(listener)
         return self
@@ -636,15 +650,15 @@
             args, kwargs = self.bind(args, kwargs)
             return wrapped(*args, **kwargs)
 
         self.__wrapper = wrapper
         self.__dependencies = Dependencies.empty()
         self.__owner = None
         self.__setup_queue = LimitedQueue[Callable[[], Any]]()
-        self.setup(
+        self.on_setup(
             lambda: self.__set_signature(
                 inspect.signature(
                     wrapped,
                     eval_str=True,
                 )
             )
         )
@@ -661,23 +675,15 @@
     def __get__(self, instance: object = None, owner: type = None):
         if instance is None:
             return self
 
         return self.__wrapper.__get__(instance, owner)
 
     def __set_name__(self, owner: type, name: str):
-        if self.__dependencies.are_resolved:
-            raise TypeError(
-                "Function owner must be assigned before dependencies are resolved."
-            )
-
-        if self.__owner:
-            raise TypeError("Function owner is already defined.")
-
-        self.__owner = owner
+        self.set_owner(owner)
 
     @property
     def signature(self) -> Signature:
         return self.__signature__
 
     def bind(
         self,
@@ -692,25 +698,32 @@
 
         bound = self.signature.bind_partial(*args, **kwargs)
         bound.arguments = (
             bound.arguments | self.__dependencies.arguments | bound.arguments
         )
         return Arguments(bound.args, bound.kwargs)
 
-    def update(self, module: Module):
-        with thread_lock:
-            self.__dependencies = Dependencies.resolve(
-                self.signature,
-                module,
-                self.__owner,
+    def set_owner(self, owner: type):
+        if self.__dependencies.are_resolved:
+            raise TypeError(
+                "Function owner must be assigned before dependencies are resolved."
             )
 
+        if self.__owner:
+            raise TypeError("Function owner is already defined.")
+
+        self.__owner = owner
         return self
 
-    def setup(self, wrapped: Callable[[], Any] = None, /):
+    @synchronized()
+    def update(self, module: Module):
+        self.__dependencies = Dependencies.resolve(self.signature, module, self.__owner)
+        return self
+
+    def on_setup(self, wrapped: Callable[[], Any] = None, /):
         def decorator(wp):
             self.__setup_queue.add(wp)
             return wp
 
         return decorator(wrapped) if wrapped else decorator
 
     @singledispatchmethod
@@ -726,11 +739,9 @@
     def __consume_setup_queue(self):
         for function in self.__setup_queue:
             function()
 
         return self
 
     def __set_signature(self, signature: Signature):
-        with thread_lock:
-            self.__signature__ = signature
-
+        self.__signature__ = signature
         return self
```

### Comparing `python_injection-0.8.0/injection/exceptions.py` & `python_injection-0.8.1/injection/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.0/injection/integrations/blacksheep.py` & `python_injection-0.8.1/injection/integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.0/injection/utils.py` & `python_injection-0.8.1/injection/utils.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.0/pyproject.toml` & `python_injection-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-injection"
-version = "0.8.0"
+version = "0.8.1"
 description = "Fast and easy dependency injection framework."
 authors = ["remimd"]
 keywords = ["dependencies", "inject", "injection"]
 license = "MIT"
 packages = [{ include = "injection" }]
 readme = "documentation/basic-usage.md"
 repository = "https://github.com/100nm/python-injection"
```

### Comparing `python_injection-0.8.0/PKG-INFO` & `python_injection-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-injection
-Version: 0.8.0
+Version: 0.8.1
 Summary: Fast and easy dependency injection framework.
 Home-page: https://github.com/100nm/python-injection
 License: MIT
 Keywords: dependencies,inject,injection
 Author: remimd
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: MIT License
```


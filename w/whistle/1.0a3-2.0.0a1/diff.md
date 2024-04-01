# Comparing `tmp/whistle-1.0a3.tar.gz` & `tmp/whistle-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/whistle-1.0a3.tar", last modified: Tue Oct 17 10:45:45 2017, max compression
+gzip compressed data, was "whistle-2.0.0a1.tar", max compression
```

## Comparing `whistle-1.0a3.tar` & `whistle-2.0.0a1.tar`

### file list

```diff
@@ -1,21 +1,16 @@
-drwxr-xr-x   0 rd         (502) staff       (20)        0 2017-10-17 10:45:45.000000 whistle-1.0a3/
--rw-r--r--   0 rd         (502) staff       (20)        0 2017-10-17 10:45:31.000000 whistle-1.0a3/classifiers.txt
--rw-r--r--   0 rd         (502) staff       (20)       14 2017-10-17 10:45:31.000000 whistle-1.0a3/MANIFEST.in
--rw-r--r--   0 rd         (502) staff       (20)     1319 2017-10-17 10:45:45.000000 whistle-1.0a3/PKG-INFO
--rw-r--r--   0 rd         (502) staff       (20)      742 2017-10-17 10:45:31.000000 whistle-1.0a3/README.rst
--rw-r--r--   0 rd         (502) staff       (20)      349 2017-10-17 10:45:31.000000 whistle-1.0a3/requirements-dev.txt
--rw-r--r--   0 rd         (502) staff       (20)        5 2017-10-17 10:45:31.000000 whistle-1.0a3/requirements.txt
--rw-r--r--   0 rd         (502) staff       (20)       80 2017-10-17 10:45:45.000000 whistle-1.0a3/setup.cfg
--rw-r--r--   0 rd         (502) staff       (20)     1818 2017-10-17 10:45:31.000000 whistle-1.0a3/setup.py
--rw-r--r--   0 rd         (502) staff       (20)        6 2017-10-17 10:45:31.000000 whistle-1.0a3/version.txt
-drwxr-xr-x   0 rd         (502) staff       (20)        0 2017-10-17 10:45:45.000000 whistle-1.0a3/whistle/
--rw-r--r--   0 rd         (502) staff       (20)      190 2017-10-17 10:45:31.000000 whistle-1.0a3/whistle/__init__.py
--rw-r--r--   0 rd         (502) staff       (20)       22 2017-10-17 10:45:31.000000 whistle-1.0a3/whistle/_version.py
--rw-r--r--   0 rd         (502) staff       (20)     3447 2017-10-17 10:45:31.000000 whistle-1.0a3/whistle/dispatcher.py
--rw-r--r--   0 rd         (502) staff       (20)      627 2017-10-17 10:45:31.000000 whistle-1.0a3/whistle/event.py
-drwxr-xr-x   0 rd         (502) staff       (20)        0 2017-10-17 10:45:45.000000 whistle-1.0a3/whistle.egg-info/
--rw-r--r--   0 rd         (502) staff       (20)        1 2017-10-17 10:45:45.000000 whistle-1.0a3/whistle.egg-info/dependency_links.txt
--rw-r--r--   0 rd         (502) staff       (20)     1319 2017-10-17 10:45:45.000000 whistle-1.0a3/whistle.egg-info/PKG-INFO
--rw-r--r--   0 rd         (502) staff       (20)       81 2017-10-17 10:45:45.000000 whistle-1.0a3/whistle.egg-info/requires.txt
--rw-r--r--   0 rd         (502) staff       (20)      340 2017-10-17 10:45:45.000000 whistle-1.0a3/whistle.egg-info/SOURCES.txt
--rw-r--r--   0 rd         (502) staff       (20)        8 2017-10-17 10:45:45.000000 whistle-1.0a3/whistle.egg-info/top_level.txt
+-rw-r--r--   0        0        0     2262 2023-12-09 10:09:36.861775 whistle-2.0.0a1/README.rst
+-rw-r--r--   0        0        0      698 2024-04-01 14:22:31.087050 whistle-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0      338 2024-01-21 17:15:21.015994 whistle-2.0.0a1/whistle/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-01 14:14:31.499606 whistle-2.0.0a1/whistle/_version.py
+-rw-r--r--   0        0        0      154 2024-01-21 17:15:21.016240 whistle-2.0.0a1/whistle/dispatchers/__init__.py
+-rw-r--r--   0        0        0     1459 2024-01-21 17:15:21.016618 whistle-2.0.0a1/whistle/dispatchers/asynchronous.py
+-rw-r--r--   0        0        0     1840 2024-01-21 17:15:21.016842 whistle-2.0.0a1/whistle/dispatchers/base.py
+-rw-r--r--   0        0        0     2359 2024-01-21 17:15:21.017068 whistle-2.0.0a1/whistle/dispatchers/synchronous.py
+-rw-r--r--   0        0        0       50 2024-01-21 17:15:21.017271 whistle-2.0.0a1/whistle/errors.py
+-rw-r--r--   0        0        0      728 2024-01-21 17:15:21.017624 whistle-2.0.0a1/whistle/event.py
+-rw-r--r--   0        0        0     3309 2024-01-21 17:15:21.017932 whistle-2.0.0a1/whistle/listeners.py
+-rw-r--r--   0        0        0      263 2024-01-21 17:15:21.018178 whistle-2.0.0a1/whistle/typing/__init__.py
+-rw-r--r--   0        0        0      939 2024-01-21 17:15:21.018543 whistle-2.0.0a1/whistle/typing/dispatcher.py
+-rw-r--r--   0        0        0      143 2024-01-21 17:15:21.018808 whistle-2.0.0a1/whistle/typing/event.py
+-rw-r--r--   0        0        0      172 2024-01-21 17:15:21.019116 whistle-2.0.0a1/whistle/typing/listener.py
+-rw-r--r--   0        0        0     2750 1970-01-01 00:00:00.000000 whistle-2.0.0a1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `whistle-1.0a3/whistle/dispatcher.py` & `whistle-2.0.0a1/whistle/dispatchers/synchronous.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,56 @@
-import operator
+import inspect
+from typing import Optional, cast
 
+from whistle.dispatchers.base import AbstractEventDispatcher
 from whistle.event import Event
+from whistle.typing import IDispatchedEvent, IEvent, IListener
 
 
-class EventDispatcher(object):
+class EventDispatcher(AbstractEventDispatcher):
     """
-    A logical event dispatcher. All events can only be dispatched in the context of an :class:`EventDispatcher`, and
-    event dispatchers are fully independant and isolated.
+    Main class of the library, it is responsible for keeping track of registered listeners, and dispatching events to
+    them. All listeners are scoped to the event dispatcher instance, so you can have multiple event dispatchers with
+    different sets of listeners.
 
     """
 
-    def __init__(self):
-        self._listeners = {}
-        self._sorted = {}
+    def add_listener(self, event_id: str, listener: IListener, /, *, priority: int = 0):
+        if inspect.iscoroutinefunction(listener):
+            raise TypeError(f"Listener should not be a coroutine function, {type(listener)} given")
+        return super().add_listener(event_id, listener, priority=priority)
 
-    def dispatch(self, event_id, event=None):
-        if event is None:
-            event = Event()
-
-        event.dispatcher = self
-        event.name = event_id
-
-        if not event_id in self._listeners:
-            return event
-
-        self.do_dispatch(self.get_listeners(event_id), event)
-
-        return event
-
-    def get_listeners(self, event_id=None):
-        if event_id is not None:
-            if not event_id in self._sorted:
-                self.sort_listeners(event_id)
-
-            return self._sorted[event_id]
-
-        for event_id in self._listeners:
-            if not event_id in self._sorted:
-                self.sort_listeners(event_id)
-
-        return self._sorted
-
-    def has_listeners(self, event_id=None):
-        return bool(len(self.get_listeners(event_id)))
-
-    def add_listener(self, event_id, listener, priority=0):
-        if not event_id in self._listeners:
-            self._listeners[event_id] = {}
-        if not priority in self._listeners[event_id]:
-            self._listeners[event_id][priority] = []
-        self._listeners[event_id][priority].append(listener)
+    def dispatch(self, event_id: str, event: Optional[IEvent] = None, /) -> IDispatchedEvent:
+        """
+        Dispatch the given event, with the given event id.
 
-        if event_id in self._sorted:
-            del self._sorted[event_id]
+        An optional event can be given, and should respect the :class:`whistle.protocols.IEvent` protocol.
+        If no event is given, a new :class:`whistle.event.Event` instance is created and used.
 
-    def listen(self, event_id, priority=0):
-        """
-        Decorator that add the decorated functions as one of this instance listeners, for the given event name.
+        Returns the event instance after it has been dispatched, whether it has been created or provided by the caller.
 
-        :param event_id:
-        :param priority:
-        :return:
+        :param event_id: hashable identifier for the event
+        :param event: optional event instance
+        :return: the event instance after it has been dispatched
 
         """
+        if event is None:
+            event = Event()
 
-        def wrapper(listener):
-            self.add_listener(event_id, listener, priority)
-            return listener
+        # todo should name be part of dispatched event ?
+        event.name = event_id
+        event.dispatcher = self
 
-        return wrapper
+        self.do_dispatch(self._listeners.get(event_id), event)
 
-    def remove_listener(self, event_id, listener):
-        """
-        Remove a fiven listener from this event dispatcher. For now, if the listener is not registered for this event,
-        this method has no effect, but we may raise ValueError in the future if the given listener is not found, you
-        should catch it if you're not certain the listener is registered.
-
-        TODO raise ValueError if not found.
-
-        :param event_id:
-        :param listener:
-        :return:
-        """
-        if not event_id in self._listeners:
-            return
+        return cast(IDispatchedEvent, event)
 
-        for priority, listeners in self._listeners[event_id].items():
-            if listener in self._listeners[event_id][priority]:
-                # pylint: disable=filter-builtin-not-iterating
-                self._listeners[event_id][priority] = filter(
-                    lambda l: l != listener, self._listeners[event_id][priority]
-                )
-                if event_id in self._sorted:
-                    del self._sorted[event_id]
+    async def adispatch(self, event_id: str, event: Optional[IEvent] = None, /) -> IDispatchedEvent:
+        # allows to use the async interface with a sync dispatcher, although this is not recommended
+        # todo add a strict mode that raises an error when trying to use async interface with a sync dispatcher
+        return self.dispatch(event_id, event)
 
-    def do_dispatch(self, listeners, event):
+    def do_dispatch(self, listeners, event: IEvent, /):
         for listener in listeners:
             listener(event)
-            if event.propagation_stopped: break
-
-    def sort_listeners(self, event_id):
-        self._sorted[event_id] = []
-        if event_id in self._listeners:
-            self._sorted[event_id] = [
-                listener
-                for listeners in sorted(self._listeners[event_id].items(), key=operator.itemgetter(0))
-                for listener in listeners[1]
-            ]
+            if event.propagation_stopped:
+                break
```

### Comparing `whistle-1.0a3/whistle/event.py` & `whistle-2.0.0a1/whistle/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,13 +4,18 @@
     logic with your events, or just let the event dispatcher create instances for you
 
     The event handlers will have :class:`Event` instances passed, so you can bundle any data required by your handlers
     there.
 
     """
 
+    name = None
+    """Event name placeholder, will be set by dispatcher."""
+
+    dispatcher = None
+
     propagation_stopped = False
     """Has the event propagation ended?"""
 
     def stop_propagation(self):
         """Stop event propagation, meaning that the remaining handlers won't be called after this one."""
         self.propagation_stopped = True
```


# Comparing `tmp/pyeventmanager-0.4.1.tar.gz` & `tmp/pyeventmanager-0.5.0.tar.gz`

## Comparing `pyeventmanager-0.4.1.tar` & `pyeventmanager-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/event_manager/__init__.py
--rw-r--r--   0        0        0    16005 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/event_manager/event_manager.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/event_manager/fork_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/event_manager/listeners/__init__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/event_manager/listeners/base.py
--rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/event_manager/listeners/batch.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/event_manager/listeners/scheduled.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/event_manager/listeners/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/event_manager/queues/__init__.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/event_manager/queues/base.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/event_manager/queues/memory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/tests/test_dummy.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/.gitignore
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/README.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyeventmanager-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/event_manager/__init__.py
+-rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/event_manager/event_manager.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/event_manager/fork_types.py
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/event_manager/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/event_manager/listeners/__init__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/event_manager/listeners/base.py
+-rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/event_manager/listeners/batch.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/event_manager/listeners/scheduled.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/event_manager/listeners/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/event_manager/queues/__init__.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/event_manager/queues/base.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/event_manager/queues/memory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/tests/test_dummy.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/.gitignore
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/README.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 pyeventmanager-0.5.0/PKG-INFO
```

### Comparing `pyeventmanager-0.4.1/CHANGELOG.md` & `pyeventmanager-0.5.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Changelog
 
+## [0.5.0](https://github.com/JeordyR/PyEventManager/compare/v0.4.1...v1.0.0) (2024-04-01)
+
+
+### ⚠ BREAKING CHANGES
+
+* Added support for responses using Futures, changed EventManager to be static implementation.
+
+### Features
+
+* Added support for responses using Futures, changed EventManager to be static implementation. ([2f27db5](https://github.com/JeordyR/PyEventManager/commit/2f27db5f92fe5a827071a69112893ba09ea69474))
+
 ## [0.4.1](https://github.com/JeordyR/PyEventManager/compare/v0.4.0...v0.4.1) (2024-03-22)
 
 
 ### Bug Fixes
 
 * fix queues not storing and retrieving data as expected ([74d74c0](https://github.com/JeordyR/PyEventManager/commit/74d74c097762ad4ea296ccd89350ecdbf00d981e))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyeventmanager-0.4.1/.github/workflows/ci.yml` & `pyeventmanager-0.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.4.1/.github/workflows/docs.yml` & `pyeventmanager-0.5.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.4.1/event_manager/listeners/scheduled.py` & `pyeventmanager-0.5.0/event_manager/listeners/scheduled.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,29 +28,27 @@
 
 class ScheduledListener(BaseListener):
     def __init__(
         self,
         interval: timedelta,
         func: Callable,
         fork_type: ForkType,
-        recursive: bool = False,
     ):
         """
         Class for a basic listener in the event management system.
 
         Args:
             event (str): Event to match on.
             func (Callable): Function to call when listener triggers on a matching event.
             fork_type (ForkType, optional): Type of fork to use when running the function. Defaults to PROCESS.
         """
         self.event = ""
         self.interval = interval
         self.func = func
         self.fork_type = fork_type
-        self.recursive = recursive
         self.sync_event: MultieprocessingEvent | ThreadingEvent = (
             ThreadingEvent() if fork_type == ForkType.THREAD else MultiprocessingEventInit()
         )
 
     def __call__(self, *args, **kwargs):
         """
         Call invocation for the obejct, creates and runs a new fork with the stored function.
@@ -65,15 +63,15 @@
         kwargs = {
             "_interval": self.interval,
             "_func": self.func,
             "_event": self.sync_event,
             **kwargs,
         }
 
-        self.fork_type.value(target=run, daemon=not self.recursive, args=args, kwargs=kwargs).start()
+        self.fork_type.value(target=run, daemon=False, args=args, kwargs=kwargs).start()
 
     def stop(self):
         """
         Stop the scheduled listener.
         """
         logger.debug(f"Stopping {self.func.__name__} from running on schedule.")
         self.sync_event.set()
```

### Comparing `pyeventmanager-0.4.1/event_manager/listeners/simple.py` & `pyeventmanager-0.5.0/event_manager/listeners/simple.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,68 @@
 import inspect
 import logging
 from collections.abc import Callable
+from concurrent.futures import Future
 
 from event_manager.fork_types import ForkType
 from event_manager.listeners.base import BaseListener
 
 logger = logging.getLogger("event_manager")
 
 
+def _wrapper(_func: Callable, _future: Future, *args, **kwargs):
+    """
+    Wrapper function to run the function and store the result in the future.
+
+    Args:
+        _func (Callable): Function to run.
+        _future (Future): Future to store the result in.
+    """
+    if _future.set_running_or_notify_cancel():
+        try:
+            if inspect.getfullargspec(_func).args or inspect.getfullargspec(_func).kwonlyargs:
+                _future.set_result(_func(*args, **kwargs))
+            else:
+                _future.set_result(_func())
+        except Exception as e:
+            _future.set_exception(e)
+
+
 class Listener(BaseListener):
-    def __init__(self, event: str, func: Callable, fork_type: ForkType, recursive: bool = False):
+    def __init__(self, event: str, func: Callable, fork_type: ForkType):
         """
         Class for a basic listener in the event management system.
 
         Args:
             event (str): Event to match on.
             func (Callable): Function to call when listener triggers on a matching event.
             fork_type (ForkType, optional): Type of fork to use when running the function. Defaults to PROCESS.
         """
         self.func = func
         self.event = event
         self.fork_type = fork_type
-        self.recursive = recursive
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args, **kwargs) -> Future:
         """
         Call invocation for the obejct, creates and runs a new fork with the stored function.
 
         Arguments in the call are passed through to the stored function.
 
         Args:
             pool (Executor): Executor to run the function in.
         """
         logger.debug(f"Listener running func: {self.func.__name__}")
 
-        if inspect.getfullargspec(self.func).args or inspect.getfullargspec(self.func).kwonlyargs:
-            self.fork_type.value(target=self.func, daemon=not self.recursive, args=args, kwargs=kwargs).start()
-        else:
-            self.fork_type.value(target=self.func, daemon=not self.recursive).start()
+        future = Future()
+
+        self.fork_type.value(
+            target=_wrapper,
+            daemon=False,
+            args=args,
+            kwargs={
+                "_func": self.func,
+                "_future": future,
+                **kwargs,
+            },
+        ).start()
+
+        return future
```

### Comparing `pyeventmanager-0.4.1/event_manager/queues/base.py` & `pyeventmanager-0.5.0/event_manager/queues/base.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.4.1/event_manager/queues/memory.py` & `pyeventmanager-0.5.0/event_manager/queues/memory.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 
     def put(self, *args, **kwargs):
         """Put an item into the queue and update the last_updated attribute with curernt time."""
         self.last_updated = datetime.now()
 
         ThreadQueueBase.put(self, *args, **kwargs)
 
-    def get(self) -> Any:
+    def get(self, block: bool = False) -> Any:
         """Get an item from the queue."""
-        return ThreadQueueBase.get(self)
+        return ThreadQueueBase.get(self, block=block)
 
     def get_all(self) -> list[Any]:
         """
         Get and return all items from the queue
 
         Returns:
             list[Any]: List of all items from the queue.
@@ -70,17 +70,17 @@
 
     def put(self, *args, **kwargs):
         """Put an item into the queue and update the last_updated attribute with curernt time."""
         self.last_updated = datetime.now()
 
         ProcessingQueueBase.put(self, *args, **kwargs)
 
-    def get(self) -> Any:
+    def get(self, block: bool = False) -> Any:
         """Get an item from the queue."""
-        return ProcessingQueueBase.get(self)
+        return ProcessingQueueBase.get(self, block=block)
 
     def get_all(self) -> list[Any]:
         """
         Get and return all items from the queue
 
         Returns:
             list[Any]: List of all items from the queue.
```

### Comparing `pyeventmanager-0.4.1/.gitignore` & `pyeventmanager-0.5.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 __pycache__/
 *.py[cod]
 *$py.class
 .docs/
 junit/
 *.ipynb
 .ruff_cache/
+notes.md
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
```

### Comparing `pyeventmanager-0.4.1/README.md` & `pyeventmanager-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 [Read the Docs!](https://jeordyr.github.io/PyEventManager/)
 
 PyEventManager is a simple event-based routing package allowing code to be structured in a pseudo-decentralized manner.
 
 Instead of calling functions directly, you can emit an event and have one or more functions (listeners) configured to listen on that event execute. These listeners can currently be run either in a new thread or a new process, allowing the creation of background tasks for long-running jobs off an API event, for example.
 
+Wrapped listeners return a [Future](https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.Future) that can be waited on to recieve the response(s) back from the listener.
+
 There are multiple execution options when registering a listener:
 
 * **Simple**: Execute the function (listener) when the specified event is emitted.
 * **Batch**: Batch up the data from mulitple event emissions until no new events occur for `interval` seconds, then execute the function with all of the received data.
 * **Scheduled**: Run a function on an interval with no inputs.
 
 For each listener type, there are multiple execution options determining how the function will be executed; determined by `fork_type`
@@ -20,16 +22,15 @@
 ---
 
 ## Todo
 
 * Add tests
 * Add support for async execution within an existing event loop
 * Add support for external data stores (redis, rabbitmq?, etc.) for persistence of event data / batching
-* Consider adding support for returning data from the listeners
-* ~~Fix up docstrings across the board~~
+
 
 ---
 
 ## Installation
 
 Install via [pip](https://pypi.python.org/pypi/pyeventmanager)
 
@@ -49,30 +50,32 @@
     # Use a decorator to register a simple listener
 
     @em.on(event="somecategory.event")
     def handle_some_event(data: MyDataType):
         ...
 
     # Register a function to handle all events in the system
-    @em.on_all()
+    @em.on(event="*")
     def handle_all_events(data: Any):
         ...
 
     # Register a function to handle all events for a category using wildcard
     @em.on(event="somecategory.*")
     def handle_all_somecategory_events(data: Any):
         ...
 
     # Register a simple listener using callback syntax
     def also_handle_some_event(data: MyDataType):
         ...
 
     em.on(event="somecategory.event", func=also_handle_some_event)
 
-    # Emit an event without worrying about response
+    # Emit an event passing data
+    ## *args, **kwargs are passed through to listener,
+    ##  so any fields can be used as long as the matching listener accepts the same
     em.emit(event="somecategory.event", data=MyDataType(...))
 
     # Emit an event, wait for jobs to finish, and get the results
     from concurrent.futures import wait
 
     futures = em.emit(event="somecategory.event, data=MyDataType(...))
     wait(futures)
@@ -85,39 +88,45 @@
 ```python
     from event_manager import EventManager, ForkType
 
     em = EventManager()
 
     # Use Threading instead of Processing
     @em.on(event="something.*", fork_type=ForkType.THREAD)
+    def handle_something():
+        ...
+```
 
 ### Batch Listener
 
-.. code-block:: python
-
+```python
     from event_manager import EventManager, ForkType, ThreadQueue
 
     em = EventManager()
 
     # Batch all data for `category.some_event` until no new events occur for 60 seconds
-    @em.on(event="category.some_event", batch=True, batch_window=60)
+    @em.on_batch(event="category.some_event", batch_idle_window=60)
     def handle_some_event_batch(data: list[MyDataType]):
         ...
 
     # Same batch, using Threading.
     # The queue type will be auto-detected if not specified, but better to be explicit.
     @em.on(
         event="category.some_event",
         fork_type=ForkType.THREAD,
-        batch=True,
-        batch_window=60,
+        batch_idle_window=60,
         queue_type=ThreadQueue,
     )
     def handle_some_event_batch(data: list[MyDataType]):
         ...
+
+    # Batch data until 30 seconds pass, or 20 events come through, whichever happends first
+    @em.on_batch(event="category.some_event", batch_count=20, batch_window=30)
+    def handle_some_event_batch(data: list[MyDataType]):
+        ...
 ```
 
 ### Scheduled Listener
 
 Interval is defined using a [datetime.timedelta](https://docs.python.org/3/library/datetime.html#timedelta-objects) object.
 
 ```python
@@ -132,19 +141,19 @@
     def run_daily():
         ...
 
     # Schedule a function to be run hourly
     @em.schedule(interval=timedelta(hours=1))
     def run_hourly():
         ...
+```
 
 ### Using A Custom Queue for Batch Listener
 
-.. code-block:: python
-
+```python
     from datetime import datetime
     from typing import Any
 
     from event_manager import EventManager, ForkType, QueueInterface
 
     class MyCustomQueue(QueueInterface):
         last_updated: datetime | None
@@ -183,27 +192,25 @@
             ...
 
     em = EventManager()
 
     # Add a batched listener and pass in our custom Queue implementation
     @em.on(
         event="category.some_event",
-        batch=True,
-        batch_window=60,
+        batch_idle_window=60,
         queue_type=MyCustomQueue,
     )
     def handle_batch_process(data: list[Any]):
         ...
 
     # Add a batched listener configured to use Threading with our custom Queue implementation
     @em.on(
         event="category.some_event",
         fork_type=ForkType.THREAD,
-        batch=True,
-        batch_window=60,
+        batch_idle_window=60,
         queue_type=MyCustomQueue,
     )
     def handle_batch_process(data: list[Any]):
         ...
 ```
 
 ---
```

### Comparing `pyeventmanager-0.4.1/pyproject.toml` & `pyeventmanager-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyeventmanager"
-version = "0.4.1"
+version = "0.5.0"
 authors = [{ name = "Jeordy", email = "JeordyR@users.noreply.github.com" }]
 description = "Event management system for Python with support for Threading and Multiprocessing for task running."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
```

### Comparing `pyeventmanager-0.4.1/PKG-INFO` & `pyeventmanager-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyeventmanager
-Version: 0.4.1
+Version: 0.5.0
 Summary: Event management system for Python with support for Threading and Multiprocessing for task running.
 Project-URL: Documentation, https://event-manager.jeofi.com
 Project-URL: Homepage, https://event-manager.jeofi.com
 Project-URL: Repository, https://github.com/JeordyR/PyEventManager
 Project-URL: Issues, https://github.com/JeordyR/PyEventManager/issues
 Author-email: Jeordy <JeordyR@users.noreply.github.com>
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,16 @@
 
 [Read the Docs!](https://jeordyr.github.io/PyEventManager/)
 
 PyEventManager is a simple event-based routing package allowing code to be structured in a pseudo-decentralized manner.
 
 Instead of calling functions directly, you can emit an event and have one or more functions (listeners) configured to listen on that event execute. These listeners can currently be run either in a new thread or a new process, allowing the creation of background tasks for long-running jobs off an API event, for example.
 
+Wrapped listeners return a [Future](https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.Future) that can be waited on to recieve the response(s) back from the listener.
+
 There are multiple execution options when registering a listener:
 
 * **Simple**: Execute the function (listener) when the specified event is emitted.
 * **Batch**: Batch up the data from mulitple event emissions until no new events occur for `interval` seconds, then execute the function with all of the received data.
 * **Scheduled**: Run a function on an interval with no inputs.
 
 For each listener type, there are multiple execution options determining how the function will be executed; determined by `fork_type`
@@ -35,16 +37,15 @@
 ---
 
 ## Todo
 
 * Add tests
 * Add support for async execution within an existing event loop
 * Add support for external data stores (redis, rabbitmq?, etc.) for persistence of event data / batching
-* Consider adding support for returning data from the listeners
-* ~~Fix up docstrings across the board~~
+
 
 ---
 
 ## Installation
 
 Install via [pip](https://pypi.python.org/pypi/pyeventmanager)
 
@@ -64,30 +65,32 @@
     # Use a decorator to register a simple listener
 
     @em.on(event="somecategory.event")
     def handle_some_event(data: MyDataType):
         ...
 
     # Register a function to handle all events in the system
-    @em.on_all()
+    @em.on(event="*")
     def handle_all_events(data: Any):
         ...
 
     # Register a function to handle all events for a category using wildcard
     @em.on(event="somecategory.*")
     def handle_all_somecategory_events(data: Any):
         ...
 
     # Register a simple listener using callback syntax
     def also_handle_some_event(data: MyDataType):
         ...
 
     em.on(event="somecategory.event", func=also_handle_some_event)
 
-    # Emit an event without worrying about response
+    # Emit an event passing data
+    ## *args, **kwargs are passed through to listener,
+    ##  so any fields can be used as long as the matching listener accepts the same
     em.emit(event="somecategory.event", data=MyDataType(...))
 
     # Emit an event, wait for jobs to finish, and get the results
     from concurrent.futures import wait
 
     futures = em.emit(event="somecategory.event, data=MyDataType(...))
     wait(futures)
@@ -100,39 +103,45 @@
 ```python
     from event_manager import EventManager, ForkType
 
     em = EventManager()
 
     # Use Threading instead of Processing
     @em.on(event="something.*", fork_type=ForkType.THREAD)
+    def handle_something():
+        ...
+```
 
 ### Batch Listener
 
-.. code-block:: python
-
+```python
     from event_manager import EventManager, ForkType, ThreadQueue
 
     em = EventManager()
 
     # Batch all data for `category.some_event` until no new events occur for 60 seconds
-    @em.on(event="category.some_event", batch=True, batch_window=60)
+    @em.on_batch(event="category.some_event", batch_idle_window=60)
     def handle_some_event_batch(data: list[MyDataType]):
         ...
 
     # Same batch, using Threading.
     # The queue type will be auto-detected if not specified, but better to be explicit.
     @em.on(
         event="category.some_event",
         fork_type=ForkType.THREAD,
-        batch=True,
-        batch_window=60,
+        batch_idle_window=60,
         queue_type=ThreadQueue,
     )
     def handle_some_event_batch(data: list[MyDataType]):
         ...
+
+    # Batch data until 30 seconds pass, or 20 events come through, whichever happends first
+    @em.on_batch(event="category.some_event", batch_count=20, batch_window=30)
+    def handle_some_event_batch(data: list[MyDataType]):
+        ...
 ```
 
 ### Scheduled Listener
 
 Interval is defined using a [datetime.timedelta](https://docs.python.org/3/library/datetime.html#timedelta-objects) object.
 
 ```python
@@ -147,19 +156,19 @@
     def run_daily():
         ...
 
     # Schedule a function to be run hourly
     @em.schedule(interval=timedelta(hours=1))
     def run_hourly():
         ...
+```
 
 ### Using A Custom Queue for Batch Listener
 
-.. code-block:: python
-
+```python
     from datetime import datetime
     from typing import Any
 
     from event_manager import EventManager, ForkType, QueueInterface
 
     class MyCustomQueue(QueueInterface):
         last_updated: datetime | None
@@ -198,27 +207,25 @@
             ...
 
     em = EventManager()
 
     # Add a batched listener and pass in our custom Queue implementation
     @em.on(
         event="category.some_event",
-        batch=True,
-        batch_window=60,
+        batch_idle_window=60,
         queue_type=MyCustomQueue,
     )
     def handle_batch_process(data: list[Any]):
         ...
 
     # Add a batched listener configured to use Threading with our custom Queue implementation
     @em.on(
         event="category.some_event",
         fork_type=ForkType.THREAD,
-        batch=True,
-        batch_window=60,
+        batch_idle_window=60,
         queue_type=MyCustomQueue,
     )
     def handle_batch_process(data: list[Any]):
         ...
 ```
 
 ---
```


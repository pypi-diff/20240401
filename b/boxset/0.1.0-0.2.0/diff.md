# Comparing `tmp/boxset-0.1.0-py3-none-any.whl.zip` & `tmp/boxset-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,7 @@
-Zip file size: 2546 bytes, number of entries: 6
--rw-rw-r--  2.0 unx       19 b- defN 24-Mar-29 08:33 __init__.py
--rw-rw-r--  2.0 unx     2798 b- defN 24-Mar-29 08:49 util.py
--rw-rw-r--  2.0 unx      600 b- defN 24-Mar-29 08:51 boxset-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-29 08:51 boxset-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 24-Mar-29 08:51 boxset-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      423 b- defN 24-Mar-29 08:51 boxset-0.1.0.dist-info/RECORD
-6 files, 3946 bytes uncompressed, 1784 bytes compressed:  54.8%
+Zip file size: 2616 bytes, number of entries: 5
+-rw-r--r--  2.0 unx       42 b- defN 24-Apr-01 16:43 boxset/__init__.py
+-rw-r--r--  2.0 unx     3669 b- defN 24-Apr-01 12:01 boxset/util.py
+-rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 boxset-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      609 b- defN 16-Jan-01 00:00 boxset-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      346 b- defN 16-Jan-01 00:00 boxset-0.2.0.dist-info/RECORD
+5 files, 4747 bytes uncompressed, 1974 bytes compressed:  58.4%
```

## zipnote {}

```diff
@@ -1,19 +1,16 @@
-Filename: __init__.py
+Filename: boxset/__init__.py
 Comment: 
 
-Filename: util.py
+Filename: boxset/util.py
 Comment: 
 
-Filename: boxset-0.1.0.dist-info/METADATA
+Filename: boxset-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: boxset-0.1.0.dist-info/WHEEL
+Filename: boxset-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: boxset-0.1.0.dist-info/top_level.txt
-Comment: 
-
-Filename: boxset-0.1.0.dist-info/RECORD
+Filename: boxset-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `util.py` & `boxset/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,29 @@
+import functools
 import itertools
-from typing import Any, Callable, Generator, Sequence, Union
+import time
+from threading import Lock
+from typing import Any, Callable, Generator, Iterable
 
-def split_list(
-    iterable: Sequence[Any],
+
+def split_seq(
+    iterable: Iterable[Any],
     size: int,
-    callback: Union[Callable[[Any], Any], None] = None,
-    is_skip_empty: bool = True,
 ) -> Generator[list[Any], None, None]:
     """
     Split a long sequence into smaller chunks of given size.
-
-    Args:
-        iterable (Sequence[Any]): The sequence to be split.
-        size (int): The maximum size of each chunk.
-        callback (Union[Callable[[Any], Any], None], optional): A function to apply to each item before adding to the chunk. Defaults to None.
-        is_skip_empty (bool, optional): Whether to skip empty items after applying the callback. Defaults to True.
-
     Yields:
         Generator[list[Any], None, None]: A generator that yields lists of items.
 
     Examples:
-        >>> list(split_list(range(10), 3))
+        >>> list(split_seq(range(10), 3))
         [[0, 1, 2], [3, 4, 5], [6, 7, 8], [9]]
 
-        >>> list(split_list([1, 2, '', 3, None, 4], 2, is_skip_empty=False))
-        [[1, 2], ['', 3], [None, 4]]
-
-        # >>> list(split_list([1, 2, 0, 3, False, 4], 2, lambda x: x and str(x), is_skip_empty=True))
-        # [['1', '2'], ['3', '4']]
+        >>> list(split_seq(range(10), 2))
+        [[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]
     """
     # iterator: Iterator[Any] = iter(iterable)
     # while True:
     #     res: list[Any] = []
     #     try:
     #         for _ in range(size):
     #             item = next(iterator)
@@ -41,25 +33,25 @@
     #                 res.append(item)
     #     except StopIteration:
     #         if res:
     #             yield res
     #         break
     #     else:
     #         yield res
-
     it = iter(iterable)
     item = list(itertools.islice(it, size))
     while item:
         yield item
         item = list(itertools.islice(it, size))
 
+
 # 10的3次方
-ONE_K = 10 ** 3
-ONE_W = 10 ** 4
-ONE_KW = 10 ** 7
+ONE_K = 10**3
+ONE_W = 10**4
+ONE_KW = 10**7
 
 
 def cn_human_number(num):
     """
     Convert a number to a human-readable string representation.
 
     Args:
@@ -87,10 +79,67 @@
     elif num < ONE_KW:
         return f"{num/ONE_W:.1f}w"
     elif num < 100 * ONE_KW:
         return f"{num/ONE_KW:.1f}kw"
     else:
         # 科学计数法
         return f"{num:.1e}"
-    
+
+
+def delay_decorator(delay_seconds: float) -> Callable:
+    """
+    Decorator that delays the execution of a function by a specified number of seconds.
+
+    Args:
+        delay_seconds (float): The number of seconds to delay the function execution.
+
+    Returns:
+        Callable: The decorated function.
+
+    Examples:
+        >>> import time
+        >>> @delay_decorator(0.5)
+        ... def my_func():
+        ...     return time.time()
+        ...
+        >>> my_func() - time.time() > -0.01 # 第一次调用不会延迟
+        True
+        >>> my_func() - my_func() < -0.5
+        True
+
+        >>> @delay_decorator(0.5)
+        ... def add(a, b):
+        ...     return a + b
+        ...
+        >>> add(1, 2)
+        3
+        >>> add(3, 4)
+        7
+    """
+
+    def decorator(func: Callable) -> Callable:
+        last_executed: float = 0
+        lock = Lock()
+
+        @functools.wraps(func)
+        def wrapper(*args: Any, **kwargs: Any) -> Any:
+            nonlocal last_executed
+            current_time = time.time()
+            time_diff = current_time - last_executed
+
+            with lock:
+                if time_diff < delay_seconds and last_executed != 0:
+                    wait_time = delay_seconds - time_diff
+                    time.sleep(wait_time)
+
+                result = func(*args, **kwargs)
+                last_executed = time.time()
+
+            return result
+
+        return wrapper
+
+    return decorator
+
+
 # 可以减少智能匹配的推荐量
-__all__ = ["split_list", "cn_human_number"]
+__all__ = ["split_seq", "cn_human_number", "delay_decorator"]
```

## Comparing `boxset-0.1.0.dist-info/METADATA` & `boxset-0.2.0.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: boxset
-Version: 0.1.0
+Version: 0.2.0
 Summary: this is a set of many useful boxing functions
 Author-email: pyhacker <abuse@example.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+
+# empty
```


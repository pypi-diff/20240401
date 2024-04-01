# Comparing `tmp/arq-0.8.1.tar.gz` & `tmp/arq-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arq-0.8.1.tar", last modified: Mon Jun  5 19:56:42 2017, max compression
+gzip compressed data, was "dist/arq-0.9.tar", last modified: Fri Jun 23 10:58:10 2017, max compression
```

## Comparing `arq-0.8.1.tar` & `arq-0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-05 19:56:42.000000 arq-0.8.1/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-05 19:56:42.000000 arq-0.8.1/arq/
--rw-r--r--   0 travis    (1000) travis    (1000)      238 2017-06-05 19:55:47.000000 arq-0.8.1/arq/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1137 2017-06-05 19:55:47.000000 arq-0.8.1/arq/cli.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6716 2017-06-05 19:55:47.000000 arq-0.8.1/arq/drain.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4480 2017-06-05 19:55:47.000000 arq-0.8.1/arq/jobs.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1840 2017-06-05 19:55:47.000000 arq-0.8.1/arq/logs.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7831 2017-06-05 19:55:47.000000 arq-0.8.1/arq/main.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4307 2017-06-05 19:55:47.000000 arq-0.8.1/arq/testing.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6255 2017-06-05 19:55:47.000000 arq-0.8.1/arq/utils.py
--rw-r--r--   0 travis    (1000) travis    (1000)      101 2017-06-05 19:55:47.000000 arq-0.8.1/arq/version.py
--rw-r--r--   0 travis    (1000) travis    (1000)    19713 2017-06-05 19:55:47.000000 arq-0.8.1/arq/worker.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-05 19:56:42.000000 arq-0.8.1/arq.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     1997 2017-06-05 19:56:42.000000 arq-0.8.1/arq.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      348 2017-06-05 19:56:42.000000 arq-0.8.1/arq.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-06-05 19:56:42.000000 arq-0.8.1/arq.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       55 2017-06-05 19:56:42.000000 arq-0.8.1/arq.egg-info/entry_points.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       95 2017-06-05 19:56:42.000000 arq-0.8.1/arq.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        4 2017-06-05 19:56:42.000000 arq-0.8.1/arq.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-06-05 19:56:03.000000 arq-0.8.1/arq.egg-info/zip-safe
--rw-r--r--   0 travis    (1000) travis    (1000)      683 2017-06-05 19:55:47.000000 arq-0.8.1/README.rst
--rw-r--r--   0 travis    (1000) travis    (1000)      187 2017-06-05 19:56:42.000000 arq-0.8.1/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     1905 2017-06-05 19:55:47.000000 arq-0.8.1/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1997 2017-06-05 19:56:42.000000 arq-0.8.1/PKG-INFO
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-23 10:58:10.000000 arq-0.9/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-23 10:58:10.000000 arq-0.9/arq/
+-rw-r--r--   0 travis    (1000) travis    (1000)      238 2017-06-23 10:56:34.000000 arq-0.9/arq/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1137 2017-06-23 10:56:34.000000 arq-0.9/arq/cli.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     6716 2017-06-23 10:56:34.000000 arq-0.9/arq/drain.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4769 2017-06-23 10:56:34.000000 arq-0.9/arq/jobs.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1840 2017-06-23 10:56:34.000000 arq-0.9/arq/logs.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    13058 2017-06-23 10:56:34.000000 arq-0.9/arq/main.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4307 2017-06-23 10:56:34.000000 arq-0.9/arq/testing.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     9203 2017-06-23 10:56:34.000000 arq-0.9/arq/utils.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      101 2017-06-23 10:56:34.000000 arq-0.9/arq/version.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    19917 2017-06-23 10:56:34.000000 arq-0.9/arq/worker.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-23 10:58:10.000000 arq-0.9/arq.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1995 2017-06-23 10:58:10.000000 arq-0.9/arq.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      348 2017-06-23 10:58:10.000000 arq-0.9/arq.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-06-23 10:58:10.000000 arq-0.9/arq.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       55 2017-06-23 10:58:10.000000 arq-0.9/arq.egg-info/entry_points.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       95 2017-06-23 10:58:10.000000 arq-0.9/arq.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        4 2017-06-23 10:58:10.000000 arq-0.9/arq.egg-info/top_level.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-06-23 10:56:59.000000 arq-0.9/arq.egg-info/zip-safe
+-rw-r--r--   0 travis    (1000) travis    (1000)      683 2017-06-23 10:56:34.000000 arq-0.9/README.rst
+-rw-r--r--   0 travis    (1000) travis    (1000)      288 2017-06-23 10:58:10.000000 arq-0.9/setup.cfg
+-rw-r--r--   0 travis    (1000) travis    (1000)     1905 2017-06-23 10:56:34.000000 arq-0.9/setup.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1995 2017-06-23 10:58:10.000000 arq-0.9/PKG-INFO
```

### Comparing `arq-0.8.1/arq/cli.py` & `arq-0.9/arq/cli.py`

 * *Files identical despite different names*

### Comparing `arq-0.8.1/arq/drain.py` & `arq-0.9/arq/drain.py`

 * *Files identical despite different names*

### Comparing `arq-0.8.1/arq/jobs.py` & `arq-0.9/arq/jobs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 """
 :mod:`jobs`
 ===========
 
 Defines the ``Job`` class and descendants which deal with encoding and decoding job data.
 """
 from datetime import datetime
-from typing import Callable
 
 import msgpack
 
-from .utils import DEFAULT_CURTAIL, ellipsis, from_unix_ms, timestamp, to_unix_ms
+from .utils import DEFAULT_CURTAIL, from_unix_ms, timestamp, to_unix_ms_tz, truncate
 
 __all__ = ['JobSerialisationError', 'Job', 'DatetimeJob']
 
 
 class ArqError(Exception):
     pass
 
 
 class JobSerialisationError(ArqError):
     pass
 
 
+# "device control one" should be fairly unique as a dict key and only one byte
+DEVICE_CONTROL_ONE = '\x11'
+
+
 class Job:
     """
     Main Job class responsible for encoding and decoding jobs as they go
     into and come out of redis.
     """
     __slots__ = ('queue', 'queued_at', 'class_name', 'func_name', 'args', 'kwargs', 'raw_queue', 'raw_data')
 
-    #: custom encoder for msgpack, see :class:`arq.jobs.DatetimeJob` for an example of usage
-    msgpack_encoder: Callable = None
-
-    #: custom object hook for msgpack, see :class:`arq.jobs.DatetimeJob` for an example of usage
-    msgpack_object_hook: Callable = None
-
     def __init__(self, raw_data: bytes, *, queue_name: str=None, raw_queue: bytes=None) -> None:
         """
         Create a job instance be decoding a job definition eg. from redis.
 
         :param raw_data: data to decode, as created by :meth:`arq.jobs.Job.encode`
         :param raw_queue: raw name of the queue the job was taken from
         :param queue_name: name of the queue the job was dequeued from
@@ -67,14 +64,30 @@
         queued_at = queued_at or int(timestamp() * 1000)
         try:
             return cls._encode([queued_at, class_name, func_name, args, kwargs])
         except TypeError as e:
             raise JobSerialisationError(str(e)) from e
 
     @classmethod
+    def msgpack_encoder(cls, obj):
+        """
+        The default msgpack encoder, adds support for encoding sets.
+        """
+        if isinstance(obj, set):
+            return {DEVICE_CONTROL_ONE: list(obj)}
+        else:
+            return obj
+
+    @classmethod
+    def msgpack_object_hook(cls, obj):
+        if len(obj) == 1 and DEVICE_CONTROL_ONE in obj:
+            return set(obj[DEVICE_CONTROL_ONE])
+        return obj
+
+    @classmethod
     def _encode(cls, data) -> bytes:
         return msgpack.packb(data, default=cls.msgpack_encoder, use_bin_type=True)
 
     @classmethod
     def _decode(cls, data: bytes):
         return msgpack.unpackb(data, object_hook=cls.msgpack_object_hook, encoding='utf8')
 
@@ -83,43 +96,43 @@
         if self.args:
             arguments = ', '.join(map(str, self.args))
         if self.kwargs:
             if arguments:
                 arguments += ', '
             arguments += ', '.join(f'{k}={v!r}' for k, v in sorted(self.kwargs.items()))
 
-        return '{s.class_name}.{s.func_name}({args})'.format(s=self, args=ellipsis(arguments, args_curtail))
+        return '{s.class_name}.{s.func_name}({args})'.format(s=self, args=truncate(arguments, args_curtail))
 
     def __str__(self):
         return self.to_string()
 
     def __repr__(self):
         return f'<Job {self} on {self.queue}>'
 
 
-# unicode clock is small to encode and should be fairly unlikely to clash with another dict key
-DATETIME = '⌚'
+DEVICE_CONTROL_TWO = '\x12'
 TIMEZONE = 'O'
 
 
 class DatetimeJob(Job):
     """
     Alternative Job which copes with datetimes. None timezone naïve dates are supported but
     the returned datetimes will use a :mod:`datetime.timezone` class to define the timezone
     regardless of the timezone class originally used on the datetime object (eg. ``pytz``).
     """
-    @staticmethod
-    def msgpack_encoder(obj):
+    @classmethod
+    def msgpack_encoder(cls, obj):
         if isinstance(obj, datetime):
-            ts, tz = to_unix_ms(obj)
-            result = {DATETIME: ts}
+            ts, tz = to_unix_ms_tz(obj)
+            result = {DEVICE_CONTROL_TWO: ts}
             if tz is not None:
                 result[TIMEZONE] = tz
             return result
         else:
-            return obj
+            return super().msgpack_encoder(obj)
 
-    @staticmethod
-    def msgpack_object_hook(obj):
-        if DATETIME in obj and len(obj) <= 2:
-            return from_unix_ms(obj[DATETIME], utcoffset=obj.get(TIMEZONE))
-        return obj
+    @classmethod
+    def msgpack_object_hook(cls, obj):
+        if len(obj) <= 2 and DEVICE_CONTROL_TWO in obj:
+            return from_unix_ms(obj[DEVICE_CONTROL_TWO], utcoffset=obj.get(TIMEZONE))
+        else:
+            return super().msgpack_object_hook(obj)
```

### Comparing `arq-0.8.1/arq/logs.py` & `arq-0.9/arq/logs.py`

 * *Files identical despite different names*

### Comparing `arq-0.8.1/arq/testing.py` & `arq-0.9/arq/testing.py`

 * *Files identical despite different names*

### Comparing `arq-0.8.1/arq/utils.py` & `arq-0.9/arq/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from datetime import datetime, timedelta, timezone
 from typing import Tuple, Union
 
 import aioredis
 from aioredis.pool import RedisPool
 from async_timeout import timeout
 
-__all__ = ['RedisSettings', 'RedisMixin']
+__all__ = ['RedisSettings', 'RedisMixin', 'next_cron']
 logger = logging.getLogger('arq.utils')
 
 
 class RedisSettings:
     """
     No-Op class used to hold redis connection redis_settings.
     """
@@ -131,29 +131,38 @@
     This should be exactly the same as time.time(), we use this approach for consistency with
     other methods and possibly greater accuracy.
     :return: now in unix time, eg. seconds since 1970
     """
     return (datetime.utcnow() - EPOCH).total_seconds()
 
 
-def to_unix_ms(dt: datetime) -> Tuple[int, Union[int, None]]:
+def to_unix_ms_tz(dt: datetime) -> Tuple[int, Union[int, None]]:
     """
-    convert a datetime to number of milliseconds since 1970
+    convert a datetime to number of milliseconds since 1970 and calculate timezone offset
     :param dt: datetime to evaluate
     :return: tuple - (unix time in milliseconds, utc offset in seconds)
     """
     utcoffset = dt.utcoffset()
     if utcoffset is not None:
         _utcoffset = utcoffset.total_seconds()
         unix = (dt - EPOCH_TZ).total_seconds() + _utcoffset
         return int(unix * 1000), int(_utcoffset)
     else:
         return int((dt - EPOCH).total_seconds() * 1000), None
 
 
+def to_unix_ms(dt: datetime) -> int:
+    """
+    convert a datetime to number of milliseconds since 1970
+    :param dt: datetime to evaluate
+    :return: unix time in milliseconds
+    """
+    return to_unix_ms_tz(dt)[0]
+
+
 def from_unix_ms(ms: int, utcoffset: int=None) -> datetime:
     """
     convert int to a datetime.
 
     :param ms: number of milliseconds since 1970
     :param utcoffset: if set a timezone i added to the datime based on the offset in seconds.
     :return: datetime - including timezone if utcoffset is not None, else timezone naïve
@@ -172,17 +181,96 @@
     """
     return base64.urlsafe_b64encode(os.urandom(length))[:length]
 
 
 DEFAULT_CURTAIL = 80
 
 
-def ellipsis(s: str, length: int=DEFAULT_CURTAIL) -> str:
+def truncate(s: str, length: int=DEFAULT_CURTAIL) -> str:
     """
     Truncate a string and add an ellipsis (three dots) to the end if it was too long
 
     :param s: string to possibly truncate
     :param length: length to truncate the string to
     """
     if len(s) > length:
         s = s[:length - 1] + '…'
     return s
+
+
+_dt_fields = [
+    'month',
+    'day',
+    'weekday',
+    'hour',
+    'minute',
+    'second',
+    'microsecond',
+]
+
+
+def _get_next_dt(dt_, options):  # noqa: C901
+    for field in _dt_fields:
+        v = options[field]
+        if v is None:
+            continue
+        if field == 'weekday':
+            next_v = dt_.weekday()
+        else:
+            next_v = getattr(dt_, field)
+        if isinstance(v, int):
+            mismatch = next_v != v
+        else:
+            assert isinstance(v, (set, list, tuple))
+            mismatch = next_v not in v
+        # print(field, v, next_v, mismatch)
+        if mismatch:
+            micro = max(dt_.microsecond - options['microsecond'], 0)
+            if field == 'month':
+                if dt_.month == 12:
+                    return datetime(dt_.year + 1, 1, 1)
+                else:
+                    return datetime(dt_.year, dt_.month + 1, 1)
+            elif field in ('day', 'weekday'):
+                return dt_ + timedelta(days=1) - timedelta(hours=dt_.hour, minutes=dt_.minute, seconds=dt_.second,
+                                                           microseconds=micro)
+            elif field == 'hour':
+                return dt_ + timedelta(hours=1) - timedelta(minutes=dt_.minute, seconds=dt_.second, microseconds=micro)
+            elif field == 'minute':
+                return dt_ + timedelta(minutes=1) - timedelta(seconds=dt_.second, microseconds=micro)
+            elif field == 'second':
+                return dt_ + timedelta(seconds=1) - timedelta(microseconds=micro)
+            else:
+                assert field == 'microsecond'
+                return dt_ + timedelta(microseconds=options['microsecond'] - dt_.microsecond)
+
+
+def next_cron(preview_dt: datetime, *,
+              month: Union[None, set, int]=None,
+              day: Union[None, set, int]=None,
+              weekday: Union[None, set, int, str]=None,
+              hour: Union[None, set, int]=None,
+              minute: Union[None, set, int]=None,
+              second: Union[None, set, int]=0,
+              microsecond: int=123456):
+    """
+    Find the next datetime matching the given parameters.
+    """
+    dt = preview_dt + timedelta(seconds=1)
+    if isinstance(weekday, str):
+        weekday = ['mon', 'tues', 'wed', 'thurs', 'fri', 'sat', 'sun'].index(weekday.lower())
+    options = dict(
+        month=month,
+        day=day,
+        weekday=weekday,
+        hour=hour,
+        minute=minute,
+        second=second,
+        microsecond=microsecond,
+    )
+
+    while True:
+        next_dt = _get_next_dt(dt, options)
+        # print(dt, next_dt)
+        if next_dt is None:
+            return dt
+        dt = next_dt
```

### Comparing `arq-0.8.1/arq/worker.py` & `arq-0.9/arq/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from async_timeout import timeout
 
 from .drain import Drain
 from .jobs import ArqError, Job
 from .logs import default_log_config
 from .main import Actor  # noqa
-from .utils import RedisMixin, ellipsis, timestamp
+from .utils import RedisMixin, timestamp, truncate
 
 __all__ = ['BaseWorker', 'RunWorkerProcess', 'StopJob', 'import_string']
 
 work_logger = logging.getLogger('arq.work')
 ctrl_logger = logging.getLogger('arq.control')
 jobs_logger = logging.getLogger('arq.jobs')
 
@@ -228,23 +228,28 @@
 
         Also regularly runs ``record_health``.
         """
         redis_queues, queue_lookup = self.get_redis_queues()
         original_redis_queues = list(redis_queues)
 
         async with self.drain:
-            await self.record_health(original_redis_queues, queue_lookup)
+            await self.heart_beat(original_redis_queues, queue_lookup)
             async for raw_queue, raw_data in self.drain.iter(*redis_queues):
                 if raw_queue is not None:
                     job = self.job_class(raw_data, queue_name=queue_lookup[raw_queue], raw_queue=raw_queue)
                     shadow = self._shadow_lookup.get(job.class_name)
                     re_enqueue = shadow and getattr(shadow, 're_enqueue_jobs', False)
                     work_logger.debug('scheduling job %r, re-enqueue: %r', job, re_enqueue)
                     self.drain.add(self.run_job, job, re_enqueue)
-                await self.record_health(original_redis_queues, queue_lookup)
+                await self.heart_beat(original_redis_queues, queue_lookup)
+
+    async def heart_beat(self, redis_queues, queue_lookup):
+        await self.record_health(redis_queues, queue_lookup)
+        for shadow in self._shadow_lookup.values():
+            await shadow.run_cron()
 
     async def record_health(self, redis_queues, queue_lookup):
         now_ts = timestamp()
         if (now_ts - self.last_health_check) < self.health_check_interval:
             return
         self.last_health_check = now_ts
         pending_tasks = sum(not t.done() for t in self.drain.pending_tasks)
@@ -318,15 +323,15 @@
             job_str = j.to_string(self.log_curtail)
             jobs_logger.info('%-4s queued%7.3fs → %s', j.queue, started_at - j.queued_at, job_str)
 
     def log_job_result(self, started_at: float, result, j: Job):
         if not jobs_logger.isEnabledFor(logging.INFO):
             return
         job_time = timestamp() - started_at
-        sr = '' if result is None else ellipsis(repr(result), self.log_curtail)
+        sr = '' if result is None else truncate(repr(result), self.log_curtail)
         jobs_logger.info('%-4s ran in%7.3fs ← %s.%s ● %s', j.queue, job_time, j.class_name, j.func_name, sr)
 
     def handle_prepare_exc(self, msg: str):
         self.drain.jobs_failed += 1
         jobs_logger.error(msg)
         # exit with zero so we don't increment jobs_failed twice
         return 0
```

### Comparing `arq-0.8.1/arq.egg-info/PKG-INFO` & `arq-0.9/arq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arq
-Version: 0.8.1
+Version: 0.9
 Summary: Job queues in python with asyncio, redis and msgpack.
 Home-page: https://github.com/samuelcolvin/arq
 Author: Samuel Colvin
 Author-email: s@muelcolvin.com
 License: MIT
 Description: arq
         ===
```

### Comparing `arq-0.8.1/README.rst` & `arq-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `arq-0.8.1/setup.py` & `arq-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `arq-0.8.1/PKG-INFO` & `arq-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arq
-Version: 0.8.1
+Version: 0.9
 Summary: Job queues in python with asyncio, redis and msgpack.
 Home-page: https://github.com/samuelcolvin/arq
 Author: Samuel Colvin
 Author-email: s@muelcolvin.com
 License: MIT
 Description: arq
         ===
```


# Comparing `tmp/pg8000-1.9.8.tar.gz` & `tmp/pg8000-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pg8000-1.9.8.tar", last modified: Mon May  5 12:35:25 2014, max compression
+gzip compressed data, was "dist/pg8000-1.9.9.tar", last modified: Mon May 12 19:26:22 2014, max compression
```

## Comparing `pg8000-1.9.8.tar` & `pg8000-1.9.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2014-05-05 12:35:25.000000 pg8000-1.9.8/
--rw-r--r--   0 tlocke    (1000) tlocke    (1000)     1477 2014-03-11 14:07:20.000000 pg8000-1.9.8/README.creole
--rw-r--r--   0 tlocke    (1000) tlocke    (1000)     2073 2014-05-05 12:12:01.000000 pg8000-1.9.8/setup.py
-drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2014-05-05 12:35:25.000000 pg8000-1.9.8/pg8000/
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    73993 2014-05-05 12:10:20.000000 pg8000-1.9.8/pg8000/core.py
--rw-r--r--   0 tlocke    (1000) tlocke    (1000)     8913 2014-03-26 18:37:52.000000 pg8000-1.9.8/pg8000/__init__.py
--rw-r--r--   0 tlocke    (1000) tlocke    (1000)     3663 2013-12-05 16:15:07.000000 pg8000-1.9.8/pg8000/errors.py
--rw-r--r--   0 tlocke    (1000) tlocke    (1000)      440 2013-12-05 16:15:07.000000 pg8000-1.9.8/pg8000/util.py
--rw-r--r--   0 tlocke    (1000) tlocke    (1000)    20969 2014-01-25 15:16:22.000000 pg8000-1.9.8/pg8000/six.py
--rw-r--r--   0 tlocke    (1000) tlocke    (1000)     1635 2014-01-25 15:16:23.000000 pg8000-1.9.8/pg8000/types.py
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)     1845 2014-05-05 12:35:25.000000 pg8000-1.9.8/PKG-INFO
+drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2014-05-12 19:26:22.000000 pg8000-1.9.9/
+-rw-r--r--   0 tlocke    (1000) tlocke    (1000)     1477 2014-03-11 14:07:20.000000 pg8000-1.9.9/README.creole
+-rw-r--r--   0 tlocke    (1000) tlocke    (1000)     2073 2014-05-12 19:17:04.000000 pg8000-1.9.9/setup.py
+drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2014-05-12 19:26:22.000000 pg8000-1.9.9/pg8000/
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    75187 2014-05-11 20:59:52.000000 pg8000-1.9.9/pg8000/core.py
+-rw-r--r--   0 tlocke    (1000) tlocke    (1000)     8647 2014-05-07 20:29:20.000000 pg8000-1.9.9/pg8000/__init__.py
+-rw-r--r--   0 tlocke    (1000) tlocke    (1000)     3663 2013-12-05 16:15:07.000000 pg8000-1.9.9/pg8000/errors.py
+-rw-r--r--   0 tlocke    (1000) tlocke    (1000)      440 2013-12-05 16:15:07.000000 pg8000-1.9.9/pg8000/util.py
+-rw-r--r--   0 tlocke    (1000) tlocke    (1000)    20969 2014-01-25 15:16:22.000000 pg8000-1.9.9/pg8000/six.py
+-rw-r--r--   0 tlocke    (1000) tlocke    (1000)     1635 2014-05-07 20:30:30.000000 pg8000-1.9.9/pg8000/types.py
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)     1845 2014-05-12 19:26:22.000000 pg8000-1.9.9/PKG-INFO
```

### Comparing `pg8000-1.9.8/README.creole` & `pg8000-1.9.9/README.creole`

 * *Files identical despite different names*

### Comparing `pg8000-1.9.8/setup.py` & `pg8000-1.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 version 2.0.
 
 pg8000's name comes from the belief that it is probably about the 8000th \
 PostgreSQL interface for Python."""
 
 setup(
         name="pg8000",
-        version="1.9.8",
+        version="1.9.9",
         description="PostgreSQL interface library",
         long_description=long_description,
         author="Mathieu Fenniak",
         author_email="biziqe@mathieu.fenniak.net",
         url="https://github.com/mfenniak/pg8000",
         classifiers = [
             "Development Status :: 4 - Beta",
```

### Comparing `pg8000-1.9.8/pg8000/core.py` & `pg8000-1.9.9/pg8000/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,19 +238,19 @@
                     placeholders[-1] += c
             elif style == 'format':
                 state = OUTSIDE
 
         prev_c = c
 
     if style in ('numeric', 'qmark', 'format'):
-        def make_args(args):
-            return () if args is None else args
+        def make_args(vals):
+            return vals
     else:
-        def make_args(args):
-            return tuple(args[p] for p in placeholders)
+        def make_args(vals):
+            return tuple(vals[p] for p in placeholders)
 
     return ''.join(output_query), make_args
 
 
 def require_open_cursor(fn):
     def _fn(self, *args, **kwargs):
         if self._c is None:
@@ -337,28 +337,59 @@
 
 
 def timestamptz_recv_float(data, offset, length):
     return timestamp_recv_float(data, offset, length).replace(tzinfo=utc)
 
 
 def interval_send_integer(v):
-    return qii_pack(v.microseconds, v.days, v.months)
+    microseconds = v.microseconds
+    try:
+        microseconds += int(v.seconds * 1e6)
+    except AttributeError:
+        pass
+
+    try:
+        months = v.months
+    except AttributeError:
+        months = 0
+
+    return qii_pack(microseconds, v.days, months)
 
 
 def interval_send_float(v):
-    return dii_pack(v.microseconds / 1000.0 / 1000.0, v.days, v.months)
+    seconds = v.microseconds / 1000.0 / 1000.0
+    try:
+        seconds += v.seconds
+    except AttributeError:
+        pass
+
+    try:
+        months = v.months
+    except AttributeError:
+        months = 0
+
+    return dii_pack(seconds, v.days, months)
 
 
 def interval_recv_integer(data, offset, length):
-    return Interval(*qii_unpack(data, offset))
+    microseconds, days, months = qii_unpack(data, offset)
+    if months == 0:
+        seconds, micros = divmod(microseconds, 1e6)
+        return datetime.timedelta(days, seconds, micros)
+    else:
+        return Interval(microseconds, days, months)
 
 
 def interval_recv_float(data, offset, length):
     seconds, days, months = dii_unpack(data, offset)
-    return Interval(int(seconds * 1000 * 1000), days, months)
+    if months == 0:
+        secs, microseconds = divmod(seconds, 1e6)
+        return datetime.timedelta(days, secs, microseconds)
+    else:
+        return Interval(int(seconds * 1000 * 1000), days, months)
 
 
 def int8_recv(data, offset, length):
     return q_unpack(data, offset)[0]
 
 
 def int2_recv(data, offset, length):
@@ -497,14 +528,17 @@
 
     ##
     # Executes a database operation.  Parameters may be provided as a sequence
     # or mapping and will be bound to variables in the operation.
     # <p>
     # Stability: Part of the DBAPI 2.0 specification.
     def execute(self, operation, args=None, stream=None):
+        if args is None:
+            args = tuple()
+
         self._row_count = -1
         if not self._c.use_cache:
             self._c.statement_cache.clear()
 
         try:
             self._c.begin()
         except AttributeError:
@@ -560,21 +594,26 @@
             if table is None:
                 raise CopyQueryOrTableRequiredError()
             query = "COPY %s TO stdout DELIMITER '%s'" % (table, sep)
             if null is not None:
                 query += " NULL '%s'" % (null,)
         self.copy_execute(fileobj, query)
 
-    def _get_ps(self, operation, params):
-        key = (None if params is None else tuple(map(type, params))), operation
+    def _get_ps(self, operation, vals):
+        if pg8000.paramstyle in ('numeric', 'qmark', 'format'):
+            args = vals
+        else:
+            args = tuple(vals[k] for k in sorted(vals.keys()))
+
+        key = tuple(oid for oid, x, y in self._c.make_params(args)), operation
 
         try:
             return self._c.statement_cache[key]
         except KeyError:
-            ps = PreparedStatement(self._c, operation, params)
+            ps = PreparedStatement(self._c, operation, vals)
             self._c.statement_cache[key] = ps
             return ps
 
     @require_open_cursor
     def copy_execute(self, fileobj, query):
         self.execute(query, stream=fileobj)
 
@@ -1064,14 +1103,15 @@
             float: (701, FC_BINARY, d_pack),  # float8
             str: (705, FC_TEXT, text_out),  # unknown
             datetime.date: (1082, FC_TEXT, date_out),  # date
             datetime.time: (1083, FC_TEXT, time_out),  # time
             1114: (1114, FC_BINARY, timestamp_send_integer),  # timestamp
             # timestamp w/ tz
             1184: (1184, FC_BINARY, timestamptz_send_integer),
+            datetime.timedelta: (1186, FC_BINARY, interval_send_integer),
             Interval: (1186, FC_BINARY, interval_send_integer),
             Decimal: (1700, FC_TEXT, numeric_out),  # Decimal
             UUID: (2950, FC_BINARY, uuid_send),  # uuid
         }
 
         self.inspect_funcs = {
             datetime.datetime: self.inspect_datetime,
@@ -1153,17 +1193,17 @@
                 self.handle_messages()
             finally:
                 self._sock_lock.release()
         except:
             self.close()
             raise exc_info()[1]
 
-        self._begin = PreparedStatement(self, "BEGIN TRANSACTION")
-        self._commit = PreparedStatement(self, "COMMIT TRANSACTION")
-        self._rollback = PreparedStatement(self, "ROLLBACK TRANSACTION")
+        self._begin = PreparedStatement(self, "BEGIN TRANSACTION", ())
+        self._commit = PreparedStatement(self, "COMMIT TRANSACTION", ())
+        self._rollback = PreparedStatement(self, "ROLLBACK TRANSACTION", ())
         self.in_transaction = False
         self.notifies = []
         self.notifies_lock = threading.Lock()
 
     def handle_ERROR_RESPONSE(self, data, ps):
         msg_dict = data_into_dict(data)
         if msg_dict[RESPONSE_CODE] == "28000":
@@ -1286,23 +1326,23 @@
         # commit, but before the begin, it will be executed immediately
         # without a surrounding transaction.  Like all threading bugs -- it
         # sounds unlikely, until it happens every time in one
         # application...  however, to fix this, we need to lock the
         # database connection entirely, so that no cursors can execute
         # statements on other threads.  Support for that type of lock will
         # be done later.
-        self._commit.execute()
+        self._commit.execute(())
 
     ##
     # Rolls back the current database transaction.
     # <p>
     # Stability: Part of the DBAPI 2.0 specification.
     def rollback(self):
         # see bug description in commit.
-        self._rollback.execute()
+        self._rollback.execute(())
 
     ##
     # Closes the database connection.
     # <p>
     # Stability: Part of the DBAPI 2.0 specification.
     def close(self):
         try:
@@ -1323,15 +1363,15 @@
 
     ##
     # Begins a new transaction.
     # <p>
     # Stability: Added in v1.00, stability guaranteed for v1.xx.
     def begin(self):
         if not self.in_transaction and not self.autocommit:
-            self._begin.execute()
+            self._begin.execute(())
 
     def handle_AUTHENTICATION_REQUEST(self, data, ps):
         assert self._sock_lock.locked()
         # Int32 -   An authentication code that represents different
         #           authentication messages:
         #               0 = AuthenticationOk
         #               5 = MD5 pwd
@@ -1441,17 +1481,15 @@
             val = bytearray(ps.statement_name_bin)
             val.extend(statement.encode(self._client_encoding) + NULL_BYTE)
             val.extend(h_pack(len(ps.params)))
             for oid, fc, send_func in ps.params:
                 # Parse message doesn't seem to handle the -1 type_oid for NULL
                 # values that other messages handle.  So we'll provide type_oid
                 # 705, the PG "unknown" type.
-                if oid == -1:
-                    oid = 705
-                val.extend(i_pack(oid))
+                val.extend(i_pack(705 if oid == -1 else oid))
 
             # Byte1('D') - Identifies the message as a describe command.
             # Int32 - Message length, including self.
             # Byte1 - 'S' for prepared statement, 'P' for portal.
             # String - The name of the item to describe.
             self._send_message(PARSE, val)
             self._send_message(DESCRIBE, STATEMENT + ps.statement_name_bin)
@@ -1613,23 +1651,27 @@
 
                 self.py_types[1184] = (
                     1184, FC_BINARY, timestamptz_send_integer)
                 self.pg_types[1184] = (FC_BINARY, timestamptz_recv_integer)
 
                 self.py_types[Interval] = (
                     1186, FC_BINARY, interval_send_integer)
+                self.py_types[datetime.timedelta] = (
+                    1186, FC_BINARY, interval_send_integer)
                 self.pg_types[1186] = (FC_BINARY, interval_recv_integer)
             else:
                 self.py_types[1114] = (1114, FC_BINARY, timestamp_send_float)
                 self.pg_types[1114] = (FC_BINARY, timestamp_recv_float)
                 self.py_types[1184] = (1184, FC_BINARY, timestamptz_send_float)
                 self.pg_types[1184] = (FC_BINARY, timestamptz_recv_float)
 
                 self.py_types[Interval] = (
                     1186, FC_BINARY, interval_send_float)
+                self.py_types[datetime.timedelta] = (
+                    1186, FC_BINARY, interval_send_float)
                 self.pg_types[1186] = (FC_BINARY, interval_recv_float)
 
         elif key == b("server_version"):
             self._server_version = value.decode("ascii")
             if self._server_version.startswith("8"):
                 self._commands_with_count = (
                     b("INSERT"), b("DELETE"), b("UPDATE"), b("MOVE"),
@@ -1891,15 +1933,15 @@
     # automatically.
     # <p>
     # Stability: Added in v1.00, stability guaranteed for v1.xx.  It is
     # possible that implementation changes in the future could cause this
     # parameter to be ignored.
     row_cache_size = 100
 
-    def __init__(self, connection, query, values=None):
+    def __init__(self, connection, query, values):
 
         # Stability: Added in v1.03, stability guaranteed for v1.xx.
         self.row_count = -1
 
         self.c = connection
         self.portal_name = None
         self.row_cache_size_bin = i_pack(PreparedStatement.row_cache_size)
@@ -1963,15 +2005,15 @@
     def get_row_description(self):
         return self.row_desc
 
     ##
     # Run the SQL prepared statement with the given parameters.
     # <p>
     # Stability: Added in v1.00, stability guaranteed for v1.xx.
-    def execute(self, values=None, stream=None):
+    def execute(self, values, stream=None):
         try:
             self._lock.acquire()
             # cleanup last execute
             self._cached_rows.clear()
             self.row_count = -1
             self.portal_suspended = False
             try:
```

### Comparing `pg8000-1.9.8/pg8000/__init__.py` & `pg8000-1.9.9/pg8000/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,43 +219,27 @@
 # Construct an object holding binary data.
 def Binary(value):
     if PY2:
         return Bytea(value)
     else:
         return value
 
-try:
-    from pytz import utc
-except ImportError:
-    ZERO = datetime.timedelta(0)
-
-    class UTC(datetime.tzinfo):
-
-        def utcoffset(self, dt):
-            return ZERO
-
-        def tzname(self, dt):
-            return "UTC"
-
-        def dst(self, dt):
-            return ZERO
-    utc = UTC()
-
 
 # For compatibility with 1.8
 import pg8000 as dbapi
 DBAPI = dbapi
 pg8000_dbapi = DBAPI
+from pg8000.core import utc
 
 from pg8000.errors import (
     Warning, DatabaseError, InterfaceError,
     ProgrammingError, CopyQueryOrTableRequiredError, Error, OperationalError,
     IntegrityError, InternalError, NotSupportedError,
     ArrayContentNotHomogenousError, ArrayContentEmptyError,
     ArrayDimensionsNotConsistentError, ArrayContentNotSupportedError)
 
 __all__ = [
     Warning, Bytea, DatabaseError, connect, InterfaceError, ProgrammingError,
     CopyQueryOrTableRequiredError, Error, OperationalError, IntegrityError,
     InternalError, NotSupportedError, ArrayContentNotHomogenousError,
     ArrayContentEmptyError, ArrayDimensionsNotConsistentError,
-    ArrayContentNotSupportedError]
+    ArrayContentNotSupportedError, utc]
```

### Comparing `pg8000-1.9.8/pg8000/errors.py` & `pg8000-1.9.9/pg8000/errors.py`

 * *Files identical despite different names*

### Comparing `pg8000-1.9.8/pg8000/six.py` & `pg8000-1.9.9/pg8000/six.py`

 * *Files identical despite different names*

### Comparing `pg8000-1.9.8/pg8000/types.py` & `pg8000-1.9.9/pg8000/types.py`

 * *Files identical despite different names*

### Comparing `pg8000-1.9.8/PKG-INFO` & `pg8000-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pg8000
-Version: 1.9.8
+Version: 1.9.9
 Summary: PostgreSQL interface library
 Home-page: https://github.com/mfenniak/pg8000
 Author: Mathieu Fenniak
 Author-email: biziqe@mathieu.fenniak.net
 License: UNKNOWN
 Description: 
         pg8000
```


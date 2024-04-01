# Comparing `tmp/gtfs_station_stop-0.7.0b4.tar.gz` & `tmp/gtfs_station_stop-0.7.0b5.tar.gz`

## Comparing `gtfs_station_stop-0.7.0b4.tar` & `gtfs_station_stop-0.7.0b5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/.flake8
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/.gitlab-ci.yml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/requirements-dev.txt
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/requirements.txt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/setup.cfg
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/__init__.py
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/__main__.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/alert.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/arrival.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/calendar.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/const.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/feed_subject.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/helpers.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/route_info.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/route_status.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/static_database.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/station_stop.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/station_stop_info.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/trip_info.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/conftest.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/fixtures.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/mock_feed_server.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/test_arrival.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/test_calendar.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/test_feed_subject.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/test_helpers.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/test_route_info.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/test_route_status.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/test_station_stop.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/test_station_stop_info.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/test_trip_info.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/data/gtfs_static/calendar.txt
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/data/gtfs_static/calendar_dates.txt
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/data/gtfs_static/routes.txt
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/data/gtfs_static/stops.txt
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/data/gtfs_static/trips.txt
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/data/gtfs_static_supl/stops.txt
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/tests/data/gtfs_static_supl/trips.txt
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/LICENSE
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/README.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/pyproject.toml
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b4/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/.flake8
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/.gitlab-ci.yml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/requirements-dev.txt
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/requirements.txt
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/setup.cfg
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/__init__.py
+-rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/__main__.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/alert.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/arrival.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/calendar.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/const.py
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/feed_subject.py
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/helpers.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/route_info.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/route_status.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/static_database.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/station_stop.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/station_stop_info.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/trip_info.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/conftest.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/fixtures.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/mock_feed_server.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_arrival.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_calendar.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_feed_subject.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_helpers.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_route_info.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_route_status.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_station_stop.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_station_stop_info.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_trip_info.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static/calendar.txt
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static/calendar_dates.txt
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static/routes.txt
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static/stops.txt
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static/trips.txt
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static_supl/stops.txt
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static_supl/trips.txt
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/LICENSE
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/README.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/pyproject.toml
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/PKG-INFO
```

### Comparing `gtfs_station_stop-0.7.0b4/.gitlab-ci.yml` & `gtfs_station_stop-0.7.0b5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/.pre-commit-config.yaml` & `gtfs_station_stop-0.7.0b5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/setup.cfg` & `gtfs_station_stop-0.7.0b5/setup.cfg`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/__main__.py` & `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,48 +63,65 @@
     print(gtfs_station_stop.__about__.__version__)
     exit(0)
 
 start_time = time.time()
 
 # Get the API Key, argument takes precedent of environment variable
 api_key = args.api_key or os.environ.get("API_KEY")
+headers = {"api-key": api_key, "x-api-key": api_key, "api_key": api_key}
 
 ssi_db = None
 ti_db = None
 calendar = None
 
 if args.do_async and args.info_zip:
 
     async def async_get_static_info():
         async with asyncio.TaskGroup() as tg:
             ssi_db_task = tg.create_task(
-                async_factory(StationStopInfoDatabase, *args.info_zip)
+                async_factory(
+                    StationStopInfoDatabase,
+                    *args.info_zip,
+                    headers=headers,
+                )
+            )
+            ti_db_task = tg.create_task(
+                async_factory(
+                    TripInfoDatabase,
+                    *args.info_zip,
+                    headers=headers,
+                )
+            )
+            calendar_task = tg.create_task(
+                async_factory(
+                    Calendar,
+                    *args.info_zip,
+                    headers=headers,
+                )
             )
-            ti_db_task = tg.create_task(async_factory(TripInfoDatabase, *args.info_zip))
-            calendar_task = tg.create_task(async_factory(Calendar, *args.info_zip))
         return (ssi_db_task.result(), ti_db_task.result(), calendar_task.result())
 
     ssi_db, ti_db, calendar = asyncio.run(async_get_static_info())
 elif args.info_zip:
-    ssi_db = StationStopInfoDatabase(*args.info_zip)
-    ti_db = TripInfoDatabase(*args.info_zip)
-    calendar = Calendar(*args.info_zip)
+    ssi_db = StationStopInfoDatabase(*args.info_zip, headers=headers)
+    ti_db = TripInfoDatabase(*args.info_zip, headers=headers)
+    calendar = Calendar(*args.info_zip, headers=headers)
 
 if calendar is not None:
     # Print out the current active service IDs
     print()
     print("SERVICES:")
     print("=========")
     exptabs: int = max(len(v.service_id) + 2 for v in calendar.services.values())
     for s in calendar.get_active_services():
         print(f"{s.service_id}:\t\033[92m active \033[00m".expandtabs(exptabs))
     for s in calendar.get_inactive_services():
         print(f"{s.service_id}:\t\033[91m inactive \033[00m".expandtabs(exptabs))
 
-feed_subject = FeedSubject(args.feed_urls, api_key)
+feed_subject = FeedSubject(args.feed_urls, headers=headers)
 station_stops = [StationStop(id, feed_subject) for id in args.stops]
 route_statuses = [RouteStatus(id, feed_subject) for id in args.routes]
 
 if args.do_async:
     asyncio.run(feed_subject.async_update())
 else:
     station_stops = [StationStop(id, feed_subject) for id in args.stops]
```

### Comparing `gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/calendar.py` & `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 from datetime import date, datetime
 from typing import NamedTuple
 
-from gtfs_station_stop.helpers import gtfs_record_iter
 from gtfs_station_stop.static_database import GtfsStaticDatabase
 
 SERVICE_EXCEPTION_TYPE_ADDED = "1"
 SERVICE_EXCEPTION_TYPE_REMOVED = "2"
 
 
 class ServiceDays(NamedTuple):
@@ -49,20 +48,20 @@
         )
 
     def no_regular_service(service_id: str):
         return Service(service_id, ServiceDays.no_service(), date.min, date.min)
 
 
 class Calendar(GtfsStaticDatabase):
-    def __init__(self, *gtfs_files: os.PathLike):
+    def __init__(self, *gtfs_files: os.PathLike, **kwargs):
         self.services = {}
-        super().__init__(*gtfs_files)
+        super().__init__(*gtfs_files, **kwargs)
 
     def add_gtfs_data(self, zip_filelike):
-        for line in gtfs_record_iter(zip_filelike, "calendar.txt"):
+        for line in self._get_gtfs_record_iter(zip_filelike, "calendar.txt"):
             self.services[line["service_id"]] = Service(
                 line["service_id"],
                 ServiceDays(
                     line["monday"] == "1",
                     line["tuesday"] == "1",
                     line["wednesday"] == "1",
                     line["thursday"] == "1",
@@ -70,15 +69,15 @@
                     line["saturday"] == "1",
                     line["sunday"] == "1",
                 ),
                 datetime.strptime(line["start_date"], "%Y%m%d").date(),
                 datetime.strptime(line["end_date"], "%Y%m%d").date(),
             )
         # Add in special services
-        for line in gtfs_record_iter(zip_filelike, "calendar_dates.txt"):
+        for line in self._get_gtfs_record_iter(zip_filelike, "calendar_dates.txt"):
             service_id = line["service_id"]
             if self.services.get(service_id) is None:
                 # Create a blank calendar if it is missing
                 self.services[service_id] = Service.no_regular_service(service_id)
             if line["exception_type"] == SERVICE_EXCEPTION_TYPE_ADDED:
                 self.services[service_id].added_exceptions.add(
                     datetime.strptime(line["date"], "%Y%m%d").date()
```

### Comparing `gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/feed_subject.py` & `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/feed_subject.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
 class RouteStatus:
     # implemented in route_status.py
     pass
 
 
 class FeedSubject:
-    def __init__(self, realtime_feed_uris: Sequence[str], api_key: str = ""):
+    def __init__(self, realtime_feed_uris: Sequence[str], **kwargs):
         self.realtime_feed_uris = set(realtime_feed_uris)
-        self.api_key = api_key
+        self.kwargs = kwargs
         self.subscribers = defaultdict(WeakSet)
 
     def _request_gtfs_feed(self, uri: str) -> bytes:
         req: requests.Response = requests.get(
-            url=uri, headers={"x-api-key": self.api_key}
+            url=uri, headers=self.kwargs.get("headers")
         )
         if req.status_code <= 200 and req.status_code < 300:
             return req.content
-        raise RuntimeError(f"HTTP error code {req.status_code}")
+        raise RuntimeError(f"HTTP error code {req.status_code}, {req.text}")
 
     def _get_gtfs_feed(self) -> gtfs_realtime_pb2.FeedMessage:
         def load_feed_data(_subject, _uri):
             uri_feed = gtfs_realtime_pb2.FeedMessage()
             uri_feed.ParseFromString(_subject._request_gtfs_feed(_uri))
             return uri_feed
 
@@ -55,18 +55,22 @@
             ]
             for fut in concurrent.futures.as_completed(futs):
                 feed.MergeFrom(fut.result())
 
         return feed
 
     async def _async_request_gtfs_feed(self, uri: str) -> bytes:
-        async with aiohttp.ClientSession() as session:
+        async with aiohttp.ClientSession(headers=self.kwargs.get("headers")) as session:
             async with session.get(uri) as req:
                 if req.status <= 200 and req.status < 300:
                     return await req.read()
+                else:
+                    raise RuntimeError(
+                        f"HTTP error code {req.status}, {await req.text()}"
+                    )
 
     async def _async_get_gtfs_feed(self) -> gtfs_realtime_pb2.FeedMessage:
         async def async_merge_feed(
             merge_into_feed: gtfs_realtime_pb2.FeedMessage,
             merge_from_feed: gtfs_realtime_pb2.FeedMessage,
         ):
             merge_into_feed.MergeFrom(merge_from_feed)
```

### Comparing `gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/helpers.py` & `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,38 +41,43 @@
     try:
         result = urlparse(url)
         return all([result.scheme, result.netloc])
     except (ValueError, AttributeError):
         return False
 
 
-def gtfs_record_iter(zip_filelike, target_txt: os.PathLike):
+def gtfs_record_iter(zip_filelike, target_txt: os.PathLike, **kwargs):
     """Generates a line from a given GTFS table. Can handle local files or URLs."""
 
     zip_data = zip_filelike
     # If the data is a url, make the request for the file resource.
     if is_url(zip_filelike):
         # Make the request, check for good return code, and convert to IO object.
         # As GTFS Static Data updates rarely, (most providers recommend pulling this once per day),
         # we will use a cache to minimize unnecessary checks.
         session = requests_cache.CachedSession(
-            GTFS_STATIC_CACHE, expire_after=GTFS_STATIC_CACHE_EXPIRY
+            GTFS_STATIC_CACHE,
+            expire_after=GTFS_STATIC_CACHE_EXPIRY,
         )
-        res = session.get(zip_filelike)
+        res = session.get(zip_filelike, headers=kwargs.get("headers"))
         if 200 <= res.status_code < 400:
             zip_data = BytesIO(res.content)
+        else:
+            raise ConnectionRefusedError
 
     with ZipFile(zip_data, "r") as zip:
         # Find the stops.txt file
         first_or_none: str = next(
             (name for name in zip.namelist() if name == target_txt), None
         )
         if first_or_none is None:
             raise RuntimeError(f"Did not find required {target_txt} file")
         # Create the dictionary of IDs, parents should precede the children
-        with StringIO(str(zip.read(first_or_none), encoding="ASCII")) as stops_dot_txt:
+        with StringIO(
+            str(zip.read(first_or_none), encoding="utf-8-sig")
+        ) as stops_dot_txt:
             reader = csv.DictReader(
                 stops_dot_txt,
                 delimiter=",",
             )
             for line in reader:
                 yield line
```

### Comparing `gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/route_status.py` & `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/route_status.py`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/static_database.py` & `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/static_database.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 import os
 from io import BytesIO
 
 from aiohttp_client_cache import CachedSession, SQLiteBackend
 
 from gtfs_station_stop.const import GTFS_STATIC_CACHE, GTFS_STATIC_CACHE_EXPIRY
+from gtfs_station_stop.helpers import gtfs_record_iter
 
 
 class GtfsStaticDatabase:
-    def __init__(self, *gtfs_files: os.PathLike):
+    def __init__(self, *gtfs_files: os.PathLike, **kwargs):
+        self.kwargs = kwargs
         for file in gtfs_files:
             self.add_gtfs_data(file)
 
+    def _get_gtfs_record_iter(self, zip_filelike, target_txt: os.PathLike):
+        return gtfs_record_iter(zip_filelike, target_txt, **self.kwargs)
+
     def add_gtfs_data(self, gtfs_pathlike: os.PathLike):
         raise NotImplementedError
 
 
 async def async_factory(
     gtfs_class: GtfsStaticDatabase,
     *gtfs_urls: os.PathLike,
     **kwargs,
 ):
     gtfs_db = gtfs_class()
-    for url in gtfs_urls:
-        async with CachedSession(
-            cache=SQLiteBackend(
-                kwargs.get("gtfs_static_cache", GTFS_STATIC_CACHE),
-                expire_after=kwargs.get("expire_after", GTFS_STATIC_CACHE_EXPIRY),
-            )
-        ) as session:
+    async with CachedSession(
+        cache=SQLiteBackend(
+            kwargs.get("gtfs_static_cache", GTFS_STATIC_CACHE),
+            expire_after=kwargs.get("expire_after", GTFS_STATIC_CACHE_EXPIRY),
+        ),
+        headers=kwargs.get("headers"),
+    ) as session:
+        for url in gtfs_urls:
             async with session.get(url) as response:
-                zip_data = BytesIO(await response.read())
-                gtfs_db.add_gtfs_data(zip_data)
+                if 200 <= response.status < 400:
+                    zip_data = BytesIO(await response.read())
+                    gtfs_db.add_gtfs_data(zip_data)
+                else:
+                    raise RuntimeError(
+                        f"HTTP error code {response.status}, {await response.text()}"
+                    )
     return gtfs_db
```

### Comparing `gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/station_stop.py` & `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/station_stop.py`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/src/gtfs_station_stop/trip_info.py` & `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/trip_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import os
 from collections.abc import Iterable
 from datetime import date, datetime
 from typing import Any
 
 from gtfs_station_stop.calendar import Calendar
-from gtfs_station_stop.helpers import gtfs_record_iter
 from gtfs_station_stop.static_database import GtfsStaticDatabase
 
 
 class TripInfo:
     def __init__(self, trip_data_dict: dict):
         self.route_id = trip_data_dict["route_id"]
         self.trip_id = trip_data_dict["trip_id"]
         self.service_id = trip_data_dict["service_id"]
-        self.trip_headsign = trip_data_dict["trip_headsign"]
-        self.direction_id = trip_data_dict["direction_id"]
-        self.shape_id = trip_data_dict["shape_id"]
+        self.trip_headsign = trip_data_dict.get("trip_headsign", "")
+        self.trip_short_name = trip_data_dict.get("trip_short_name", "")
+        self.direction_id = trip_data_dict.get("direction_id")
+        self.shape_id = trip_data_dict.get("shape_id")
 
     def __repr__(self):
         return f"{self.trip_id}: {self.route_id} to {self.trip_headsign}"
 
 
 class TripInfoDatabase(GtfsStaticDatabase):
-    def __init__(self, *gtfs_files: os.PathLike):
+    def __init__(self, *gtfs_files: os.PathLike, **kwargs):
         self.trip_infos = {}
         self.__cached_route_ids = None
-        super().__init__(*gtfs_files)
+        super().__init__(*gtfs_files, **kwargs)
 
     def add_gtfs_data(self, zip_filepath: os.PathLike):
-        for line in gtfs_record_iter(zip_filepath, "trips.txt"):
+        for line in self._get_gtfs_record_iter(zip_filepath, "trips.txt"):
             id = line["trip_id"]
             self.trip_infos[id] = TripInfo(line)
         # invalidate the cache
         self.__cached_route_ids = None
 
     def get_close_match(
         self,
```

### Comparing `gtfs_station_stop-0.7.0b4/tests/conftest.py` & `gtfs_station_stop-0.7.0b5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/tests/fixtures.py` & `gtfs_station_stop-0.7.0b5/tests/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-l",
         "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs",
         "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/camsys%2Fsubway-alerts",
     ]
     dotenv.load_dotenv()
     return FeedSubject(
         feed_urls,
-        os.environ.get("API_KEY"),
+        headers={"x-api-key": os.environ.get("API_KEY")},
     )
 
 
 @pytest.fixture
 def feed_subject(mock_feed_subject, nyct_feed_subject):
     # Set the feed server to use either mock data read from the tests/data directory, or to use real data
     # By default, use mock data
```

### Comparing `gtfs_station_stop-0.7.0b4/tests/mock_feed_server.py` & `gtfs_station_stop-0.7.0b5/tests/mock_feed_server.py`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/tests/test_calendar.py` & `gtfs_station_stop-0.7.0b5/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/tests/test_helpers.py` & `gtfs_station_stop-0.7.0b5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/tests/test_route_status.py` & `gtfs_station_stop-0.7.0b5/tests/test_route_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from gtfs_station_stop.feed_subject import FeedSubject
 from gtfs_station_stop.route_status import RouteStatus
 
 
 def test_create_route_status():
-    rs = RouteStatus("Z", FeedSubject("", []))
+    rs = RouteStatus("Z", FeedSubject([]))
     assert hasattr(rs, "alerts")
 
 
 def test_subscribe_to_feed(feed_subject):
     rs = RouteStatus("Z", feed_subject)
     assert len(feed_subject.subscribers) == 1
     del rs
```

### Comparing `gtfs_station_stop-0.7.0b4/tests/test_station_stop.py` & `gtfs_station_stop-0.7.0b5/tests/test_station_stop.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from freezegun import freeze_time
 
 from gtfs_station_stop.feed_subject import FeedSubject
 from gtfs_station_stop.station_stop import StationStop
 
 
 def test_create_station_stop():
-    ss = StationStop("L20N", FeedSubject("", []))
+    ss = StationStop("L20N", FeedSubject([]))
     assert hasattr(ss, "alerts")
     assert hasattr(ss, "arrivals")
 
 
 def test_subscribe_to_feed(feed_subject):
     ss = StationStop("L20N", feed_subject)
     assert len(feed_subject.subscribers) == 1
```

### Comparing `gtfs_station_stop-0.7.0b4/tests/test_station_stop_info.py` & `gtfs_station_stop-0.7.0b5/tests/test_station_stop_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     ssi = await async_factory(
         StationStopInfoDatabase,
         *[
             url
             for url in mock_feed_server.static_urls
             if url.endswith("gtfs_static.zip")
         ],
+        headers={"api-key": "TEST_KEY"},
     )
     assert ssi["101"].name == "Test Station Main St"
     assert ssi["101N"].name == "Test Station Main St"
     assert ssi["102S"].parent == ssi["102"]
 
 
 def test_get_stop_ids(good_station_stop_info_db):
```

### Comparing `gtfs_station_stop-0.7.0b4/tests/test_trip_info.py` & `gtfs_station_stop-0.7.0b5/tests/test_trip_info.py`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/tests/data/gtfs_static/trips.txt` & `gtfs_station_stop-0.7.0b5/tests/data/gtfs_static/trips.txt`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/.gitignore` & `gtfs_station_stop-0.7.0b5/.gitignore`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/LICENSE` & `gtfs_station_stop-0.7.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/README.md` & `gtfs_station_stop-0.7.0b5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # GTFS Station Stop
 
 A project for organizing GTFS Real-Time data for use as a homeassistant sensor.
 
 ## Usage
 
-This is designed for use with Home Assistant GTFS Realtime Custom Component.
+This is designed for use with [Home Assistant GTFS Realtime Custom Component](https://github.com/bcpearce/homeassistant-gtfs-realtime).
+
+It can also be used for general GTFS update purposes.
 
 ### Feed Subjects and Station Stops
 
 All updates go through the Feed Subject which is setup to call updates from one or more feed URLS.
 
 Create a feed subject like so, then pass it in the constructor for a Station Stop
 
@@ -60,28 +62,40 @@
 ```python
 from gtfs_station_stop.station_stop_info import StationStopInfoDatabase
 
 station_stop_info_db = StationStopInfoDatabase("gtfs_static.zip")
 print(f"{station_stop_info_db['STOP_ID']}")
 ```
 
+Static info can be queried through the `station_stop_info`, `route_info`, `calendar`, and `trip_info` submodules.
+
+GTFS providers will regularly update their static feeds.  In order to account for this, the library will attempt to cache zip file downloads for static info.
+
 ### Async Updates
 
 Asynchronous updates are also supported through the `async_update()` method.
 
 ```python
 await feed_subject.async_update()
 ```
 
-Static data can also be obtained similarly with `gtfs_station_stop.helpers.async_get_gtfs_database`.
+Static data can also be obtained similarly with `gtfs_station_stop.static_database.async_factory`.
 
 ```python
 station_stop_info_database = await async_get_gtfs_database(StationStopInfoDatabase, "https://gtfsprovider.example.com/static.zip")
 ```
 
+### Command Line Interface
+
+This can be run as a Python module on the command line using
+
+`python -m gtfs_station_stop`
+
+Use `python -m gtfs_station_stop --help` for details.
+
 ## Development Setup
 
 Install all development dependencies with:
 
 ```bash
 $ pip install -r requirements-dev.txt
 ```
```

### Comparing `gtfs_station_stop-0.7.0b4/pyproject.toml` & `gtfs_station_stop-0.7.0b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gtfs_station_stop-0.7.0b4/PKG-INFO` & `gtfs_station_stop-0.7.0b5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gtfs_station_stop
-Version: 0.7.0b4
+Version: 0.7.0b5
 Summary: Package for reading and organizing GTFS data for a given station stop.
 Author-email: Benjamin Pearce <gtfs@bcpearce.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -18,15 +18,17 @@
 
 # GTFS Station Stop
 
 A project for organizing GTFS Real-Time data for use as a homeassistant sensor.
 
 ## Usage
 
-This is designed for use with Home Assistant GTFS Realtime Custom Component.
+This is designed for use with [Home Assistant GTFS Realtime Custom Component](https://github.com/bcpearce/homeassistant-gtfs-realtime).
+
+It can also be used for general GTFS update purposes.
 
 ### Feed Subjects and Station Stops
 
 All updates go through the Feed Subject which is setup to call updates from one or more feed URLS.
 
 Create a feed subject like so, then pass it in the constructor for a Station Stop
 
@@ -78,28 +80,40 @@
 ```python
 from gtfs_station_stop.station_stop_info import StationStopInfoDatabase
 
 station_stop_info_db = StationStopInfoDatabase("gtfs_static.zip")
 print(f"{station_stop_info_db['STOP_ID']}")
 ```
 
+Static info can be queried through the `station_stop_info`, `route_info`, `calendar`, and `trip_info` submodules.
+
+GTFS providers will regularly update their static feeds.  In order to account for this, the library will attempt to cache zip file downloads for static info.
+
 ### Async Updates
 
 Asynchronous updates are also supported through the `async_update()` method.
 
 ```python
 await feed_subject.async_update()
 ```
 
-Static data can also be obtained similarly with `gtfs_station_stop.helpers.async_get_gtfs_database`.
+Static data can also be obtained similarly with `gtfs_station_stop.static_database.async_factory`.
 
 ```python
 station_stop_info_database = await async_get_gtfs_database(StationStopInfoDatabase, "https://gtfsprovider.example.com/static.zip")
 ```
 
+### Command Line Interface
+
+This can be run as a Python module on the command line using
+
+`python -m gtfs_station_stop`
+
+Use `python -m gtfs_station_stop --help` for details.
+
 ## Development Setup
 
 Install all development dependencies with:
 
 ```bash
 $ pip install -r requirements-dev.txt
 ```
```


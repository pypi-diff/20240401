# Comparing `tmp/edx-search-3.8.2.tar.gz` & `tmp/edx-search-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-search-3.8.2.tar", last modified: Tue Jan  9 21:49:52 2024, max compression
+gzip compressed data, was "edx-search-3.9.1.tar", last modified: Mon Apr  1 18:53:57 2024, max compression
```

## Comparing `edx-search-3.8.2.tar` & `edx-search-3.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 21:49:52.148999 edx-search-3.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-09 21:49:47.000000 edx-search-3.8.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    35135 2024-01-09 21:49:47.000000 edx-search-3.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-09 21:49:47.000000 edx-search-3.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-09 21:49:52.148999 edx-search-3.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12575 2024-01-09 21:49:47.000000 edx-search-3.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 21:49:52.144999 edx-search-3.8.2/edx_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-09 21:49:52.000000 edx-search-3.8.2/edx_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-09 21:49:52.000000 edx-search-3.8.2/edx_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 21:49:52.000000 edx-search-3.8.2/edx_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-09 21:49:52.000000 edx-search-3.8.2/edx_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-09 21:49:52.000000 edx-search-3.8.2/edx_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 21:49:52.148999 edx-search-3.8.2/edxsearch/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-09 21:49:47.000000 edx-search-3.8.2/edxsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-01-09 21:49:47.000000 edx-search-3.8.2/edxsearch/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-09 21:49:47.000000 edx-search-3.8.2/edxsearch/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-01-09 21:49:47.000000 edx-search-3.8.2/edxsearch/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 21:49:52.148999 edx-search-3.8.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-01-09 21:49:47.000000 edx-search-3.8.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-09 21:49:47.000000 edx-search-3.8.2/requirements/testing.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 21:49:52.148999 edx-search-3.8.2/search/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22940 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/filter_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/result_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/search_engine_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 21:49:52.148999 edx-search-3.8.2/search/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/tests/mock_search_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/tests/test_api_timing_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/tests/test_course_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/tests/test_course_discovery_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/tests/test_engines.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/tests/test_mock_search_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/tests/test_search_result_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20485 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    36990 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-01-09 21:49:47.000000 edx-search-3.8.2/search/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 21:49:52.148999 edx-search-3.8.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2546 2024-01-09 21:49:47.000000 edx-search-3.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:53:57.618677 edx-search-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 18:53:53.000000 edx-search-3.9.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    35135 2024-04-01 18:53:53.000000 edx-search-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-01 18:53:53.000000 edx-search-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-04-01 18:53:57.618677 edx-search-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12575 2024-04-01 18:53:53.000000 edx-search-3.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:53:57.614677 edx-search-3.9.1/edx_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-04-01 18:53:57.000000 edx-search-3.9.1/edx_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-01 18:53:57.000000 edx-search-3.9.1/edx_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:53:57.000000 edx-search-3.9.1/edx_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 18:53:57.000000 edx-search-3.9.1/edx_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-01 18:53:57.000000 edx-search-3.9.1/edx_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:53:57.614677 edx-search-3.9.1/edxsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 18:53:53.000000 edx-search-3.9.1/edxsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-01 18:53:53.000000 edx-search-3.9.1/edxsearch/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-01 18:53:53.000000 edx-search-3.9.1/edxsearch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-01 18:53:53.000000 edx-search-3.9.1/edxsearch/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:53:57.614677 edx-search-3.9.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-01 18:53:53.000000 edx-search-3.9.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-01 18:53:53.000000 edx-search-3.9.1/requirements/testing.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:53:57.614677 edx-search-3.9.1/search/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22944 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/filter_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/result_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/search_engine_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:53:57.614677 edx-search-3.9.1/search/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/tests/mock_search_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/tests/test_api_timing_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15658 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/tests/test_course_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/tests/test_course_discovery_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/tests/test_engines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/tests/test_mock_search_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/tests/test_search_result_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20303 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36782 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6825 2024-04-01 18:53:53.000000 edx-search-3.9.1/search/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:53:57.618677 edx-search-3.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2802 2024-04-01 18:53:53.000000 edx-search-3.9.1/setup.py
```

### Comparing `edx-search-3.8.2/LICENSE` & `edx-search-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-search-3.8.2/README.md` & `edx-search-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `edx-search-3.8.2/edx_search.egg-info/SOURCES.txt` & `edx-search-3.9.1/edx_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-search-3.8.2/edxsearch/settings.py` & `edx-search-3.9.1/edxsearch/settings.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.8.2/requirements/base.in` & `edx-search-3.9.1/requirements/base.in`

 * *Files identical despite different names*

### Comparing `edx-search-3.8.2/search/api.py` & `edx-search-3.9.1/search/api.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.8.2/search/elastic.py` & `edx-search-3.9.1/search/elastic.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,24 +465,25 @@
         except BulkIndexError as ex:
             valid_errors = [error for error in ex.errors if error["delete"]["status"] != 404]
 
             if valid_errors:
                 log.exception("An error occurred while removing documents from the index: %r", valid_errors)
                 raise
 
+    # pylint: disable=arguments-renamed, unused-argument
     def search(self,
                query_string=None,
                field_dictionary=None,
                filter_dictionary=None,
                exclude_dictionary=None,
                aggregation_terms=None,
                exclude_ids=None,
                use_field_match=False,
                log_search_params=False,
-               **kwargs):  # pylint: disable=arguments-differ, unused-argument
+               **kwargs):
         """
         Implements call to search the index for the desired content.
 
         Args:
             query_string (str): the string of values upon which to search within the
             content of the objects within the index
```

### Comparing `edx-search-3.8.2/search/filter_generator.py` & `edx-search-3.9.1/search/filter_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 class SearchFilterGenerator:
 
     """
     Class to provide a set of filters for the search.
     Users of this search app will override this class and update setting for SEARCH_FILTER_GENERATOR
     """
 
-    # disabling pylint violations because overriders will want to use these
-    # pylint: disable=unused-argument, no-self-use
     def filter_dictionary(self, **kwargs):
         """ base implementation which filters via start_date """
         return {"start_date": DateRange(None, datetime.utcnow())}
 
     def field_dictionary(self, **kwargs):
         """ base implementation which add course if provided """
         field_dictionary = {}
```

### Comparing `edx-search-3.8.2/search/initializer.py` & `edx-search-3.9.1/search/initializer.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 class SearchInitializer:
 
     """
     Class to set starting environment parameters for search app.
     Users of this search app will override this class and update setting for SEARCH_INITIALIZER
     """
 
-    # disabling pylint violations because overriders will want to use these
-    # pylint: disable=unused-argument, no-self-use
     def initialize(self, **kwargs):
         """ empty base implementation """
 
     @classmethod
     def set_search_enviroment(cls, **kwargs):
         """
         Called from within search handler
```

### Comparing `edx-search-3.8.2/search/result_processor.py` & `edx-search-3.9.1/search/result_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from .utils import _load_class
 
 DESIRED_EXCERPT_LENGTH = 100
 ELLIPSIS = '<span class="search-results-ellipsis"></span>'
 
 # log appears to be standard name used for logger
-log = logging.getLogger(__name__)  # pylint: disable=invalid-name
+log = logging.getLogger(__name__)
 
 
 class SearchResultProcessor:
 
     """
     Class to post-process a search result from the search.
     Each @property defined herein will be exposed as a member in the json-results given to the end user
@@ -83,16 +83,15 @@
         for matched_string in {match.group() for match in matches}:
             match_in = match_in.replace(
                 matched_string,
                 getattr(settings, "SEARCH_MATCH_DECORATION", "<b>{}</b>").format(matched_string)
             )
         return match_in
 
-    # disabling pylint violations because overriders will want to use these
-    def should_remove(self, user):  # pylint: disable=unused-argument, no-self-use
+    def should_remove(self, user):  # pylint: disable=unused-argument
         """
         Override this in a class in order to add in last-chance access checks to the search process
         Your application will want to make this decision
         """
         return False
 
     def add_properties(self):
@@ -112,15 +111,15 @@
         result_processor = _load_class(getattr(settings, "SEARCH_RESULT_PROCESSOR", None), cls)
         srp = result_processor(dictionary, match_phrase)
         if srp.should_remove(user):
             return None
         try:
             srp.add_properties()
         # protect around any problems introduced by subclasses within their properties
-        except Exception as ex:  # pylint: disable=broad-except
+        except Exception as ex:
             log.exception("error processing properties for %s - %s: will remove from results",
                           json.dumps(dictionary, cls=DjangoJSONEncoder), str(ex))
             return None
         return dictionary
 
     @property
     def excerpt(self):
```

### Comparing `edx-search-3.8.2/search/search_engine_base.py` & `edx-search-3.9.1/search/search_engine_base.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.8.2/search/tests/mock_search_engine.py` & `edx-search-3.9.1/search/tests/mock_search_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
                     add_agg_value(individual_value)
             else:
                 terms[agg_value] += 1
 
         for document in aggregated_documents:
             add_agg_value(document[aggregate])
 
-        total = sum([terms[term] for term in terms])
+        total = sum([terms[term] for term in terms])    # pylint: disable=consider-using-generator
 
         return total, terms
 
     for agg in aggregation_terms:
         total, terms = process_aggregation(agg)
         aggregations[agg] = {
             "total": total,
```

### Comparing `edx-search-3.8.2/search/tests/test_api_timing_events.py` & `edx-search-3.9.1/search/tests/test_api_timing_events.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.8.2/search/tests/test_course_discovery.py` & `edx-search-3.9.1/search/tests/test_course_discovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python
 # Some of the subclasses that get used as settings-overrides will yield this pylint
 # error, but they do get used when included as part of the override_settings
-# pylint: disable=too-few-public-methods
-# pylint: disable=too-many-ancestors
 """ Tests for search functionalty """
 
 import copy
 from datetime import datetime
 import ddt
 
 from django.core.cache import cache
@@ -80,15 +78,15 @@
     "enrollment_start": {"type": "date"},
     "enrollment_end": {"type": "date"}
 })
 @override_settings(MOCK_SEARCH_BACKING_FILE=None)
 @override_settings(COURSEWARE_CONTENT_INDEX_NAME=TEST_INDEX_NAME)
 @override_settings(COURSEWARE_INFO_INDEX_NAME=TEST_INDEX_NAME)
 # Any class that inherits from TestCase will cause too-many-public-methods pylint error
-class TestMockCourseDiscoverySearch(TestCase, SearcherMixin):  # pylint: disable=too-many-public-methods
+class TestMockCourseDiscoverySearch(TestCase, SearcherMixin):
     """
     Tests course discovery activities
     """
 
     @property
     def _is_elastic(self):
         """ check search engine implementation, to manage cleanup differently """
```

### Comparing `edx-search-3.8.2/search/tests/test_course_discovery_views.py` & `edx-search-3.9.1/search/tests/test_course_discovery_views.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,16 @@
 from django.test.utils import override_settings
 
 from search.tests.tests import TEST_INDEX_NAME
 from search.tests.utils import post_discovery_request
 from .test_views import MockSearchUrlTest
 from .test_course_discovery import DemoCourse
 
-# Any class that inherits from TestCase will cause too-many-public-methods pylint error
-# pylint: disable=too-many-public-methods
 
-
-@override_settings(ELASTIC_FIELD_MAPPINGS={  # pylint: disable=too-many-ancestors
+@override_settings(ELASTIC_FIELD_MAPPINGS={
     "start_date": {"type": "date"},
     "enrollment_start": {"type": "date"},
     "enrollment_end": {"type": "date"}
 })
 @override_settings(SEARCH_ENGINE="search.tests.mock_search_engine.MockSearchEngine")
 @override_settings(COURSEWARE_CONTENT_INDEX_NAME=TEST_INDEX_NAME)
 @override_settings(COURSEWARE_INFO_INDEX_NAME=TEST_INDEX_NAME)
```

### Comparing `edx-search-3.8.2/search/tests/test_engines.py` & `edx-search-3.9.1/search/tests/test_engines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 # Some of the subclasses that get used as settings-overrides will yield this pylint
 # error, but they do get used when included as part of the override_settings
-# pylint: disable=too-few-public-methods
 """ Tests for search functionality """
 
 import json
 import os
 from datetime import datetime
 from unittest.mock import patch
```

### Comparing `edx-search-3.8.2/search/tests/test_mock_search_engine.py` & `edx-search-3.9.1/search/tests/test_mock_search_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,14 @@
 from django.test.utils import override_settings
 
 from search.tests.mock_search_engine import _find_field, _filter_intersection, json_date_to_datetime
 from search.tests.utils import SearcherMixin
 from search.utils import DateRange
 
 
-# Any class that inherits from TestCase will cause too-many-public-methods pylint error
-# pylint: disable=too-many-public-methods
-
-
 @override_settings(SEARCH_ENGINE="search.tests.mock_search_engine.MockSearchEngine")
 @override_settings(ELASTIC_FIELD_MAPPINGS={"start_date": {"type": "date"}})
 class MockSpecificSearchTests(TestCase, SearcherMixin):
     """ For testing pieces of the Mock Engine that have no equivalent in Elastic """
 
     def test_find_field_arguments(self):
         """ test that field argument validity is observed """
```

### Comparing `edx-search-3.8.2/search/tests/test_search_result_processor.py` & `edx-search-3.9.1/search/tests/test_search_result_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import ddt
 
 from django.test import TestCase
 from django.test.utils import override_settings
 from search.result_processor import SearchResultProcessor, ELLIPSIS
 
 
-# Any class that inherits from TestCase will cause too-many-public-methods pylint error
-# pylint: disable=too-many-public-methods
 @ddt.ddt
 class SearchResultProcessorTests(TestCase):
     """ Tests to check SearchResultProcessor is working as desired """
 
     def test_strings_in_dictionary(self):
         """ Test finding strings within dictionary item """
         test_dict = {
@@ -293,15 +291,14 @@
 
 
 class TestSearchResultProcessor(SearchResultProcessor):
     """
     Override the SearchResultProcessor so that we get the additional (inferred) properties
     and can identify results that should be removed due to access restriction
     """
-    # pylint: disable=no-self-use
     @property
     def additional_property(self):
         """ additional property that should appear within processed results """
         return "Should have an extra value"
 
     @property
     def url(self):
```

### Comparing `edx-search-3.8.2/search/tests/test_views.py` & `edx-search-3.9.1/search/tests/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from search.search_engine_base import DEFAULT_ELASTIC_SEARCH_SWITCH
 from search.elastic import ElasticSearchEngine
 from search.tests.mock_search_engine import MockSearchEngine
 from search.tests.utils import post_request, SearcherMixin, TEST_INDEX_NAME
 
 
 # Any class that inherits from TestCase will cause too-many-public-methods pylint error
-# pylint: disable=too-many-public-methods
 @override_settings(SEARCH_ENGINE="search.tests.mock_search_engine.MockSearchEngine")
 @override_settings(ELASTIC_FIELD_MAPPINGS={"start_date": {"type": "date"}})
 @override_settings(COURSEWARE_CONTENT_INDEX_NAME=TEST_INDEX_NAME)
 @override_settings(COURSEWARE_INFO_INDEX_NAME=TEST_INDEX_NAME)
 class MockSearchUrlTest(TestCase, SearcherMixin):
     """
     Make sure that requests to the url get routed to the correct view handler
@@ -42,40 +41,40 @@
     def tearDown(self):
         MockSearchEngine.destroy()
         self._searcher = None
         super().tearDown()
 
     def assert_no_events_were_emitted(self):
         """Ensures no events were emitted since the last event related assertion"""
-        self.assertFalse(self.mock_tracker.emit.called)  # pylint: disable=maybe-no-member
+        self.assertFalse(self.mock_tracker.emit.called)
 
     def assert_search_initiated_event(self, search_term, size, page):
         """Ensures an search initiated event was emitted"""
-        initiated_search_call = self.mock_tracker.emit.mock_calls[0]  # pylint: disable=maybe-no-member
+        initiated_search_call = self.mock_tracker.emit.mock_calls[0]
         expected_result = call('edx.course.search.initiated', {
             "search_term": str(search_term),
             "page_size": size,
             "page_number": page,
         })
         self.assertEqual(expected_result, initiated_search_call)
 
     def assert_results_returned_event(self, search_term, size, page, total):
         """Ensures an results returned event was emitted"""
-        returned_results_call = self.mock_tracker.emit.mock_calls[1]  # pylint: disable=maybe-no-member
+        returned_results_call = self.mock_tracker.emit.mock_calls[1]
         expected_result = call('edx.course.search.results_displayed', {
             "search_term": str(search_term),
             "page_size": size,
             "page_number": page,
             "results_count": total,
         })
         self.assertEqual(expected_result, returned_results_call)
 
     def assert_initiated_return_events(self, search_term, size, page, total):
         """Asserts search initiated and results returned events were emitted"""
-        self.assertEqual(self.mock_tracker.emit.call_count, 2)  # pylint: disable=maybe-no-member
+        self.assertEqual(self.mock_tracker.emit.call_count, 2)
         self.assert_search_initiated_event(search_term, size, page)
         self.assert_results_returned_event(search_term, size, page, total)
 
     def test_url_resolution(self):
         """ make sure that the url is resolved as expected """
         resolver = resolve('/')
         self.assertEqual(resolver.view_name, 'do_search')
```

### Comparing `edx-search-3.8.2/search/tests/tests.py` & `edx-search-3.9.1/search/tests/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python
 # Some of the subclasses that get used as settings-overrides will yield this pylint
 # error, but they do get used when included as part of the override_settings
-# pylint: disable=too-few-public-methods
-# pylint: disable=too-many-ancestors
 """ Tests for search functionalty """
 
 from datetime import datetime
 
 from django.core.cache import cache
 from django.test import TestCase
 from django.test.utils import override_settings
@@ -16,16 +14,14 @@
 from search.elastic import ElasticSearchEngine
 from search.tests.utils import SearcherMixin, TEST_INDEX_NAME
 from search.utils import ValueRange, DateRange
 
 from .mock_search_engine import MockSearchEngine
 
 
-# Any class that inherits from TestCase will cause too-many-public-methods pylint error
-# pylint: disable=too-many-public-methods
 @override_settings(SEARCH_ENGINE="search.tests.mock_search_engine.MockSearchEngine")
 @override_settings(ELASTIC_FIELD_MAPPINGS={"start_date": {"type": "date"}})
 @override_settings(MOCK_SEARCH_BACKING_FILE=None)
 class MockSearchTests(TestCase, SearcherMixin):
     """ Test operation of search activities """
 
     @property
```

### Comparing `edx-search-3.8.2/search/tests/utils.py` & `edx-search-3.9.1/search/tests/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -69,18 +69,17 @@
                **kwargs):  # pylint: disable=arguments-differ
         raise Exception("There is a problem here")
 
 
 class ErroringIndexEngine(MockSearchEngine):
     """ Override to generate search engine error to test """
 
-    def index(self, sources, **kwargs):  # pylint: disable=unused-argument, arguments-differ
+    def index(self, sources, **kwargs):
         raise Exception("There is a problem here")
 
 
 class ErroringElasticImpl(Elasticsearch):
     """ Elasticsearch implementation that throws exceptions"""
 
-    # pylint: disable=unused-argument
     def search(self, **kwargs):  # pylint: disable=arguments-differ
         """ this will definitely fail """
         raise exceptions.ElasticsearchException("This search operation failed")
```

### Comparing `edx-search-3.8.2/search/utils.py` & `edx-search-3.9.1/search/utils.py`

 * *Files identical despite different names*

### Comparing `edx-search-3.8.2/search/views.py` & `edx-search-3.9.1/search/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """ handle requests for courseware search http requests """
 # This contains just the url entry points to use if desired, which currently has only one
-# pylint: disable=too-few-public-methods
 
 import logging
 
 from django.conf import settings
 from django.http import JsonResponse
 from django.utils.translation import gettext as _
 from django.views.decorators.http import require_POST
 
 from eventtracking import tracker as track
 from .api import perform_search, course_discovery_search, course_discovery_filter_fields
 from .initializer import SearchInitializer
 
 # log appears to be standard name used for logger
-log = logging.getLogger(__name__)  # pylint: disable=invalid-name
+log = logging.getLogger(__name__)
 
 
 def _process_pagination_values(request):
     """ process pagination requests from request parameter """
     size = 20
     page = 0
     from_ = 0
@@ -119,16 +118,15 @@
 
     except ValueError as invalid_err:
         results = {
             "error": str(invalid_err)
         }
         log.debug(str(invalid_err))
 
-    # Allow for broad exceptions here - this is an entry point from external reference
-    except Exception as err:  # pylint: disable=broad-except
+    except Exception as err:
         results = {
             "error": _('An error occurred when searching for "{search_string}"').format(search_string=search_term)
         }
         log.exception(
             'Search view exception when searching for %s for user %s: %r',
             search_term,
             request.user.id,
@@ -205,16 +203,15 @@
 
     except ValueError as invalid_err:
         results = {
             "error": str(invalid_err)
         }
         log.debug(str(invalid_err))
 
-    # Allow for broad exceptions here - this is an entry point from external reference
-    except Exception as err:  # pylint: disable=broad-except
+    except Exception as err:
         results = {
             "error": _('An error occurred when searching for "{search_string}"').format(search_string=search_term)
         }
         log.exception(
             'Search view exception when searching for %s for user %s: %r',
             search_term,
             request.user.id,
```

### Comparing `edx-search-3.8.2/setup.py` & `edx-search-3.9.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 """ Setup to allow pip installs of edx-search module """
 import os
 import re
+from pathlib import Path
 
 from setuptools import setup
 
 
 def load_requirements(*requirements_paths):
     """
     Load all requirements from the specified requirements files.
@@ -43,19 +44,24 @@
     if version_match:
         return version_match.group(1)
     raise RuntimeError('Unable to find version string.')
 
 
 VERSION = get_version('edxsearch', '__init__.py')
 
+# read the contents of your README file
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='edx-search',
     version=VERSION,
     description='Search and index routines for index access',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author='edX',
     author_email='oscm@edx.org',
     url='https://github.com/openedx/edx-search',
     license='AGPL',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Web Environment',
```

